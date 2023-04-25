# Comparing `tmp/pyrfc-2.8.2.tar.gz` & `tmp/pyrfc-2.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrfc-2.8.2.tar", last modified: Fri Apr 21 12:20:27 2023, max compression
+gzip compressed data, was "pyrfc-2.8.3.tar", last modified: Tue Apr 25 12:12:10 2023, max compression
```

## Comparing `pyrfc-2.8.2.tar` & `pyrfc-2.8.3.tar`

### file list

```diff
@@ -1,41 +1,22 @@
-drwxr-xr-x   0 www-admin  (1000) www-admin  (1000)        0 2023-04-21 12:20:27.473173 pyrfc-2.8.2/
-drwxr-xr-x   0 www-admin  (1000) www-admin  (1000)        0 2023-04-21 12:20:27.141726 pyrfc-2.8.2/.github/
-drwxr-xr-x   0 www-admin  (1000) www-admin  (1000)        0 2023-04-21 12:20:27.230906 pyrfc-2.8.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 www-admin  (1000) www-admin  (1000)      500 2023-04-19 12:30:28.000000 pyrfc-2.8.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 www-admin  (1000) www-admin  (1000)      595 2023-04-19 12:30:28.000000 pyrfc-2.8.2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 www-admin  (1000) www-admin  (1000)      344 2023-04-19 12:30:28.000000 pyrfc-2.8.2/.gitignore
-drwxr-xr-x   0 www-admin  (1000) www-admin  (1000)        0 2023-04-21 12:20:27.237775 pyrfc-2.8.2/.reuse/
--rw-r--r--   0 www-admin  (1000) www-admin  (1000)     2204 2023-04-19 12:30:28.000000 pyrfc-2.8.2/.reuse/dep5
--rw-r--r--   0 www-admin  (1000) www-admin  (1000)     4622 2023-04-19 12:30:28.000000 pyrfc-2.8.2/CONTRIBUTING.md
--rw-r--r--   0 www-admin  (1000) www-admin  (1000)    10273 2023-04-19 12:30:28.000000 pyrfc-2.8.2/LICENSE
-drwxr-xr-x   0 www-admin  (1000) www-admin  (1000)        0 2023-04-21 12:20:27.250953 pyrfc-2.8.2/LICENSES/
--rw-r--r--   0 www-admin  (1000) www-admin  (1000)    10283 2023-04-19 12:30:28.000000 pyrfc-2.8.2/LICENSES/Apache-2.0.txt
--rw-r--r--   0 www-admin  (1000) www-admin  (1000)       79 2023-04-21 09:26:32.000000 pyrfc-2.8.2/MANIFEST.in
--rw-r--r--   0 www-admin  (1000) www-admin  (1000)    11327 2023-04-21 12:20:27.467899 pyrfc-2.8.2/PKG-INFO
--rw-r--r--   0 www-admin  (1000) www-admin  (1000)    10133 2023-04-20 09:35:50.000000 pyrfc-2.8.2/README.md
-drwxr-xr-x   0 www-admin  (1000) www-admin  (1000)        0 2023-04-21 12:20:27.157668 pyrfc-2.8.2/ci/
-drwxr-xr-x   0 www-admin  (1000) www-admin  (1000)        0 2023-04-21 12:20:27.297636 pyrfc-2.8.2/ci/utils/
--rw-r--r--   0 www-admin  (1000) www-admin  (1000)      742 2023-04-20 10:41:23.000000 pyrfc-2.8.2/ci/utils/build.ps1
--rwxr-xr-x   0 www-admin  (1000) www-admin  (1000)      813 2023-04-21 09:03:15.000000 pyrfc-2.8.2/ci/utils/build.sh
--rwxr-xr-x   0 www-admin  (1000) www-admin  (1000)     1393 2023-04-19 12:30:28.000000 pyrfc-2.8.2/ci/utils/paths_fix.sh
--rwxr-xr-x   0 www-admin  (1000) www-admin  (1000)      228 2023-04-19 12:30:28.000000 pyrfc-2.8.2/ci/utils/paths_show.sh
--rw-r--r--   0 www-admin  (1000) www-admin  (1000)      168 2023-04-20 08:17:45.000000 pyrfc-2.8.2/pyproject.toml
--rwxr-xr-x   0 www-admin  (1000) www-admin  (1000)       27 2023-04-19 12:30:28.000000 pyrfc-2.8.2/pytest.ini
--rw-r--r--   0 www-admin  (1000) www-admin  (1000)       38 2023-04-21 12:20:27.474420 pyrfc-2.8.2/setup.cfg
--rwxr-xr-x   0 www-admin  (1000) www-admin  (1000)     7897 2023-04-21 11:58:45.000000 pyrfc-2.8.2/setup.py
-drwxr-xr-x   0 www-admin  (1000) www-admin  (1000)        0 2023-04-21 12:20:27.166260 pyrfc-2.8.2/src/
-drwxr-xr-x   0 www-admin  (1000) www-admin  (1000)        0 2023-04-21 12:20:27.416090 pyrfc-2.8.2/src/pyrfc/
--rwxr-xr-x   0 www-admin  (1000) www-admin  (1000)     1602 2023-04-21 11:32:40.000000 pyrfc-2.8.2/src/pyrfc/__init__.py
--rw-r--r--   0 www-admin  (1000) www-admin  (1000)  2278009 2023-04-21 12:20:23.000000 pyrfc-2.8.2/src/pyrfc/_cyrfc.cpp
--rwxr-xr-x   0 www-admin  (1000) www-admin  (1000)   129750 2023-04-21 11:56:06.000000 pyrfc-2.8.2/src/pyrfc/_cyrfc.pyx
--rwxr-xr-x   0 www-admin  (1000) www-admin  (1000)     5594 2023-04-21 11:41:36.000000 pyrfc-2.8.2/src/pyrfc/_exception.py
--rw-r--r--   0 www-admin  (1000) www-admin  (1000)      292 2023-04-21 11:30:18.000000 pyrfc-2.8.2/src/pyrfc/_utils.py
--rwxr-xr-x   0 www-admin  (1000) www-admin  (1000)    23820 2023-04-21 11:13:00.000000 pyrfc-2.8.2/src/pyrfc/csapnwrfc.pxd
--rw-r--r--   0 www-admin  (1000) www-admin  (1000)       86 2023-04-21 12:00:34.000000 pyrfc-2.8.2/src/pyrfc/version.py
-drwxr-xr-x   0 www-admin  (1000) www-admin  (1000)        0 2023-04-21 12:20:27.458869 pyrfc-2.8.2/src/pyrfc.egg-info/
--rw-r--r--   0 www-admin  (1000) www-admin  (1000)    11327 2023-04-21 12:20:26.000000 pyrfc-2.8.2/src/pyrfc.egg-info/PKG-INFO
--rw-r--r--   0 www-admin  (1000) www-admin  (1000)      637 2023-04-21 12:20:27.000000 pyrfc-2.8.2/src/pyrfc.egg-info/SOURCES.txt
--rw-r--r--   0 www-admin  (1000) www-admin  (1000)        1 2023-04-21 12:20:26.000000 pyrfc-2.8.2/src/pyrfc.egg-info/dependency_links.txt
--rw-r--r--   0 www-admin  (1000) www-admin  (1000)        1 2023-04-20 08:28:07.000000 pyrfc-2.8.2/src/pyrfc.egg-info/not-zip-safe
--rw-r--r--   0 www-admin  (1000) www-admin  (1000)       46 2023-04-21 12:20:26.000000 pyrfc-2.8.2/src/pyrfc.egg-info/requires.txt
--rw-r--r--   0 www-admin  (1000) www-admin  (1000)        6 2023-04-21 12:20:26.000000 pyrfc-2.8.2/src/pyrfc.egg-info/top_level.txt
+drwxr-xr-x   0 www-admin  (1000) www-admin  (1000)        0 2023-04-25 12:12:10.271593 pyrfc-2.8.3/
+drwxr-xr-x   0 www-admin  (1000) www-admin  (1000)        0 2023-04-25 12:12:10.088322 pyrfc-2.8.3/LICENSES/
+-rw-r--r--   0 www-admin  (1000) www-admin  (1000)    10283 2023-04-24 08:04:52.000000 pyrfc-2.8.3/LICENSES/Apache-2.0.txt
+-rw-r--r--   0 www-admin  (1000) www-admin  (1000)       58 2023-04-25 11:34:22.000000 pyrfc-2.8.3/MANIFEST.in
+-rw-r--r--   0 www-admin  (1000) www-admin  (1000)    23387 2023-04-25 12:12:10.268527 pyrfc-2.8.3/PKG-INFO
+-rw-r--r--   0 www-admin  (1000) www-admin  (1000)    10174 2023-04-24 17:43:16.000000 pyrfc-2.8.3/README.md
+-rw-r--r--   0 www-admin  (1000) www-admin  (1000)     1814 2023-04-25 11:44:27.000000 pyrfc-2.8.3/pyproject.toml
+-rw-r--r--   0 www-admin  (1000) www-admin  (1000)       38 2023-04-25 12:12:10.272447 pyrfc-2.8.3/setup.cfg
+-rw-r--r--   0 www-admin  (1000) www-admin  (1000)     5727 2023-04-25 11:38:06.000000 pyrfc-2.8.3/setup.py
+drwxr-xr-x   0 www-admin  (1000) www-admin  (1000)        0 2023-04-25 12:12:10.061019 pyrfc-2.8.3/src/
+drwxr-xr-x   0 www-admin  (1000) www-admin  (1000)        0 2023-04-25 12:12:10.185932 pyrfc-2.8.3/src/pyrfc/
+-rwxr-xr-x   0 www-admin  (1000) www-admin  (1000)     1330 2023-04-25 11:34:43.000000 pyrfc-2.8.3/src/pyrfc/__init__.py
+-rw-r--r--   0 www-admin  (1000) www-admin  (1000)  2313573 2023-04-25 12:12:04.000000 pyrfc-2.8.3/src/pyrfc/_cyrfc.cpp
+-rwxr-xr-x   0 www-admin  (1000) www-admin  (1000)   129750 2023-04-24 08:04:53.000000 pyrfc-2.8.3/src/pyrfc/_cyrfc.pyx
+-rwxr-xr-x   0 www-admin  (1000) www-admin  (1000)     5596 2023-04-25 11:38:52.000000 pyrfc-2.8.3/src/pyrfc/_exception.py
+-rw-r--r--   0 www-admin  (1000) www-admin  (1000)      293 2023-04-25 11:38:47.000000 pyrfc-2.8.3/src/pyrfc/_utils.py
+-rwxr-xr-x   0 www-admin  (1000) www-admin  (1000)    23820 2023-04-24 08:04:53.000000 pyrfc-2.8.3/src/pyrfc/csapnwrfc.pxd
+drwxr-xr-x   0 www-admin  (1000) www-admin  (1000)        0 2023-04-25 12:12:10.259500 pyrfc-2.8.3/src/pyrfc.egg-info/
+-rw-r--r--   0 www-admin  (1000) www-admin  (1000)    23387 2023-04-25 12:12:09.000000 pyrfc-2.8.3/src/pyrfc.egg-info/PKG-INFO
+-rw-r--r--   0 www-admin  (1000) www-admin  (1000)      333 2023-04-25 12:12:10.000000 pyrfc-2.8.3/src/pyrfc.egg-info/SOURCES.txt
+-rw-r--r--   0 www-admin  (1000) www-admin  (1000)        1 2023-04-25 12:12:09.000000 pyrfc-2.8.3/src/pyrfc.egg-info/dependency_links.txt
+-rw-r--r--   0 www-admin  (1000) www-admin  (1000)        6 2023-04-25 12:12:09.000000 pyrfc-2.8.3/src/pyrfc.egg-info/top_level.txt
```

### Comparing `pyrfc-2.8.2/LICENSE` & `pyrfc-2.8.3/LICENSES/Apache-2.0.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,85 +1,208 @@
 Apache License
+
 Version 2.0, January 2004
-http://www.apache.org/licenses/
 
-TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+http://www.apache.org/licenses/ TERMS AND CONDITIONS FOR USE, REPRODUCTION,
+AND DISTRIBUTION
+
+   1. Definitions.
+
+
+
+"License" shall mean the terms and conditions for use, reproduction, and distribution
+as defined by Sections 1 through 9 of this document.
+
+
+
+"Licensor" shall mean the copyright owner or entity authorized by the copyright
+owner that is granting the License.
+
+
+
+"Legal Entity" shall mean the union of the acting entity and all other entities
+that control, are controlled by, or are under common control with that entity.
+For the purposes of this definition, "control" means (i) the power, direct
+or indirect, to cause the direction or management of such entity, whether
+by contract or otherwise, or (ii) ownership of fifty percent (50%) or more
+of the outstanding shares, or (iii) beneficial ownership of such entity.
+
+
+
+"You" (or "Your") shall mean an individual or Legal Entity exercising permissions
+granted by this License.
+
+
+
+"Source" form shall mean the preferred form for making modifications, including
+but not limited to software source code, documentation source, and configuration
+files.
+
+
+
+"Object" form shall mean any form resulting from mechanical transformation
+or translation of a Source form, including but not limited to compiled object
+code, generated documentation, and conversions to other media types.
+
+
 
-1. Definitions.
+"Work" shall mean the work of authorship, whether in Source or Object form,
+made available under the License, as indicated by a copyright notice that
+is included in or attached to the work (an example is provided in the Appendix
+below).
 
-"License" shall mean the terms and conditions for use, reproduction, and distribution as defined by Sections 1 through 9 of this document.
 
-"Licensor" shall mean the copyright owner or entity authorized by the copyright owner that is granting the License.
 
-"Legal Entity" shall mean the union of the acting entity and all other entities that control, are controlled by, or are under common control with that entity. For the purposes of this definition, "control" means (i) the power, direct or indirect, to cause the direction or management of such entity, whether by contract or otherwise, or (ii) ownership of fifty percent (50%) or more of the outstanding shares, or (iii) beneficial ownership of such entity.
+"Derivative Works" shall mean any work, whether in Source or Object form,
+that is based on (or derived from) the Work and for which the editorial revisions,
+annotations, elaborations, or other modifications represent, as a whole, an
+original work of authorship. For the purposes of this License, Derivative
+Works shall not include works that remain separable from, or merely link (or
+bind by name) to the interfaces of, the Work and Derivative Works thereof.
 
-"You" (or "Your") shall mean an individual or Legal Entity exercising permissions granted by this License.
 
-"Source" form shall mean the preferred form for making modifications, including but not limited to software source code, documentation source, and configuration files.
 
-"Object" form shall mean any form resulting from mechanical transformation or translation of a Source form, including but not limited to compiled object code, generated documentation, and conversions to other media types.
+"Contribution" shall mean any work of authorship, including the original version
+of the Work and any modifications or additions to that Work or Derivative
+Works thereof, that is intentionally submitted to Licensor for inclusion in
+the Work by the copyright owner or by an individual or Legal Entity authorized
+to submit on behalf of the copyright owner. For the purposes of this definition,
+"submitted" means any form of electronic, verbal, or written communication
+sent to the Licensor or its representatives, including but not limited to
+communication on electronic mailing lists, source code control systems, and
+issue tracking systems that are managed by, or on behalf of, the Licensor
+for the purpose of discussing and improving the Work, but excluding communication
+that is conspicuously marked or otherwise designated in writing by the copyright
+owner as "Not a Contribution."
 
-"Work" shall mean the work of authorship, whether in Source or Object form, made available under the License, as indicated by a copyright notice that is included in or attached to the work (an example is provided in the Appendix below).
 
-"Derivative Works" shall mean any work, whether in Source or Object form, that is based on (or derived from) the Work and for which the editorial revisions, annotations, elaborations, or other modifications represent, as a whole, an original work of authorship. For the purposes of this License, Derivative Works shall not include works that remain separable from, or merely link (or bind by name) to the interfaces of, the Work and Derivative Works thereof.
 
-"Contribution" shall mean any work of authorship, including the original version of the Work and any modifications or additions to that Work or Derivative Works thereof, that is intentionally submitted to Licensor for inclusion in the Work by the copyright owner or by an individual or Legal Entity authorized to submit on behalf of the copyright owner. For the purposes of this definition, "submitted" means any form of electronic, verbal, or written communication sent to the Licensor or its representatives, including but not limited to communication on electronic mailing lists, source code control systems, and issue tracking systems that are managed by, or on behalf of, the Licensor for the purpose of discussing and improving the Work, but excluding communication that is conspicuously marked or otherwise designated in writing by the copyright owner as "Not a Contribution."
+"Contributor" shall mean Licensor and any individual or Legal Entity on behalf
+of whom a Contribution has been received by Licensor and subsequently incorporated
+within the Work.
 
-"Contributor" shall mean Licensor and any individual or Legal Entity on behalf of whom a Contribution has been received by Licensor and subsequently incorporated within the Work.
+2. Grant of Copyright License. Subject to the terms and conditions of this
+License, each Contributor hereby grants to You a perpetual, worldwide, non-exclusive,
+no-charge, royalty-free, irrevocable copyright license to reproduce, prepare
+Derivative Works of, publicly display, publicly perform, sublicense, and distribute
+the Work and such Derivative Works in Source or Object form.
 
-2. Grant of Copyright License.
+3. Grant of Patent License. Subject to the terms and conditions of this License,
+each Contributor hereby grants to You a perpetual, worldwide, non-exclusive,
+no-charge, royalty-free, irrevocable (except as stated in this section) patent
+license to make, have made, use, offer to sell, sell, import, and otherwise
+transfer the Work, where such license applies only to those patent claims
+licensable by such Contributor that are necessarily infringed by their Contribution(s)
+alone or by combination of their Contribution(s) with the Work to which such
+Contribution(s) was submitted. If You institute patent litigation against
+any entity (including a cross-claim or counterclaim in a lawsuit) alleging
+that the Work or a Contribution incorporated within the Work constitutes direct
+or contributory patent infringement, then any patent licenses granted to You
+under this License for that Work shall terminate as of the date such litigation
+is filed.
 
-Subject to the terms and conditions of this License, each Contributor hereby grants to You a perpetual, worldwide, non-exclusive, no-charge, royalty-free, irrevocable copyright license to reproduce, prepare Derivative Works of, publicly display, publicly perform, sublicense, and distribute the Work and such Derivative Works in Source or Object form.
+4. Redistribution. You may reproduce and distribute copies of the Work or
+Derivative Works thereof in any medium, with or without modifications, and
+in Source or Object form, provided that You meet the following conditions:
 
-3. Grant of Patent License.
+(a) You must give any other recipients of the Work or Derivative Works a copy
+of this License; and
 
-Subject to the terms and conditions of this License, each Contributor hereby grants to You a perpetual, worldwide, non-exclusive, no-charge, royalty-free, irrevocable (except as stated in this section) patent license to make, have made, use, offer to sell, sell, import, and otherwise transfer the Work, where such license applies only to those patent claims licensable by such Contributor that are necessarily infringed by their Contribution(s) alone or by combination of their Contribution(s) with the Work to which such Contribution(s) was submitted. If You institute patent litigation against any entity (including a cross-claim or counterclaim in a lawsuit) alleging that the Work or a Contribution incorporated within the Work constitutes direct or contributory patent infringement, then any patent licenses granted to You under this License for that Work shall terminate as of the date such litigation is filed.
+(b) You must cause any modified files to carry prominent notices stating that
+You changed the files; and
 
-4. Redistribution.
+(c) You must retain, in the Source form of any Derivative Works that You distribute,
+all copyright, patent, trademark, and attribution notices from the Source
+form of the Work, excluding those notices that do not pertain to any part
+of the Derivative Works; and
 
-You may reproduce and distribute copies of the Work or Derivative Works thereof in any medium, with or without modifications, and in Source or Object form, provided that You meet the following conditions:
+(d) If the Work includes a "NOTICE" text file as part of its distribution,
+then any Derivative Works that You distribute must include a readable copy
+of the attribution notices contained within such NOTICE file, excluding those
+notices that do not pertain to any part of the Derivative Works, in at least
+one of the following places: within a NOTICE text file distributed as part
+of the Derivative Works; within the Source form or documentation, if provided
+along with the Derivative Works; or, within a display generated by the Derivative
+Works, if and wherever such third-party notices normally appear. The contents
+of the NOTICE file are for informational purposes only and do not modify the
+License. You may add Your own attribution notices within Derivative Works
+that You distribute, alongside or as an addendum to the NOTICE text from the
+Work, provided that such additional attribution notices cannot be construed
+as modifying the License.
 
-You must give any other recipients of the Work or Derivative Works a copy of this License; and
-You must cause any modified files to carry prominent notices stating that You changed the files; and
-You must retain, in the Source form of any Derivative Works that You distribute, all copyright, patent, trademark, and attribution notices from the Source form of the Work, excluding those notices that do not pertain to any part of the Derivative Works; and
-If the Work includes a "NOTICE" text file as part of its distribution, then any Derivative Works that You distribute must include a readable copy of the attribution notices contained within such NOTICE file, excluding those notices that do not pertain to any part of the Derivative Works, in at least one of the following places: within a NOTICE text file distributed as part of the Derivative Works; within the Source form or documentation, if provided along with the Derivative Works; or, within a display generated by the Derivative Works, if and wherever such third-party notices normally appear. The contents of the NOTICE file are for informational purposes only and do not modify the License. You may add Your own attribution notices within Derivative Works that You distribute, alongside or as an addendum to the NOTICE text from the Work, provided that such additional attribution notices cannot be construed as modifying the License.
-You may add Your own copyright statement to Your modifications and may provide additional or different license terms and conditions for use, reproduction, or distribution of Your modifications, or for any such Derivative Works as a whole, provided Your use, reproduction, and distribution of the Work otherwise complies with the conditions stated in this License.
+You may add Your own copyright statement to Your modifications and may provide
+additional or different license terms and conditions for use, reproduction,
+or distribution of Your modifications, or for any such Derivative Works as
+a whole, provided Your use, reproduction, and distribution of the Work otherwise
+complies with the conditions stated in this License.
 
-5. Submission of Contributions.
+5. Submission of Contributions. Unless You explicitly state otherwise, any
+Contribution intentionally submitted for inclusion in the Work by You to the
+Licensor shall be under the terms and conditions of this License, without
+any additional terms or conditions. Notwithstanding the above, nothing herein
+shall supersede or modify the terms of any separate license agreement you
+may have executed with Licensor regarding such Contributions.
 
-Unless You explicitly state otherwise, any Contribution intentionally submitted for inclusion in the Work by You to the Licensor shall be under the terms and conditions of this License, without any additional terms or conditions. Notwithstanding the above, nothing herein shall supersede or modify the terms of any separate license agreement you may have executed with Licensor regarding such Contributions.
+6. Trademarks. This License does not grant permission to use the trade names,
+trademarks, service marks, or product names of the Licensor, except as required
+for reasonable and customary use in describing the origin of the Work and
+reproducing the content of the NOTICE file.
 
-6. Trademarks.
+7. Disclaimer of Warranty. Unless required by applicable law or agreed to
+in writing, Licensor provides the Work (and each Contributor provides its
+Contributions) on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
+KIND, either express or implied, including, without limitation, any warranties
+or conditions of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR
+A PARTICULAR PURPOSE. You are solely responsible for determining the appropriateness
+of using or redistributing the Work and assume any risks associated with Your
+exercise of permissions under this License.
 
-This License does not grant permission to use the trade names, trademarks, service marks, or product names of the Licensor, except as required for reasonable and customary use in describing the origin of the Work and reproducing the content of the NOTICE file.
+8. Limitation of Liability. In no event and under no legal theory, whether
+in tort (including negligence), contract, or otherwise, unless required by
+applicable law (such as deliberate and grossly negligent acts) or agreed to
+in writing, shall any Contributor be liable to You for damages, including
+any direct, indirect, special, incidental, or consequential damages of any
+character arising as a result of this License or out of the use or inability
+to use the Work (including but not limited to damages for loss of goodwill,
+work stoppage, computer failure or malfunction, or any and all other commercial
+damages or losses), even if such Contributor has been advised of the possibility
+of such damages.
 
-7. Disclaimer of Warranty.
+9. Accepting Warranty or Additional Liability. While redistributing the Work
+or Derivative Works thereof, You may choose to offer, and charge a fee for,
+acceptance of support, warranty, indemnity, or other liability obligations
+and/or rights consistent with this License. However, in accepting such obligations,
+You may act only on Your own behalf and on Your sole responsibility, not on
+behalf of any other Contributor, and only if You agree to indemnify, defend,
+and hold each Contributor harmless for any liability incurred by, or claims
+asserted against, such Contributor by reason of your accepting any such warranty
+or additional liability. END OF TERMS AND CONDITIONS
 
-Unless required by applicable law or agreed to in writing, Licensor provides the Work (and each Contributor provides its Contributions) on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied, including, without limitation, any warranties or conditions of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A PARTICULAR PURPOSE. You are solely responsible for determining the appropriateness of using or redistributing the Work and assume any risks associated with Your exercise of permissions under this License.
+APPENDIX: How to apply the Apache License to your work.
 
-8. Limitation of Liability.
+To apply the Apache License to your work, attach the following boilerplate
+notice, with the fields enclosed by brackets "[]" replaced with your own identifying
+information. (Don't include the brackets!) The text should be enclosed in
+the appropriate comment syntax for the file format. We also recommend that
+a file or class name and description of purpose be included on the same "printed
+page" as the copyright notice for easier identification within third-party
+archives.
 
-In no event and under no legal theory, whether in tort (including negligence), contract, or otherwise, unless required by applicable law (such as deliberate and grossly negligent acts) or agreed to in writing, shall any Contributor be liable to You for damages, including any direct, indirect, special, incidental, or consequential damages of any character arising as a result of this License or out of the use or inability to use the Work (including but not limited to damages for loss of goodwill, work stoppage, computer failure or malfunction, or any and all other commercial damages or losses), even if such Contributor has been advised of the possibility of such damages.
+Copyright [yyyy] [name of copyright owner]
 
-9. Accepting Warranty or Additional Liability.
+Licensed under the Apache License, Version 2.0 (the "License");
 
-While redistributing the Work or Derivative Works thereof, You may choose to offer, and charge a fee for, acceptance of support, warranty, indemnity, or other liability obligations and/or rights consistent with this License. However, in accepting such obligations, You may act only on Your own behalf and on Your sole responsibility, not on behalf of any other Contributor, and only if You agree to indemnify, defend, and hold each Contributor harmless for any liability incurred by, or claims asserted against, such Contributor by reason of your accepting any such warranty or additional liability.
+you may not use this file except in compliance with the License.
 
-END OF TERMS AND CONDITIONS
+You may obtain a copy of the License at
 
-APPENDIX: How to apply the Apache License to your work
+http://www.apache.org/licenses/LICENSE-2.0
 
-To apply the Apache License to your work, attach the following boilerplate notice, with the fields enclosed by brackets "[]" replaced with your own identifying information. (Don't include the brackets!) The text should be enclosed in the appropriate comment syntax for the file format. We also recommend that a file or class name and description of purpose be included on the same "printed page" as the copyright notice for easier identification within third-party archives.
+Unless required by applicable law or agreed to in writing, software
 
-   Copyright [yyyy] [name of copyright owner]
+distributed under the License is distributed on an "AS IS" BASIS,
 
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 
-     http://www.apache.org/licenses/LICENSE-2.0
+See the License for the specific language governing permissions and
 
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+limitations under the License.
```

### Comparing `pyrfc-2.8.2/PKG-INFO` & `pyrfc-2.8.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,7 @@
-Metadata-Version: 2.1
-Name: pyrfc
-Version: 2.8.2
-Summary: Python bindings for SAP NetWeaver RFC SDK
-Home-page: https://github.com/SAP/pyrfc
-Download-URL: https://github.com/SAP/PyRFC/tarball/master
-Author: SAP SE
-Maintainer: Srdjan Boskovic
-Maintainer-email: srdjan.boskovic@sap.com
-License: OSI Approved :: Apache Software License
-Keywords: _cyrfc pyrfc pyrfc sap rfc nwrfc sapnwrfc
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Cython
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Software Development :: Libraries
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <h1>PyRFC</h1>
 
 Asynchronous, non-blocking [SAP NetWeawer RFC SDK](https://support.sap.com/en/product/connectors/nwrfcsdk.html) bindings for Python.
 
 [![license](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![PyPI - Wheel](https://img.shields.io/pypi/wheel/pyrfc)](https://pypi.org/project/pyrfc/)
 [![PyPI - Version](https://img.shields.io/pypi/v/pyrfc)](https://pypi.org/project/pyrfc/)
@@ -109,30 +80,32 @@
 
 ## Download and installation
 
 ```shell
 pip install pyrfc
 ```
 
-Cython is required on Linux platforms, for the the default build from source installation method.
+Cython must be installed upfront because the build from source is standard installation method on Linux.
 
-Build from source can be also requested on Windows and Darwin platforms:
+Build from source can be requested also on other platforms:
 
 ```shell
 pip install pyrfc --no-binary :all:
 # or
 PYRFC_BUILD_CYTHON=yes pip install pyrfc --no-binary :all:
 ```
 
 Alternative build from source installation:
 
 ```shell
 git clone https://github.com/SAP/PyRFC.git
 cd PyRFC
-python setup.py bdist_wheel
+python -m pip install .
+# or
+python -m build --wheel --sdist --outdir dist
 pip install --upgrade --no-index --find-links=dist pyrfc
 ```
 
 See also the [pyrfc documentation](http://sap.github.io/PyRFC),
 complementing _SAP NWRFC SDK_[documentation](https://support.sap.com/nwrfcsdk), especially [SAP NWRFC SDK 7.50 Programming Guide](https://support.sap.com/content/dam/support/en_us/library/ssp/products/connectors/nwrfcsdk/NW_RFC_750_ProgrammingGuide.pdf).
 
 ## Getting started
```

### Comparing `pyrfc-2.8.2/src/pyrfc/__init__.py` & `pyrfc-2.8.3/src/pyrfc/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 # SPDX-FileCopyrightText: 2013 SAP SE Srdjan Boskovic <srdjan.boskovic@sap.com>
 #
 # SPDX-License-Identifier: Apache-2.0
 
-# import from internal modules that they could be directly imported from
-# the pyrfc package
-
-# Set DLL path, per https://docs.python.org/3.8/whatsnew/3.8.html#bpo-36085-whatsnew
-
+import importlib.metadata
 import os
-from .version import __version_info__, __version__
+
+__version__ = importlib.metadata.version("pyrfc")
+__version_info__ = tuple(__version__.split("."))
 
 if os.name == "nt":
+    # Set DLL path, per https://docs.python.org/3.8/whatsnew/3.8.html#bpo-36085-whatsnew
     try:
         os.add_dll_directory(os.path.join(os.environ["SAPNWRFC_HOME"], "lib"))
     except Exception:
         pass
 
 from ._exception import (
     RFCError,
@@ -26,39 +25,32 @@
     ExternalAuthorizationError,
     ExternalApplicationError,
     ExternalRuntimeError,
 )
 
 from ._utils import py_to_string, string_to_py
 
-try:
-    from ._cyrfc import (
-        get_nwrfclib_version,
-        reload_ini_file,
-        set_ini_file_directory,
-        set_cryptolib_path,
-        set_locale_radix,
-        language_iso_to_sap,
-        language_sap_to_iso,
-        cancel_connection,
-        Connection,
-        ConnectionParameters,
-        Decimal,
-        Throughput,
-        TypeDescription,
-        FunctionDescription,
-        Server,
-        UnitCallType,
-        UnitState,
-        RCStatus,
-        RfcParameterDirection,
-        RfcFieldType
-    )
-except ModuleNotFoundError as ex:
-    if "'src.pyrfc._cyrfc'" in ex.msg:
-        # is ok, call from setup.py build
-        pass
-    else:
-        raise ex
+from ._cyrfc import (
+    get_nwrfclib_version,
+    reload_ini_file,
+    set_ini_file_directory,
+    set_cryptolib_path,
+    set_locale_radix,
+    language_iso_to_sap,
+    language_sap_to_iso,
+    cancel_connection,
+    Connection,
+    ConnectionParameters,
+    Decimal,
+    Throughput,
+    TypeDescription,
+    FunctionDescription,
+    Server,
+    UnitCallType,
+    UnitState,
+    RCStatus,
+    RfcParameterDirection,
+    RfcFieldType
+)
 
 __author__ = "SAP SE"
 __email__ = "srdjan.boskovic@sap.com"
```

### Comparing `pyrfc-2.8.2/src/pyrfc/_cyrfc.cpp` & `pyrfc-2.8.3/src/pyrfc/_cyrfc.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
 #define CYTHON_ABI "0_29_34"
 #define CYTHON_HEX_VERSION 0x001D22F0
-#define CYTHON_FUTURE_DIVISION 0
+#define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
     #define __stdcall
@@ -1611,21 +1611,14 @@
 
 /* BytesEquals.proto */
 static CYTHON_INLINE int __Pyx_PyBytes_Equals(PyObject* s1, PyObject* s2, int equals);
 
 /* UnicodeEquals.proto */
 static CYTHON_INLINE int __Pyx_PyUnicode_Equals(PyObject* s1, PyObject* s2, int equals);
 
-/* StrEquals.proto */
-#if PY_MAJOR_VERSION >= 3
-#define __Pyx_PyString_Equals __Pyx_PyUnicode_Equals
-#else
-#define __Pyx_PyString_Equals __Pyx_PyBytes_Equals
-#endif
-
 /* GetException.proto */
 #if CYTHON_FAST_THREAD_STATE
 #define __Pyx_GetException(type, value, tb)  __Pyx__GetException(__pyx_tstate, type, value, tb)
 static int __Pyx__GetException(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
 #else
 static int __Pyx_GetException(PyObject **type, PyObject **value, PyObject **tb);
 #endif
@@ -1760,39 +1753,28 @@
     ((likely((Py_TYPE(obj) == type) | (none_allowed && (obj == Py_None)))) ? 1 :\
         __Pyx__ArgTypeTest(obj, type, name, exact))
 static int __Pyx__ArgTypeTest(PyObject *obj, PyTypeObject *type, const char *name, int exact);
 
 /* ReRaiseException.proto */
 static CYTHON_INLINE void __Pyx_ReraiseException(void);
 
-/* StringJoin.proto */
-#if PY_MAJOR_VERSION < 3
-#define __Pyx_PyString_Join __Pyx_PyBytes_Join
-#define __Pyx_PyBaseString_Join(s, v) (PyUnicode_CheckExact(s) ? PyUnicode_Join(s, v) : __Pyx_PyBytes_Join(s, v))
-#else
-#define __Pyx_PyString_Join PyUnicode_Join
-#define __Pyx_PyBaseString_Join PyUnicode_Join
-#endif
-#if CYTHON_COMPILING_IN_CPYTHON
-    #if PY_MAJOR_VERSION < 3
-    #define __Pyx_PyBytes_Join _PyString_Join
-    #else
-    #define __Pyx_PyBytes_Join _PyBytes_Join
-    #endif
-#else
-static CYTHON_INLINE PyObject* __Pyx_PyBytes_Join(PyObject* sep, PyObject* values);
-#endif
-
 /* PyObjectFormat.proto */
 #if CYTHON_USE_UNICODE_WRITER
 static PyObject* __Pyx_PyObject_Format(PyObject* s, PyObject* f);
 #else
 #define __Pyx_PyObject_Format(s, f) PyObject_Format(s, f)
 #endif
 
+/* CIntToPyUnicode.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyUnicode_From_RFCTYPE(RFCTYPE value, Py_ssize_t width, char padding_char, char format_char);
+
+/* PyObjectFormatAndDecref.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyObject_FormatSimpleAndDecref(PyObject* s, PyObject* f);
+static CYTHON_INLINE PyObject* __Pyx_PyObject_FormatAndDecref(PyObject* s, PyObject* f);
+
 /* PyDictContains.proto */
 static CYTHON_INLINE int __Pyx_PyDict_ContainsTF(PyObject* item, PyObject* dict, int eq) {
     int result = PyDict_Contains(dict, item);
     return unlikely(result < 0) ? result : (result == (eq == Py_EQ));
 }
 
 /* dict_getitem_default.proto */
@@ -1984,21 +1966,14 @@
 static PyCodeObject *__pyx_find_code_object(int code_line);
 static void __pyx_insert_code_object(int code_line, PyCodeObject* code_object);
 
 /* AddTraceback.proto */
 static void __Pyx_AddTraceback(const char *funcname, int c_line,
                                int py_line, const char *filename);
 
-/* Print.proto */
-static int __Pyx_Print(PyObject*, PyObject *, int);
-#if CYTHON_COMPILING_IN_PYPY || PY_MAJOR_VERSION >= 3
-static PyObject* __pyx_print = 0;
-static PyObject* __pyx_print_kwargs = 0;
-#endif
-
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_RFC_DIRECTION(RFC_DIRECTION value);
 
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_RFCTYPE(RFCTYPE value);
 
 /* CIntToPy.proto */
@@ -2063,17 +2038,14 @@
 
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_RFC_INT2(RFC_INT2 value);
 
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_RFC_INT8(RFC_INT8 value);
 
-/* PrintOne.proto */
-static int __Pyx_PrintOne(PyObject* stream, PyObject *o);
-
 /* CIntFromPy.proto */
 static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *);
 
 /* CStringEquals.proto */
 static CYTHON_INLINE int __Pyx_StrEq(const char *, const char *);
 
 /* CheckBinaryVersion.proto */
@@ -2141,53 +2113,53 @@
 
 /* Implementation of 'pyrfc._cyrfc' */
 static PyObject *__pyx_builtin_object;
 static PyObject *__pyx_builtin_staticmethod;
 static PyObject *__pyx_builtin_TypeError;
 static PyObject *__pyx_builtin_range;
 static PyObject *__pyx_builtin_enumerate;
+static PyObject *__pyx_builtin_print;
 static const char __pyx_k_Q[] = "Q";
 static const char __pyx_k_T[] = "T";
+static const char __pyx_k_d[] = "d";
 static const char __pyx_k_t[] = "t";
 static const char __pyx_k_02[] = "02";
 static const char __pyx_k_04[] = "04";
 static const char __pyx_k_OK[] = "OK";
 static const char __pyx_k__3[] = "/";
 static const char __pyx_k__4[] = ")>";
 static const char __pyx_k__5[] = "";
 static const char __pyx_k__6[] = "'";
 static const char __pyx_k_id[] = "id";
 static const char __pyx_k_rc[] = "rc";
 static const char __pyx_k_TID[] = "TID ";
 static const char __pyx_k_UTC[] = " UTC] ";
-static const char __pyx_k__20[] = ".";
-static const char __pyx_k__23[] = "[";
-static const char __pyx_k__24[] = " '";
-static const char __pyx_k__27[] = "'.";
-static const char __pyx_k__28[] = ").";
-static const char __pyx_k__45[] = "\000";
-static const char __pyx_k__50[] = "*";
+static const char __pyx_k__21[] = ".";
+static const char __pyx_k__24[] = "[";
+static const char __pyx_k__25[] = " '";
+static const char __pyx_k__28[] = "'.";
+static const char __pyx_k__29[] = ").";
+static const char __pyx_k__46[] = "\000";
+static const char __pyx_k__51[] = "*";
 static const char __pyx_k_add[] = "add";
 static const char __pyx_k_day[] = "day";
 static const char __pyx_k_del[] = "__del__";
 static const char __pyx_k_doc[] = "__doc__";
-static const char __pyx_k_end[] = "end";
 static const char __pyx_k_get[] = "get";
 static const char __pyx_k_key[] = "key";
 static const char __pyx_k_rel[] = "rel";
 static const char __pyx_k_sys[] = "sys";
 static const char __pyx_k_Enum[] = "Enum";
 static const char __pyx_k_Unit[] = "Unit ";
 static const char __pyx_k_args[] = "args";
 static const char __pyx_k_auto[] = "auto";
 static const char __pyx_k_code[] = "code";
 static const char __pyx_k_date[] = "date";
 static const char __pyx_k_dest[] = "dest";
 static const char __pyx_k_enum[] = "enum";
-static const char __pyx_k_file[] = "file";
 static const char __pyx_k_free[] = "_free";
 static const char __pyx_k_host[] = "host";
 static const char __pyx_k_hour[] = "hour";
 static const char __pyx_k_init[] = "__init__";
 static const char __pyx_k_join[] = "join";
 static const char __pyx_k_lock[] = "lock";
 static const char __pyx_k_main[] = "__main__";
@@ -2428,14 +2400,15 @@
 static const char __pyx_k_sapnwrfc_ini[] = "sapnwrfc.ini";
 static const char __pyx_k_sending_date[] = "sending_date";
 static const char __pyx_k_sending_time[] = "sending_time";
 static const char __pyx_k_server_log_2[] = "server_log";
 static const char __pyx_k_staticmethod[] = "staticmethod";
 static const char __pyx_k_stringsource[] = "stringsource";
 static const char __pyx_k_unit_history[] = "unit_history";
+static const char __pyx_k_when_filling[] = " when filling ";
 static const char __pyx_k_RFCTYPE_DTDAY[] = "RFCTYPE_DTDAY";
 static const char __pyx_k_RFCTYPE_FLOAT[] = "RFCTYPE_FLOAT";
 static const char __pyx_k_RFCTYPE_TABLE[] = "RFCTYPE_TABLE";
 static const char __pyx_k_RFC_NOT_FOUND[] = "RFC_NOT_FOUND";
 static const char __pyx_k_add_parameter[] = "add_parameter";
 static const char __pyx_k_bgRfcFunction[] = "__bgRfcFunction";
 static const char __pyx_k_client_params[] = "client_params";
@@ -2446,14 +2419,15 @@
 static const char __pyx_k_not_requested[] = "not_requested";
 static const char __pyx_k_numberOfCalls[] = "numberOfCalls";
 static const char __pyx_k_peakBusyCount[] = "peakBusyCount";
 static const char __pyx_k_receivedBytes[] = "receivedBytes";
 static const char __pyx_k_reduce_cython[] = "__reduce_cython__";
 static const char __pyx_k_server_params[] = "server_params";
 static const char __pyx_k_transactional[] = "transactional";
+static const char __pyx_k_when_wrapping[] = " when wrapping ";
 static const char __pyx_k_RFCTYPE_DECF16[] = "RFCTYPE_DECF16";
 static const char __pyx_k_RFCTYPE_DECF34[] = "RFCTYPE_DECF34";
 static const char __pyx_k_RFCTYPE_DTWEEK[] = "RFCTYPE_DTWEEK";
 static const char __pyx_k_RFCTYPE_STRING[] = "RFCTYPE_STRING";
 static const char __pyx_k_genericHandler[] = "genericHandler";
 static const char __pyx_k_get_unit_state[] = "_get_unit_state";
 static const char __pyx_k_metadataLookup[] = "metadataLookup";
@@ -2471,24 +2445,24 @@
 static const char __pyx_k_TypeDescription[] = "<TypeDescription '";
 static const char __pyx_k_applicationTime[] = "applicationTime";
 static const char __pyx_k_background_unit[] = "background_unit";
 static const char __pyx_k_bgRfcFunction_2[] = "bgRfcFunction";
 static const char __pyx_k_collections_abc[] = "collections.abc";
 static const char __pyx_k_is_not_callable[] = "' is not callable: '";
 static const char __pyx_k_no_commit_check[] = "no_commit_check";
-static const char __pyx_k_or_confirm_unit[] = "or confirm_unit().";
 static const char __pyx_k_partnerCodepage[] = "partnerCodepage";
 static const char __pyx_k_reload_ini_file[] = "reload_ini_file";
 static const char __pyx_k_request_context[] = "request_context";
 static const char __pyx_k_setOnConnection[] = "setOnConnection";
 static const char __pyx_k_setstate_cython[] = "__setstate_cython__";
 static const char __pyx_k_unit_attributes[] = "unit_attributes";
 static const char __pyx_k_unit_identifier[] = "unit_identifier";
 static const char __pyx_k_ABAPRuntimeError[] = "ABAPRuntimeError";
 static const char __pyx_k_ServerConnection[] = "ServerConnection";
+static const char __pyx_k_Unknown_RFC_type[] = "Unknown RFC type ";
 static const char __pyx_k_currentBusyCount[] = "currentBusyCount";
 static const char __pyx_k_direction_string[] = "'direction' (string) '";
 static const char __pyx_k_func_desc_handle[] = "func_desc_handle";
 static const char __pyx_k_is_not_supported[] = "' is not supported";
 static const char __pyx_k_server_functions[] = "server_functions";
 static const char __pyx_k_set_locale_radix[] = "set_locale_radix";
 static const char __pyx_k_type_description[] = "type_description";
@@ -2585,15 +2559,14 @@
 static const char __pyx_k_BgRfc_callback_function_key_not[] = "BgRfc callback function key not supported: '";
 static const char __pyx_k_Callback_functions_may_only_rai[] = "\nCallback functions may only raise ABAPApplicationError, ABAPRuntimeError, or ExternalRuntimeError.\nThe values of the request were:\nparams: ";
 static const char __pyx_k_Connection_configuration_option[] = "Connection configuration option '";
 static const char __pyx_k_Error_in_bgRFC_handler_onCommit[] = "Error in bgRFC handler onCommit:";
 static const char __pyx_k_Error_while_retrieving_connecti[] = "': Error while retrieving connection attributes (rc=";
 static const char __pyx_k_Parameter_calls_must_contain_at[] = "Parameter 'calls' must contain at least on call description (func_name, params).";
 static const char __pyx_k_Parameter_unit_not_valid_Please[] = "Parameter 'unit' not valid. Please use initialize_unit() to retrieve a valid unit.";
-static const char __pyx_k_Unknown_RFC_type_d_when_filling[] = "Unknown RFC type %d when filling %s";
 static const char __pyx_k_bgRFC_handler_onGetState_is_not[] = "bgRFC handler onGetState is not registered for server connection handle '{<uintptr_t>rfcHandle}'";
 static const char __pyx_k_code_set_to_RFC_EXTERNAL_FAILUR[] = " - code set to RFC_EXTERNAL_FAILURE.";
 static const char __pyx_k_invocation_rejected_because_the[] = "' invocation rejected because the connection is closed";
 static const char __pyx_k_parameter_text_string_parameter[] = "'parameter_text' (string) '{parameter_text}' must not exceed 79 chars.";
 static const char __pyx_k_raises_an_invalid_exception_Exc[] = "' raises an invalid exception:\n Exception: ";
 static const char __pyx_k_self__handle_self__tHandle_self[] = "self._handle,self._tHandle,self._uHandle cannot be converted to a Python object for pickling";
 static const char __pyx_k_when_getting_server_context_for[] = " when getting server context for connection '";
@@ -2610,92 +2583,91 @@
 static const char __pyx_k_Length_of_parameter_unit_id_must[] = "Length of parameter 'unit['id']' must be ";
 static const char __pyx_k_No_state_check_possible_of_non_b[] = "No state check possible of non-bgRFC units.";
 static const char __pyx_k_No_transaction_handle_for_this_c[] = "No transaction handle for this connection available.";
 static const char __pyx_k_No_unit_handle_for_this_connecti[] = "No unit handle for this connection available.";
 static const char __pyx_k_Parameter_calls_must_be_iterable[] = "Parameter 'calls' must be iterable.";
 static const char __pyx_k_Parameter_calls_must_contain_val[] = "Parameter 'calls' must contain valid call descriptions (func_name, params dict).";
 static const char __pyx_k_Remote_function_module_name_must[] = "Remote function module name must be unicode string, received:";
-static const char __pyx_k_There_is_an_active_unit_for_this[] = "There is an active unit for this connection. Use destroy_unit() ";
-static const char __pyx_k_Unknown_RFC_type_d_when_wrapping[] = "Unknown RFC type %d when wrapping %s";
+static const char __pyx_k_There_is_an_active_unit_for_this[] = "There is an active unit for this connection. Use destroy_unit() or confirm_unit().";
 static const char __pyx_k_User_user_from_system_sysId_clie[] = "User '{user}' from system '{sysId}' client '{client}' host '{partnerHost}' invokes '{func_name}'";
 static const char __pyx_k_a_decimal_value_required_receive[] = "a decimal value required, received";
 static const char __pyx_k_a_numeric_string_is_required_rec[] = "a numeric string is required, received";
 static const char __pyx_k_dictionary_required_for_structur[] = "dictionary required for structure parameter, received";
 static const char __pyx_k_list_required_for_table_paramete[] = "list required for table parameter, received";
 static const char __pyx_k_no_default___reduce___due_to_non[] = "no default __reduce__ due to non-trivial __cinit__";
 static const char __pyx_k_sapnwrfc_ini_path_is_not_a_strin[] = "sapnwrfc.ini path is not a string:";
 static const char __pyx_k_self__handle_cannot_be_converted[] = "self._handle cannot be converted to a Python object for pickling";
 static const char __pyx_k_self__throughput_handle_cannot_b[] = "self._throughput_handle cannot be converted to a Python object for pickling";
-static PyObject *__pyx_kp_s_00000000;
+static PyObject *__pyx_kp_u_00000000;
 static PyObject *__pyx_kp_u_02;
 static PyObject *__pyx_kp_u_04;
 static PyObject *__pyx_n_s_ABAPApplicationError;
 static PyObject *__pyx_n_s_ABAPRuntimeError;
 static PyObject *__pyx_kp_s_A_function_description_This_cla;
 static PyObject *__pyx_kp_s_A_type_description_This_class_w;
-static PyObject *__pyx_kp_s_Argument_attributes_not_valid_t;
-static PyObject *__pyx_kp_s_Argument_background_must_be_a_bo;
-static PyObject *__pyx_kp_s_Argument_queue_names_not_valid_t;
-static PyObject *__pyx_kp_s_Argument_unit_not_valid_Is_unit;
+static PyObject *__pyx_kp_u_Argument_attributes_not_valid_t;
+static PyObject *__pyx_kp_u_Argument_background_must_be_a_bo;
+static PyObject *__pyx_kp_u_Argument_queue_names_not_valid_t;
+static PyObject *__pyx_kp_u_Argument_unit_not_valid_Is_unit;
 static PyObject *__pyx_kp_u_Authentication_exception_raised;
 static PyObject *__pyx_kp_u_BgRfc_callback_function_key_not;
 static PyObject *__pyx_kp_u_BgRfc_callback_function_referenc;
 static PyObject *__pyx_kp_u_Callback_functions_may_only_rai;
 static PyObject *__pyx_n_s_CommunicationError;
 static PyObject *__pyx_n_s_Connection;
 static PyObject *__pyx_n_s_ConnectionParameters;
 static PyObject *__pyx_kp_u_Connection_configuration_option;
-static PyObject *__pyx_kp_s_Connection_object_required_recei;
-static PyObject *__pyx_kp_s_Connection_parameters_missing;
+static PyObject *__pyx_kp_u_Connection_object_required_recei;
+static PyObject *__pyx_kp_u_Connection_parameters_missing;
 static PyObject *__pyx_kp_u_Connection_was_canceled;
-static PyObject *__pyx_kp_s_Crypto_library_not_found;
+static PyObject *__pyx_kp_u_Crypto_library_not_found;
 static PyObject *__pyx_n_s_Decimal;
 static PyObject *__pyx_n_s_Enum;
 static PyObject *__pyx_kp_u_Error_code;
-static PyObject *__pyx_kp_s_Error_in_bgRFC_handler_onCheck;
-static PyObject *__pyx_kp_s_Error_in_bgRFC_handler_onCommit;
-static PyObject *__pyx_kp_s_Error_in_bgRFC_handler_onConfirm;
-static PyObject *__pyx_kp_s_Error_in_bgRFC_handler_onGetStat;
-static PyObject *__pyx_kp_s_Error_in_bgRFC_handler_onRollbac;
+static PyObject *__pyx_kp_u_Error_in_bgRFC_handler_onCheck;
+static PyObject *__pyx_kp_u_Error_in_bgRFC_handler_onCommit;
+static PyObject *__pyx_kp_u_Error_in_bgRFC_handler_onConfirm;
+static PyObject *__pyx_kp_u_Error_in_bgRFC_handler_onGetStat;
+static PyObject *__pyx_kp_u_Error_in_bgRFC_handler_onRollbac;
 static PyObject *__pyx_kp_u_Error_while_retrieving_connecti;
 static PyObject *__pyx_n_s_ExternalApplicationError;
 static PyObject *__pyx_n_s_ExternalAuthorizationError;
 static PyObject *__pyx_n_s_ExternalRuntimeError;
 static PyObject *__pyx_kp_u_Function;
 static PyObject *__pyx_kp_u_FunctionDescription;
 static PyObject *__pyx_n_s_FunctionDescription_2;
 static PyObject *__pyx_n_s_FunctionDescription___init;
 static PyObject *__pyx_n_s_FunctionDescription___repr;
 static PyObject *__pyx_n_s_FunctionDescription_add_paramete;
-static PyObject *__pyx_kp_s_H_M_S;
-static PyObject *__pyx_kp_s_Invalid_connection_handle;
-static PyObject *__pyx_kp_s_Invalid_exception_raised_by_call;
+static PyObject *__pyx_kp_u_H_M_S;
+static PyObject *__pyx_kp_u_Invalid_connection_handle;
+static PyObject *__pyx_kp_u_Invalid_exception_raised_by_call;
 static PyObject *__pyx_kp_u_Invalid_length_of_unit_id_should;
-static PyObject *__pyx_kp_s_Invocation_finished_submitting;
+static PyObject *__pyx_kp_u_Invocation_finished_submitting;
 static PyObject *__pyx_n_s_Iterable;
 static PyObject *__pyx_n_s_LOCALE_RADIX;
 static PyObject *__pyx_kp_u_Length_of_parameter_unit_id_must;
 static PyObject *__pyx_n_s_LogonError;
 static PyObject *__pyx_n_s_MASK_DTIME;
 static PyObject *__pyx_n_s_MASK_RETURN_IMPORT_PARAMS;
 static PyObject *__pyx_n_s_MASK_RSTRIP;
 static PyObject *__pyx_kp_u_New_handle;
-static PyObject *__pyx_kp_s_No_connections_assigned;
+static PyObject *__pyx_kp_u_No_connections_assigned;
 static PyObject *__pyx_kp_u_No_metadata_found_for_function;
-static PyObject *__pyx_kp_s_No_state_check_possible_of_non_b;
-static PyObject *__pyx_kp_s_No_transaction_handle_for_this_c;
-static PyObject *__pyx_kp_s_No_unit_handle_for_this_connecti;
-static PyObject *__pyx_kp_s_Not_a_valid_error_group;
+static PyObject *__pyx_kp_u_No_state_check_possible_of_non_b;
+static PyObject *__pyx_kp_u_No_transaction_handle_for_this_c;
+static PyObject *__pyx_kp_u_No_unit_handle_for_this_connecti;
+static PyObject *__pyx_kp_u_Not_a_valid_error_group;
 static PyObject *__pyx_n_s_OK;
-static PyObject *__pyx_kp_s_Parameter_calls_must_be_iterable;
-static PyObject *__pyx_kp_s_Parameter_calls_must_contain_at;
-static PyObject *__pyx_kp_s_Parameter_calls_must_contain_val;
-static PyObject *__pyx_kp_s_Parameter_unit_not_valid_Please;
+static PyObject *__pyx_kp_u_Parameter_calls_must_be_iterable;
+static PyObject *__pyx_kp_u_Parameter_calls_must_contain_at;
+static PyObject *__pyx_kp_u_Parameter_calls_must_contain_val;
+static PyObject *__pyx_kp_u_Parameter_unit_not_valid_Please;
 static PyObject *__pyx_n_s_Pyx_CFunc_object____object___t;
-static PyObject *__pyx_n_s_Q;
+static PyObject *__pyx_n_u_Q;
 static PyObject *__pyx_n_s_RCStatus;
 static PyObject *__pyx_n_s_RFCError;
 static PyObject *__pyx_n_s_RFCTYPE_ABAPOBJECT;
 static PyObject *__pyx_n_s_RFCTYPE_BCD;
 static PyObject *__pyx_n_s_RFCTYPE_BYTE;
 static PyObject *__pyx_n_s_RFCTYPE_CDAY;
 static PyObject *__pyx_n_s_RFCTYPE_CHAR;
@@ -2727,387 +2699,410 @@
 static PyObject *__pyx_n_s_RFC_EXECUTED;
 static PyObject *__pyx_n_s_RFC_EXPORT;
 static PyObject *__pyx_n_s_RFC_EXTERNAL_FAILURE;
 static PyObject *__pyx_n_s_RFC_IMPORT;
 static PyObject *__pyx_n_s_RFC_NOT_FOUND;
 static PyObject *__pyx_n_s_RFC_TABLES;
 static PyObject *__pyx_kp_u_Remote_function_module;
-static PyObject *__pyx_kp_s_Remote_function_module_name_must;
+static PyObject *__pyx_kp_u_Remote_function_module_name_must;
 static PyObject *__pyx_kp_u_Request_for;
 static PyObject *__pyx_n_s_RfcFieldType;
 static PyObject *__pyx_n_s_RfcParameterDirection;
 static PyObject *__pyx_n_s_Server;
+static PyObject *__pyx_n_u_Server;
 static PyObject *__pyx_n_s_ServerConnection;
-static PyObject *__pyx_kp_s_Server_close;
-static PyObject *__pyx_kp_s_Server_connection;
+static PyObject *__pyx_kp_u_Server_close;
+static PyObject *__pyx_kp_u_Server_connection;
 static PyObject *__pyx_kp_u_Server_function;
-static PyObject *__pyx_kp_s_Server_function_installed;
-static PyObject *__pyx_n_s_T;
+static PyObject *__pyx_kp_u_Server_function_installed;
+static PyObject *__pyx_n_u_T;
 static PyObject *__pyx_kp_u_TID;
-static PyObject *__pyx_kp_s_There_is_an_active_unit_for_this;
+static PyObject *__pyx_kp_u_There_is_an_active_unit_for_this;
 static PyObject *__pyx_n_s_Thread;
 static PyObject *__pyx_n_s_Throughput;
 static PyObject *__pyx_n_s_Timer;
 static PyObject *__pyx_kp_u_TypeDescription;
 static PyObject *__pyx_n_s_TypeDescription_2;
 static PyObject *__pyx_n_s_TypeDescription___init;
 static PyObject *__pyx_n_s_TypeDescription___repr;
 static PyObject *__pyx_n_s_TypeDescription_add_field;
 static PyObject *__pyx_n_s_TypeError;
 static PyObject *__pyx_kp_u_UTC;
 static PyObject *__pyx_kp_u_Unit;
 static PyObject *__pyx_n_s_UnitCallType;
 static PyObject *__pyx_n_s_UnitState;
-static PyObject *__pyx_kp_s_Unknown_RFC_type_d_when_filling;
-static PyObject *__pyx_kp_s_Unknown_RFC_type_d_when_wrapping;
-static PyObject *__pyx_kp_s_User_user_from_system_sysId_clie;
+static PyObject *__pyx_kp_u_Unknown_RFC_type;
+static PyObject *__pyx_kp_u_User_user_from_system_sysId_clie;
 static PyObject *__pyx_kp_u_Values;
-static PyObject *__pyx_kp_s_Y_m_d;
-static PyObject *__pyx_kp_s__20;
-static PyObject *__pyx_kp_u__20;
-static PyObject *__pyx_kp_u__23;
+static PyObject *__pyx_kp_u_Y_m_d;
+static PyObject *__pyx_kp_u__21;
 static PyObject *__pyx_kp_u__24;
-static PyObject *__pyx_kp_u__27;
+static PyObject *__pyx_kp_u__25;
 static PyObject *__pyx_kp_u__28;
+static PyObject *__pyx_kp_u__29;
 static PyObject *__pyx_kp_u__3;
 static PyObject *__pyx_kp_u__4;
-static PyObject *__pyx_kp_s__45;
-static PyObject *__pyx_kp_s__5;
-static PyObject *__pyx_n_s__50;
+static PyObject *__pyx_kp_u__46;
+static PyObject *__pyx_kp_u__5;
+static PyObject *__pyx_n_s__51;
 static PyObject *__pyx_kp_u__6;
-static PyObject *__pyx_kp_s_a_decimal_value_required_receive;
-static PyObject *__pyx_kp_s_a_numeric_string_is_required_rec;
-static PyObject *__pyx_n_s_active_unit;
+static PyObject *__pyx_kp_u_a_decimal_value_required_receive;
+static PyObject *__pyx_kp_u_a_numeric_string_is_required_rec;
+static PyObject *__pyx_n_u_active_unit;
 static PyObject *__pyx_n_s_add;
 static PyObject *__pyx_n_s_add_field;
 static PyObject *__pyx_n_s_add_parameter;
 static PyObject *__pyx_n_s_alive;
 static PyObject *__pyx_kp_u_already_installed;
-static PyObject *__pyx_kp_s_an_integer_required_received;
-static PyObject *__pyx_kp_s_an_string_is_required_received;
+static PyObject *__pyx_kp_u_an_integer_required_received;
+static PyObject *__pyx_kp_u_an_string_is_required_received;
 static PyObject *__pyx_n_s_append;
-static PyObject *__pyx_n_s_applicationTime;
+static PyObject *__pyx_n_u_applicationTime;
 static PyObject *__pyx_n_s_args;
 static PyObject *__pyx_n_s_attributes;
-static PyObject *__pyx_n_s_auth_check;
+static PyObject *__pyx_n_u_auth_check;
 static PyObject *__pyx_kp_u_authorization_check_for;
 static PyObject *__pyx_n_s_auto;
 static PyObject *__pyx_n_s_background;
+static PyObject *__pyx_n_u_background;
 static PyObject *__pyx_n_s_background_unit;
-static PyObject *__pyx_kp_s_bgRFC_handler_onGetState_is_not;
+static PyObject *__pyx_kp_u_bgRFC_handler_onGetState_is_not;
 static PyObject *__pyx_n_s_bgRfcFunction;
 static PyObject *__pyx_n_s_bgRfcFunction_2;
 static PyObject *__pyx_kp_u_but_found;
-static PyObject *__pyx_n_s_call_type;
+static PyObject *__pyx_n_u_call_type;
 static PyObject *__pyx_n_s_callback;
+static PyObject *__pyx_n_u_callback;
 static PyObject *__pyx_n_s_calls;
 static PyObject *__pyx_n_s_cancel;
 static PyObject *__pyx_n_s_cancel_connection;
 static PyObject *__pyx_n_s_cfunc_to_py;
 static PyObject *__pyx_kp_u_chars_found;
-static PyObject *__pyx_n_s_check;
+static PyObject *__pyx_n_u_check;
 static PyObject *__pyx_n_s_clear;
-static PyObject *__pyx_n_s_client;
+static PyObject *__pyx_n_u_client;
 static PyObject *__pyx_n_s_client_connection;
 static PyObject *__pyx_n_s_client_params;
 static PyObject *__pyx_n_s_cline_in_traceback;
 static PyObject *__pyx_n_s_close;
 static PyObject *__pyx_n_s_close_2;
 static PyObject *__pyx_n_s_code;
 static PyObject *__pyx_kp_u_code_set_to_RFC_ABAP_EXCEPTION;
 static PyObject *__pyx_kp_u_code_set_to_RFC_ABAP_MESSAGE;
 static PyObject *__pyx_kp_u_code_set_to_RFC_EXTERNAL_FAILUR;
-static PyObject *__pyx_n_s_codepage;
+static PyObject *__pyx_n_u_codepage;
 static PyObject *__pyx_n_s_collections_abc;
-static PyObject *__pyx_n_s_commit;
+static PyObject *__pyx_n_u_commit;
 static PyObject *__pyx_n_s_committed;
 static PyObject *__pyx_n_s_config;
-static PyObject *__pyx_n_s_confirm;
+static PyObject *__pyx_n_u_confirm;
 static PyObject *__pyx_n_s_confirm_transaction;
 static PyObject *__pyx_n_s_confirm_unit;
 static PyObject *__pyx_n_s_confirmed;
 static PyObject *__pyx_n_s_connection;
-static PyObject *__pyx_n_s_connection_attributes;
+static PyObject *__pyx_n_u_connection_attributes;
 static PyObject *__pyx_n_s_connections;
-static PyObject *__pyx_n_s_cpicConvId;
+static PyObject *__pyx_n_u_cpicConvId;
 static PyObject *__pyx_n_s_create_and_submit_transaction;
 static PyObject *__pyx_n_s_create_and_submit_unit;
 static PyObject *__pyx_n_s_created;
-static PyObject *__pyx_n_s_currentBusyCount;
+static PyObject *__pyx_n_u_currentBusyCount;
+static PyObject *__pyx_n_u_d;
 static PyObject *__pyx_n_s_date;
-static PyObject *__pyx_kp_s_date_value_required_received;
+static PyObject *__pyx_kp_u_date_value_required_received;
 static PyObject *__pyx_n_s_datetime;
 static PyObject *__pyx_n_s_day;
 static PyObject *__pyx_n_s_debug;
+static PyObject *__pyx_n_u_debug;
 static PyObject *__pyx_n_s_decimal;
-static PyObject *__pyx_n_s_decimal_point;
+static PyObject *__pyx_n_u_decimal_point;
 static PyObject *__pyx_n_s_decimals;
+static PyObject *__pyx_n_u_decimals;
 static PyObject *__pyx_n_s_decode;
 static PyObject *__pyx_n_s_default_auth_check;
 static PyObject *__pyx_n_s_default_value;
+static PyObject *__pyx_n_u_default_value;
 static PyObject *__pyx_kp_u_default_value_string;
 static PyObject *__pyx_n_s_del;
-static PyObject *__pyx_n_s_deserializationTime;
-static PyObject *__pyx_n_s_dest;
+static PyObject *__pyx_n_u_deserializationTime;
+static PyObject *__pyx_n_u_dest;
 static PyObject *__pyx_n_s_destroy;
 static PyObject *__pyx_n_s_destroy_transaction;
 static PyObject *__pyx_n_s_destroy_unit;
-static PyObject *__pyx_kp_s_dictionary_required_for_structur;
+static PyObject *__pyx_kp_u_dictionary_required_for_structur;
 static PyObject *__pyx_n_s_direction;
+static PyObject *__pyx_n_u_direction;
 static PyObject *__pyx_kp_u_direction_string;
 static PyObject *__pyx_n_s_doc;
-static PyObject *__pyx_n_s_dtime;
+static PyObject *__pyx_n_u_dtime;
 static PyObject *__pyx_n_s_encode;
-static PyObject *__pyx_n_s_end;
 static PyObject *__pyx_n_s_enum;
 static PyObject *__pyx_n_s_enum_names;
 static PyObject *__pyx_n_s_enum_values;
 static PyObject *__pyx_n_s_enumerate;
 static PyObject *__pyx_n_s_errorInfo;
 static PyObject *__pyx_n_s_exc_info;
 static PyObject *__pyx_n_s_exception;
 static PyObject *__pyx_n_s_executed;
 static PyObject *__pyx_kp_u_field;
 static PyObject *__pyx_kp_u_field_name_string;
 static PyObject *__pyx_kp_u_field_name_string_2;
 static PyObject *__pyx_n_s_field_type;
+static PyObject *__pyx_n_u_field_type;
 static PyObject *__pyx_kp_u_field_type_string;
 static PyObject *__pyx_n_s_fields;
 static PyObject *__pyx_kp_u_fields_n_uclength;
-static PyObject *__pyx_n_s_file;
 static PyObject *__pyx_n_s_format;
 static PyObject *__pyx_n_s_free;
-static PyObject *__pyx_n_s_func_desc_handle;
+static PyObject *__pyx_n_u_func_desc_handle;
 static PyObject *__pyx_n_s_func_name;
 static PyObject *__pyx_n_s_function_name;
-static PyObject *__pyx_n_s_genericHandler;
+static PyObject *__pyx_n_u_genericHandler;
 static PyObject *__pyx_n_s_get;
 static PyObject *__pyx_n_s_getFromConnection;
-static PyObject *__pyx_n_s_getState;
+static PyObject *__pyx_n_u_getState;
 static PyObject *__pyx_n_s_get_nwrfclib_version;
 static PyObject *__pyx_n_s_get_transaction_id;
 static PyObject *__pyx_n_s_get_unit_id;
 static PyObject *__pyx_n_s_get_unit_state;
 static PyObject *__pyx_n_s_gethostname;
 static PyObject *__pyx_n_s_getstate;
 static PyObject *__pyx_n_s_handle;
 static PyObject *__pyx_kp_u_handle_2;
 static PyObject *__pyx_n_s_handle_3;
 static PyObject *__pyx_kp_u_has_invalid_state;
-static PyObject *__pyx_n_s_host;
-static PyObject *__pyx_n_s_hostname;
+static PyObject *__pyx_n_u_host;
+static PyObject *__pyx_n_u_hostname;
 static PyObject *__pyx_n_s_hour;
-static PyObject *__pyx_n_s_id;
+static PyObject *__pyx_n_u_id;
 static PyObject *__pyx_n_s_idunitStateentifier;
 static PyObject *__pyx_n_s_import;
 static PyObject *__pyx_n_s_in_process;
 static PyObject *__pyx_n_s_init;
 static PyObject *__pyx_n_s_install_bgrfc_handlers;
 static PyObject *__pyx_n_s_int_field;
 static PyObject *__pyx_kp_u_invalid_state;
 static PyObject *__pyx_kp_u_invocation_rejected_because_the;
 static PyObject *__pyx_n_s_is_alive;
 static PyObject *__pyx_kp_u_is_not_callable;
 static PyObject *__pyx_kp_u_is_not_supported;
-static PyObject *__pyx_n_s_is_stateful;
+static PyObject *__pyx_n_u_is_stateful;
 static PyObject *__pyx_n_s_is_valid;
 static PyObject *__pyx_n_s_isdigit;
 static PyObject *__pyx_n_s_isfile;
-static PyObject *__pyx_n_s_isoLanguage;
+static PyObject *__pyx_n_u_isoLanguage;
 static PyObject *__pyx_n_s_items;
 static PyObject *__pyx_n_s_iteritems;
 static PyObject *__pyx_n_s_join;
-static PyObject *__pyx_n_s_kernelRel;
-static PyObject *__pyx_n_s_kernel_trace;
+static PyObject *__pyx_n_u_kernelRel;
+static PyObject *__pyx_n_u_kernel_trace;
 static PyObject *__pyx_n_s_key;
 static PyObject *__pyx_n_s_lang_iso;
 static PyObject *__pyx_n_s_lang_sap;
-static PyObject *__pyx_n_s_language;
+static PyObject *__pyx_n_u_language;
 static PyObject *__pyx_n_s_language_iso_to_sap;
 static PyObject *__pyx_n_s_language_sap_to_iso;
 static PyObject *__pyx_kp_u_launched;
 static PyObject *__pyx_kp_u_length;
-static PyObject *__pyx_kp_s_list_required_for_table_paramete;
+static PyObject *__pyx_kp_u_list_required_for_table_paramete;
 static PyObject *__pyx_n_s_locale;
 static PyObject *__pyx_n_s_localeconv;
-static PyObject *__pyx_n_s_lock;
+static PyObject *__pyx_n_u_lock;
 static PyObject *__pyx_n_s_log_message;
 static PyObject *__pyx_n_s_main;
 static PyObject *__pyx_n_s_major;
+static PyObject *__pyx_n_u_major;
 static PyObject *__pyx_n_s_message;
 static PyObject *__pyx_n_s_metaclass;
-static PyObject *__pyx_n_s_metadataLookup;
+static PyObject *__pyx_n_u_metadataLookup;
 static PyObject *__pyx_n_s_minor;
+static PyObject *__pyx_n_u_minor;
 static PyObject *__pyx_n_s_minute;
 static PyObject *__pyx_n_s_module;
 static PyObject *__pyx_n_s_month;
 static PyObject *__pyx_n_s_msg_class;
 static PyObject *__pyx_n_s_msg_number;
 static PyObject *__pyx_n_s_msg_type;
 static PyObject *__pyx_n_s_msg_v1;
 static PyObject *__pyx_n_s_msg_v2;
 static PyObject *__pyx_n_s_msg_v3;
 static PyObject *__pyx_n_s_msg_v4;
-static PyObject *__pyx_kp_s_multi_count;
+static PyObject *__pyx_kp_u_multi_count;
 static PyObject *__pyx_kp_u_must_be_in;
 static PyObject *__pyx_kp_u_must_be_in_2;
 static PyObject *__pyx_kp_u_must_be_of_type_integer;
 static PyObject *__pyx_kp_u_must_not_exceed_30_chars;
 static PyObject *__pyx_n_s_name;
+static PyObject *__pyx_n_u_name;
 static PyObject *__pyx_n_s_name_2;
-static PyObject *__pyx_n_s_no_commit_check;
+static PyObject *__pyx_n_u_no_commit_check;
 static PyObject *__pyx_kp_s_no_default___reduce___due_to_non;
 static PyObject *__pyx_n_s_not_found;
-static PyObject *__pyx_n_s_not_requested;
+static PyObject *__pyx_n_u_not_requested;
 static PyObject *__pyx_n_s_nuc_length;
+static PyObject *__pyx_n_u_nuc_length;
 static PyObject *__pyx_n_s_nuc_offset;
-static PyObject *__pyx_n_s_numberOfCalls;
+static PyObject *__pyx_n_u_nuc_offset;
+static PyObject *__pyx_n_u_numberOfCalls;
 static PyObject *__pyx_n_s_object;
-static PyObject *__pyx_kp_s_of_type;
+static PyObject *__pyx_kp_u_of_type;
 static PyObject *__pyx_n_s_open;
 static PyObject *__pyx_n_s_optional;
+static PyObject *__pyx_n_u_optional;
 static PyObject *__pyx_n_s_options;
-static PyObject *__pyx_kp_s_or_confirm_unit;
 static PyObject *__pyx_n_s_origin;
 static PyObject *__pyx_n_s_os_path;
 static PyObject *__pyx_n_s_parameter_text;
-static PyObject *__pyx_kp_s_parameter_text_string_parameter;
+static PyObject *__pyx_n_u_parameter_text;
+static PyObject *__pyx_kp_u_parameter_text_string_parameter;
 static PyObject *__pyx_n_s_parameter_type;
+static PyObject *__pyx_n_u_parameter_type;
 static PyObject *__pyx_kp_u_parameter_type_string;
 static PyObject *__pyx_n_s_parameters;
 static PyObject *__pyx_kp_u_params;
-static PyObject *__pyx_n_s_partnerBytesPerChar;
-static PyObject *__pyx_n_s_partnerCodepage;
-static PyObject *__pyx_n_s_partnerHost;
-static PyObject *__pyx_n_s_partnerIP;
-static PyObject *__pyx_n_s_partnerIPv6;
-static PyObject *__pyx_n_s_partnerRel;
-static PyObject *__pyx_n_s_partnerSystemCodepage;
-static PyObject *__pyx_n_s_partnerType;
-static PyObject *__pyx_n_s_patchLevel;
+static PyObject *__pyx_n_u_partnerBytesPerChar;
+static PyObject *__pyx_n_u_partnerCodepage;
+static PyObject *__pyx_n_u_partnerHost;
+static PyObject *__pyx_n_u_partnerIP;
+static PyObject *__pyx_n_u_partnerIPv6;
+static PyObject *__pyx_n_u_partnerRel;
+static PyObject *__pyx_n_u_partnerSystemCodepage;
+static PyObject *__pyx_n_u_partnerType;
+static PyObject *__pyx_n_u_patchLevel;
 static PyObject *__pyx_n_s_patchlevel;
 static PyObject *__pyx_n_s_pathName;
 static PyObject *__pyx_n_s_path_name;
-static PyObject *__pyx_n_s_peakBusyCount;
+static PyObject *__pyx_n_u_peakBusyCount;
 static PyObject *__pyx_n_s_platform;
-static PyObject *__pyx_n_s_port;
+static PyObject *__pyx_n_u_platform;
+static PyObject *__pyx_n_u_port;
 static PyObject *__pyx_n_s_prepare;
 static PyObject *__pyx_n_s_print;
-static PyObject *__pyx_n_s_progName;
-static PyObject *__pyx_n_s_program;
-static PyObject *__pyx_n_s_protocolType;
+static PyObject *__pyx_n_u_progName;
+static PyObject *__pyx_n_u_program;
+static PyObject *__pyx_n_u_protocolType;
 static PyObject *__pyx_n_s_pyrfc__cyrfc;
 static PyObject *__pyx_n_s_pyx_vtable;
 static PyObject *__pyx_n_s_qualname;
 static PyObject *__pyx_n_s_queue_name;
 static PyObject *__pyx_n_s_queue_names;
 static PyObject *__pyx_n_s_queued;
+static PyObject *__pyx_n_u_queued;
 static PyObject *__pyx_kp_u_raises_ABAPApplicationError;
 static PyObject *__pyx_kp_u_raises_ABAPRuntimeError;
 static PyObject *__pyx_kp_u_raises_ExternalRuntimeError;
 static PyObject *__pyx_kp_u_raises_an_invalid_exception_Exc;
 static PyObject *__pyx_n_s_range;
 static PyObject *__pyx_n_s_rc;
-static PyObject *__pyx_n_s_receivedBytes;
+static PyObject *__pyx_n_u_receivedBytes;
 static PyObject *__pyx_n_s_reduce;
 static PyObject *__pyx_n_s_reduce_cython;
 static PyObject *__pyx_n_s_reduce_ex;
-static PyObject *__pyx_n_s_registrationCount;
+static PyObject *__pyx_n_u_registrationCount;
 static PyObject *__pyx_n_s_registry;
-static PyObject *__pyx_n_s_rel;
+static PyObject *__pyx_n_u_rel;
 static PyObject *__pyx_n_s_reload_ini_file;
 static PyObject *__pyx_n_s_remove;
 static PyObject *__pyx_n_s_repr;
 static PyObject *__pyx_n_s_request_context;
 static PyObject *__pyx_kp_u_request_context_2;
-static PyObject *__pyx_n_s_reserved;
-static PyObject *__pyx_n_s_return_import_params;
-static PyObject *__pyx_n_s_rfcRole;
-static PyObject *__pyx_n_s_rollback;
+static PyObject *__pyx_n_u_reserved;
+static PyObject *__pyx_n_u_return_import_params;
+static PyObject *__pyx_n_u_rfcRole;
+static PyObject *__pyx_n_u_rollback;
 static PyObject *__pyx_n_s_rolled_back;
 static PyObject *__pyx_n_s_rsplit;
 static PyObject *__pyx_n_s_rstrip;
-static PyObject *__pyx_kp_s_sapnwrfc_ini;
-static PyObject *__pyx_kp_s_sapnwrfc_ini_not_found_in;
-static PyObject *__pyx_kp_s_sapnwrfc_ini_path_is_not_a_strin;
-static PyObject *__pyx_n_s_sat_trace;
+static PyObject *__pyx_n_u_rstrip;
+static PyObject *__pyx_kp_u_sapnwrfc_ini;
+static PyObject *__pyx_kp_u_sapnwrfc_ini_not_found_in;
+static PyObject *__pyx_kp_u_sapnwrfc_ini_path_is_not_a_strin;
+static PyObject *__pyx_n_u_sat_trace;
 static PyObject *__pyx_n_s_second;
 static PyObject *__pyx_n_s_self;
 static PyObject *__pyx_kp_s_self__handle_cannot_be_converted;
 static PyObject *__pyx_kp_s_self__handle_self__tHandle_self;
 static PyObject *__pyx_kp_s_self__throughput_handle_cannot_b;
-static PyObject *__pyx_n_s_sending_date;
-static PyObject *__pyx_n_s_sending_time;
-static PyObject *__pyx_n_s_sentBytes;
-static PyObject *__pyx_n_s_serializationTime;
+static PyObject *__pyx_n_u_sending_date;
+static PyObject *__pyx_n_u_sending_time;
+static PyObject *__pyx_n_u_sentBytes;
+static PyObject *__pyx_n_u_serializationTime;
 static PyObject *__pyx_n_s_serve;
-static PyObject *__pyx_n_s_server;
-static PyObject *__pyx_n_s_serverName;
+static PyObject *__pyx_n_u_server;
+static PyObject *__pyx_n_u_serverName;
 static PyObject *__pyx_n_s_server_context;
+static PyObject *__pyx_n_u_server_context;
 static PyObject *__pyx_n_s_server_functions;
 static PyObject *__pyx_n_s_server_log;
-static PyObject *__pyx_n_s_server_log_2;
+static PyObject *__pyx_n_u_server_log_2;
 static PyObject *__pyx_n_s_server_params;
 static PyObject *__pyx_n_s_setOnConnection;
 static PyObject *__pyx_n_s_set_cryptolib_path;
 static PyObject *__pyx_n_s_set_ini_file_directory;
 static PyObject *__pyx_n_s_set_locale_radix;
 static PyObject *__pyx_n_s_setstate;
 static PyObject *__pyx_n_s_setstate_cython;
 static PyObject *__pyx_kp_u_should_be_from_1_30_chars;
 static PyObject *__pyx_kp_u_should_be_from_1_30_chars_2;
 static PyObject *__pyx_n_s_socket;
 static PyObject *__pyx_kp_s_src_pyrfc__cyrfc_pyx;
 static PyObject *__pyx_n_s_start;
-static PyObject *__pyx_n_s_state;
+static PyObject *__pyx_n_u_state;
 static PyObject *__pyx_n_s_staticmethod;
 static PyObject *__pyx_n_s_stop;
 static PyObject *__pyx_kp_s_stringsource;
 static PyObject *__pyx_n_s_strptime;
 static PyObject *__pyx_n_s_synchronous;
 static PyObject *__pyx_n_s_sys;
 static PyObject *__pyx_n_s_sysId;
-static PyObject *__pyx_n_s_sysNumber;
+static PyObject *__pyx_n_u_sysId;
+static PyObject *__pyx_n_u_sysNumber;
 static PyObject *__pyx_n_s_sysid;
 static PyObject *__pyx_n_s_t;
-static PyObject *__pyx_n_s_t_code;
+static PyObject *__pyx_n_u_t_code;
 static PyObject *__pyx_n_s_target;
 static PyObject *__pyx_n_s_test;
 static PyObject *__pyx_n_s_threading;
 static PyObject *__pyx_n_s_throughput;
 static PyObject *__pyx_n_s_time;
-static PyObject *__pyx_kp_s_time_value_required_received;
-static PyObject *__pyx_n_s_timeout;
-static PyObject *__pyx_n_s_totalTime;
-static PyObject *__pyx_n_s_trace;
+static PyObject *__pyx_kp_u_time_value_required_received;
+static PyObject *__pyx_n_u_timeout;
+static PyObject *__pyx_n_u_totalTime;
+static PyObject *__pyx_n_u_trace;
 static PyObject *__pyx_n_s_traceback;
 static PyObject *__pyx_n_s_transaction_id;
 static PyObject *__pyx_n_s_transactional;
 static PyObject *__pyx_n_s_type;
+static PyObject *__pyx_n_u_type;
 static PyObject *__pyx_n_s_type_description;
+static PyObject *__pyx_n_u_type_description;
 static PyObject *__pyx_n_s_type_name;
 static PyObject *__pyx_n_s_uc_length;
+static PyObject *__pyx_n_u_uc_length;
 static PyObject *__pyx_n_s_uc_offset;
+static PyObject *__pyx_n_u_uc_offset;
 static PyObject *__pyx_n_s_uclang_iso;
 static PyObject *__pyx_n_s_uclang_sap;
 static PyObject *__pyx_n_s_unit;
-static PyObject *__pyx_n_s_unit_attributes;
-static PyObject *__pyx_n_s_unit_history;
+static PyObject *__pyx_n_u_unit_attributes;
+static PyObject *__pyx_n_u_unit_history;
 static PyObject *__pyx_n_s_unit_id;
-static PyObject *__pyx_n_s_unit_identifier;
+static PyObject *__pyx_n_u_unit_identifier;
 static PyObject *__pyx_n_s_update;
 static PyObject *__pyx_n_s_upper;
-static PyObject *__pyx_n_s_user;
+static PyObject *__pyx_n_u_user;
 static PyObject *__pyx_n_s_utcnow;
 static PyObject *__pyx_n_s_utils;
 static PyObject *__pyx_n_s_value;
+static PyObject *__pyx_kp_u_when_filling;
 static PyObject *__pyx_kp_u_when_getting_server_context_for;
+static PyObject *__pyx_kp_u_when_wrapping;
 static PyObject *__pyx_kp_u_with;
 static PyObject *__pyx_n_s_wrap;
-static PyObject *__pyx_kp_s_wrapString_uclen_u_utf8_size_u;
+static PyObject *__pyx_kp_u_wrapString_uclen_u_utf8_size_u;
 static PyObject *__pyx_n_s_year;
 static PyObject *__pyx_pf_5pyrfc_6_cyrfc_get_nwrfclib_version(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_5pyrfc_6_cyrfc_2set_ini_file_directory(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_path_name); /* proto */
 static PyObject *__pyx_pf_5pyrfc_6_cyrfc_4reload_ini_file(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_5pyrfc_6_cyrfc_6language_iso_to_sap(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_lang_iso); /* proto */
 static PyObject *__pyx_pf_5pyrfc_6_cyrfc_8language_sap_to_iso(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_lang_sap); /* proto */
 static PyObject *__pyx_pf_5pyrfc_6_cyrfc_10set_cryptolib_path(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_path_name); /* proto */
@@ -3246,82 +3241,83 @@
 static PyObject *__pyx_tuple__7;
 static PyObject *__pyx_tuple__8;
 static PyObject *__pyx_tuple__9;
 static PyObject *__pyx_slice__12;
 static PyObject *__pyx_slice__13;
 static PyObject *__pyx_slice__14;
 static PyObject *__pyx_slice__15;
-static PyObject *__pyx_slice__29;
-static PyObject *__pyx_slice__37;
+static PyObject *__pyx_slice__30;
 static PyObject *__pyx_slice__38;
 static PyObject *__pyx_slice__39;
 static PyObject *__pyx_slice__40;
 static PyObject *__pyx_slice__41;
 static PyObject *__pyx_slice__42;
 static PyObject *__pyx_slice__43;
 static PyObject *__pyx_slice__44;
-static PyObject *__pyx_slice__46;
+static PyObject *__pyx_slice__45;
 static PyObject *__pyx_slice__47;
+static PyObject *__pyx_slice__48;
 static PyObject *__pyx_tuple__10;
 static PyObject *__pyx_tuple__11;
 static PyObject *__pyx_tuple__16;
 static PyObject *__pyx_tuple__17;
 static PyObject *__pyx_tuple__18;
 static PyObject *__pyx_tuple__19;
-static PyObject *__pyx_tuple__21;
+static PyObject *__pyx_tuple__20;
 static PyObject *__pyx_tuple__22;
-static PyObject *__pyx_tuple__25;
+static PyObject *__pyx_tuple__23;
 static PyObject *__pyx_tuple__26;
-static PyObject *__pyx_tuple__30;
+static PyObject *__pyx_tuple__27;
 static PyObject *__pyx_tuple__31;
 static PyObject *__pyx_tuple__32;
 static PyObject *__pyx_tuple__33;
 static PyObject *__pyx_tuple__34;
 static PyObject *__pyx_tuple__35;
 static PyObject *__pyx_tuple__36;
-static PyObject *__pyx_tuple__48;
-static PyObject *__pyx_tuple__51;
-static PyObject *__pyx_tuple__53;
-static PyObject *__pyx_tuple__55;
-static PyObject *__pyx_tuple__57;
-static PyObject *__pyx_tuple__59;
-static PyObject *__pyx_tuple__61;
-static PyObject *__pyx_tuple__63;
-static PyObject *__pyx_tuple__65;
-static PyObject *__pyx_tuple__67;
+static PyObject *__pyx_tuple__37;
+static PyObject *__pyx_tuple__49;
+static PyObject *__pyx_tuple__52;
+static PyObject *__pyx_tuple__54;
+static PyObject *__pyx_tuple__56;
+static PyObject *__pyx_tuple__58;
+static PyObject *__pyx_tuple__60;
+static PyObject *__pyx_tuple__62;
+static PyObject *__pyx_tuple__64;
+static PyObject *__pyx_tuple__66;
 static PyObject *__pyx_tuple__68;
-static PyObject *__pyx_tuple__70;
-static PyObject *__pyx_tuple__72;
+static PyObject *__pyx_tuple__69;
+static PyObject *__pyx_tuple__71;
 static PyObject *__pyx_tuple__73;
-static PyObject *__pyx_tuple__75;
+static PyObject *__pyx_tuple__74;
 static PyObject *__pyx_tuple__76;
-static PyObject *__pyx_tuple__78;
-static PyObject *__pyx_tuple__80;
+static PyObject *__pyx_tuple__77;
+static PyObject *__pyx_tuple__79;
 static PyObject *__pyx_tuple__81;
-static PyObject *__pyx_tuple__83;
-static PyObject *__pyx_tuple__85;
-static PyObject *__pyx_tuple__87;
-static PyObject *__pyx_codeobj__49;
-static PyObject *__pyx_codeobj__52;
-static PyObject *__pyx_codeobj__54;
-static PyObject *__pyx_codeobj__56;
-static PyObject *__pyx_codeobj__58;
-static PyObject *__pyx_codeobj__60;
-static PyObject *__pyx_codeobj__62;
-static PyObject *__pyx_codeobj__64;
-static PyObject *__pyx_codeobj__66;
-static PyObject *__pyx_codeobj__69;
-static PyObject *__pyx_codeobj__71;
-static PyObject *__pyx_codeobj__74;
-static PyObject *__pyx_codeobj__77;
-static PyObject *__pyx_codeobj__79;
-static PyObject *__pyx_codeobj__82;
-static PyObject *__pyx_codeobj__84;
-static PyObject *__pyx_codeobj__86;
-static PyObject *__pyx_codeobj__88;
+static PyObject *__pyx_tuple__82;
+static PyObject *__pyx_tuple__84;
+static PyObject *__pyx_tuple__86;
+static PyObject *__pyx_tuple__88;
+static PyObject *__pyx_codeobj__50;
+static PyObject *__pyx_codeobj__53;
+static PyObject *__pyx_codeobj__55;
+static PyObject *__pyx_codeobj__57;
+static PyObject *__pyx_codeobj__59;
+static PyObject *__pyx_codeobj__61;
+static PyObject *__pyx_codeobj__63;
+static PyObject *__pyx_codeobj__65;
+static PyObject *__pyx_codeobj__67;
+static PyObject *__pyx_codeobj__70;
+static PyObject *__pyx_codeobj__72;
+static PyObject *__pyx_codeobj__75;
+static PyObject *__pyx_codeobj__78;
+static PyObject *__pyx_codeobj__80;
+static PyObject *__pyx_codeobj__83;
+static PyObject *__pyx_codeobj__85;
+static PyObject *__pyx_codeobj__87;
+static PyObject *__pyx_codeobj__89;
 /* Late includes */
 
 /* "pyrfc/_cyrfc.pyx":112
  * 
  * 
  * def get_nwrfclib_version():             # <<<<<<<<<<<<<<
  *     """Get SAP NW RFC Lib version
@@ -3400,27 +3396,27 @@
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = __Pyx_PyDict_NewPresized(4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 120, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_2 = __Pyx_PyInt_From_unsigned_int(__pyx_v_major); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 120, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_major, __pyx_t_2) < 0) __PYX_ERR(0, 120, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_major, __pyx_t_2) < 0) __PYX_ERR(0, 120, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = __Pyx_PyInt_From_unsigned_int(__pyx_v_minor); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 120, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_minor, __pyx_t_2) < 0) __PYX_ERR(0, 120, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_minor, __pyx_t_2) < 0) __PYX_ERR(0, 120, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = __Pyx_PyInt_From_unsigned_int(__pyx_v_patchlevel); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 120, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_patchLevel, __pyx_t_2) < 0) __PYX_ERR(0, 120, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_patchLevel, __pyx_t_2) < 0) __PYX_ERR(0, 120, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_platform); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 120, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_platform, __pyx_t_2) < 0) __PYX_ERR(0, 120, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_platform, __pyx_t_2) < 0) __PYX_ERR(0, 120, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* "pyrfc/_cyrfc.pyx":112
  * 
@@ -3489,30 +3485,30 @@
   /* "pyrfc/_cyrfc.pyx":131
  *     :return: nothing, raises an error
  *     """
  *     if type(path_name) is not str:             # <<<<<<<<<<<<<<
  *         raise TypeError('sapnwrfc.ini path is not a string:', path_name)
  *     cdef RFC_ERROR_INFO errorInfo
  */
-  __pyx_t_1 = (((PyObject *)Py_TYPE(__pyx_v_path_name)) != ((PyObject *)(&PyString_Type)));
+  __pyx_t_1 = (((PyObject *)Py_TYPE(__pyx_v_path_name)) != ((PyObject *)(&PyUnicode_Type)));
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (unlikely(__pyx_t_2)) {
 
     /* "pyrfc/_cyrfc.pyx":132
  *     """
  *     if type(path_name) is not str:
  *         raise TypeError('sapnwrfc.ini path is not a string:', path_name)             # <<<<<<<<<<<<<<
  *     cdef RFC_ERROR_INFO errorInfo
  *     cdef SAP_UC pathName [512]
  */
     __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 132, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_INCREF(__pyx_kp_s_sapnwrfc_ini_path_is_not_a_strin);
-    __Pyx_GIVEREF(__pyx_kp_s_sapnwrfc_ini_path_is_not_a_strin);
-    PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_kp_s_sapnwrfc_ini_path_is_not_a_strin);
+    __Pyx_INCREF(__pyx_kp_u_sapnwrfc_ini_path_is_not_a_strin);
+    __Pyx_GIVEREF(__pyx_kp_u_sapnwrfc_ini_path_is_not_a_strin);
+    PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_kp_u_sapnwrfc_ini_path_is_not_a_strin);
     __Pyx_INCREF(__pyx_v_path_name);
     __Pyx_GIVEREF(__pyx_v_path_name);
     PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_v_path_name);
     __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_t_3, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 132, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_Raise(__pyx_t_4, 0, 0, 0);
@@ -3549,40 +3545,40 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_6, function);
       __pyx_t_8 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_6)) {
-    PyObject *__pyx_temp[3] = {__pyx_t_7, __pyx_v_path_name, __pyx_kp_s_sapnwrfc_ini};
+    PyObject *__pyx_temp[3] = {__pyx_t_7, __pyx_v_path_name, __pyx_kp_u_sapnwrfc_ini};
     __pyx_t_5 = __Pyx_PyFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 135, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_GOTREF(__pyx_t_5);
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_6)) {
-    PyObject *__pyx_temp[3] = {__pyx_t_7, __pyx_v_path_name, __pyx_kp_s_sapnwrfc_ini};
+    PyObject *__pyx_temp[3] = {__pyx_t_7, __pyx_v_path_name, __pyx_kp_u_sapnwrfc_ini};
     __pyx_t_5 = __Pyx_PyCFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 135, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_GOTREF(__pyx_t_5);
   } else
   #endif
   {
     __pyx_t_9 = PyTuple_New(2+__pyx_t_8); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 135, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
     if (__pyx_t_7) {
       __Pyx_GIVEREF(__pyx_t_7); PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_t_7); __pyx_t_7 = NULL;
     }
     __Pyx_INCREF(__pyx_v_path_name);
     __Pyx_GIVEREF(__pyx_v_path_name);
     PyTuple_SET_ITEM(__pyx_t_9, 0+__pyx_t_8, __pyx_v_path_name);
-    __Pyx_INCREF(__pyx_kp_s_sapnwrfc_ini);
-    __Pyx_GIVEREF(__pyx_kp_s_sapnwrfc_ini);
-    PyTuple_SET_ITEM(__pyx_t_9, 1+__pyx_t_8, __pyx_kp_s_sapnwrfc_ini);
+    __Pyx_INCREF(__pyx_kp_u_sapnwrfc_ini);
+    __Pyx_GIVEREF(__pyx_kp_u_sapnwrfc_ini);
+    PyTuple_SET_ITEM(__pyx_t_9, 1+__pyx_t_8, __pyx_kp_u_sapnwrfc_ini);
     __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_9, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 135, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
   }
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __pyx_t_6 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
@@ -3610,17 +3606,17 @@
  *     if not isfile(join(path_name, "sapnwrfc.ini")):
  *         raise TypeError('sapnwrfc.ini not found in:', path_name)             # <<<<<<<<<<<<<<
  *     pathName = fillString(path_name)
  *     cdef RFC_RC rc = RfcSetIniPath(pathName, &errorInfo)
  */
     __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 136, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_INCREF(__pyx_kp_s_sapnwrfc_ini_not_found_in);
-    __Pyx_GIVEREF(__pyx_kp_s_sapnwrfc_ini_not_found_in);
-    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_kp_s_sapnwrfc_ini_not_found_in);
+    __Pyx_INCREF(__pyx_kp_u_sapnwrfc_ini_not_found_in);
+    __Pyx_GIVEREF(__pyx_kp_u_sapnwrfc_ini_not_found_in);
+    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_kp_u_sapnwrfc_ini_not_found_in);
     __Pyx_INCREF(__pyx_v_path_name);
     __Pyx_GIVEREF(__pyx_v_path_name);
     PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_v_path_name);
     __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_t_4, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 136, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
@@ -4121,30 +4117,30 @@
   /* "pyrfc/_cyrfc.pyx":216
  *     :return: nothing, raises an error
  *     """
  *     if type(path_name) is not str:             # <<<<<<<<<<<<<<
  *         raise TypeError('sapnwrfc.ini path is not a string:', path_name)
  *     cdef RFC_ERROR_INFO errorInfo
  */
-  __pyx_t_1 = (((PyObject *)Py_TYPE(__pyx_v_path_name)) != ((PyObject *)(&PyString_Type)));
+  __pyx_t_1 = (((PyObject *)Py_TYPE(__pyx_v_path_name)) != ((PyObject *)(&PyUnicode_Type)));
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (unlikely(__pyx_t_2)) {
 
     /* "pyrfc/_cyrfc.pyx":217
  *     """
  *     if type(path_name) is not str:
  *         raise TypeError('sapnwrfc.ini path is not a string:', path_name)             # <<<<<<<<<<<<<<
  *     cdef RFC_ERROR_INFO errorInfo
  *     cdef SAP_UC pathName [512]
  */
     __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 217, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_INCREF(__pyx_kp_s_sapnwrfc_ini_path_is_not_a_strin);
-    __Pyx_GIVEREF(__pyx_kp_s_sapnwrfc_ini_path_is_not_a_strin);
-    PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_kp_s_sapnwrfc_ini_path_is_not_a_strin);
+    __Pyx_INCREF(__pyx_kp_u_sapnwrfc_ini_path_is_not_a_strin);
+    __Pyx_GIVEREF(__pyx_kp_u_sapnwrfc_ini_path_is_not_a_strin);
+    PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_kp_u_sapnwrfc_ini_path_is_not_a_strin);
     __Pyx_INCREF(__pyx_v_path_name);
     __Pyx_GIVEREF(__pyx_v_path_name);
     PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_v_path_name);
     __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_t_3, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 217, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_Raise(__pyx_t_4, 0, 0, 0);
@@ -4194,17 +4190,17 @@
  *     if not isfile(path_name):
  *         raise TypeError('Crypto library not found:', path_name)             # <<<<<<<<<<<<<<
  *     pathName = fillString(path_name)
  *     cdef RFC_RC rc = RfcLoadCryptoLibrary(pathName, &errorInfo)
  */
     __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 221, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_INCREF(__pyx_kp_s_Crypto_library_not_found);
-    __Pyx_GIVEREF(__pyx_kp_s_Crypto_library_not_found);
-    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_kp_s_Crypto_library_not_found);
+    __Pyx_INCREF(__pyx_kp_u_Crypto_library_not_found);
+    __Pyx_GIVEREF(__pyx_kp_u_Crypto_library_not_found);
+    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_kp_u_Crypto_library_not_found);
     __Pyx_INCREF(__pyx_v_path_name);
     __Pyx_GIVEREF(__pyx_v_path_name);
     PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_v_path_name);
     __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_t_4, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 221, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
@@ -4408,15 +4404,15 @@
       }
     }
     __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_5) : __Pyx_PyObject_CallNoArg(__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 238, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_4 = __Pyx_PyObject_Dict_GetItem(__pyx_t_3, __pyx_n_s_decimal_point); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 238, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_Dict_GetItem(__pyx_t_3, __pyx_n_u_decimal_point); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 238, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF_SET(__pyx_v_value, __pyx_t_4);
     __pyx_t_4 = 0;
 
     /* "pyrfc/_cyrfc.pyx":237
  *     """
@@ -4779,15 +4775,15 @@
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_4, function);
       }
     }
-    __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_kp_s_Connection_parameters_missing) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_kp_s_Connection_parameters_missing);
+    __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_kp_u_Connection_parameters_missing) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_kp_u_Connection_parameters_missing);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 288, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(0, 288, __pyx_L1_error)
@@ -6088,78 +6084,78 @@
  *         self.fields.append({
  *             'name': name,             # <<<<<<<<<<<<<<
  *             'field_type': field_type,
  *             'nuc_length': nuc_length,
  */
   __pyx_t_3 = __Pyx_PyDict_NewPresized(8); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 379, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_name, __pyx_v_name) < 0) __PYX_ERR(0, 379, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_name, __pyx_v_name) < 0) __PYX_ERR(0, 379, __pyx_L1_error)
 
   /* "pyrfc/_cyrfc.pyx":380
  *         self.fields.append({
  *             'name': name,
  *             'field_type': field_type,             # <<<<<<<<<<<<<<
  *             'nuc_length': nuc_length,
  *             'nuc_offset': nuc_offset,
  */
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_field_type, __pyx_v_field_type) < 0) __PYX_ERR(0, 379, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_field_type, __pyx_v_field_type) < 0) __PYX_ERR(0, 379, __pyx_L1_error)
 
   /* "pyrfc/_cyrfc.pyx":381
  *             'name': name,
  *             'field_type': field_type,
  *             'nuc_length': nuc_length,             # <<<<<<<<<<<<<<
  *             'nuc_offset': nuc_offset,
  *             'uc_length': uc_length,
  */
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_nuc_length, __pyx_v_nuc_length) < 0) __PYX_ERR(0, 379, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_nuc_length, __pyx_v_nuc_length) < 0) __PYX_ERR(0, 379, __pyx_L1_error)
 
   /* "pyrfc/_cyrfc.pyx":382
  *             'field_type': field_type,
  *             'nuc_length': nuc_length,
  *             'nuc_offset': nuc_offset,             # <<<<<<<<<<<<<<
  *             'uc_length': uc_length,
  *             'uc_offset': uc_offset,
  */
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_nuc_offset, __pyx_v_nuc_offset) < 0) __PYX_ERR(0, 379, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_nuc_offset, __pyx_v_nuc_offset) < 0) __PYX_ERR(0, 379, __pyx_L1_error)
 
   /* "pyrfc/_cyrfc.pyx":383
  *             'nuc_length': nuc_length,
  *             'nuc_offset': nuc_offset,
  *             'uc_length': uc_length,             # <<<<<<<<<<<<<<
  *             'uc_offset': uc_offset,
  *             'decimals': decimals,
  */
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_uc_length, __pyx_v_uc_length) < 0) __PYX_ERR(0, 379, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_uc_length, __pyx_v_uc_length) < 0) __PYX_ERR(0, 379, __pyx_L1_error)
 
   /* "pyrfc/_cyrfc.pyx":384
  *             'nuc_offset': nuc_offset,
  *             'uc_length': uc_length,
  *             'uc_offset': uc_offset,             # <<<<<<<<<<<<<<
  *             'decimals': decimals,
  *             'type_description': type_description
  */
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_uc_offset, __pyx_v_uc_offset) < 0) __PYX_ERR(0, 379, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_uc_offset, __pyx_v_uc_offset) < 0) __PYX_ERR(0, 379, __pyx_L1_error)
 
   /* "pyrfc/_cyrfc.pyx":385
  *             'uc_length': uc_length,
  *             'uc_offset': uc_offset,
  *             'decimals': decimals,             # <<<<<<<<<<<<<<
  *             'type_description': type_description
  *         })
  */
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_decimals, __pyx_v_decimals) < 0) __PYX_ERR(0, 379, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_decimals, __pyx_v_decimals) < 0) __PYX_ERR(0, 379, __pyx_L1_error)
 
   /* "pyrfc/_cyrfc.pyx":386
  *             'uc_offset': uc_offset,
  *             'decimals': decimals,
  *             'type_description': type_description             # <<<<<<<<<<<<<<
  *         })
  * 
  */
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_type_description, __pyx_v_type_description) < 0) __PYX_ERR(0, 379, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_type_description, __pyx_v_type_description) < 0) __PYX_ERR(0, 379, __pyx_L1_error)
 
   /* "pyrfc/_cyrfc.pyx":378
  *             if not isinstance(int_field, (int, long)):
  *                 raise TypeError(f"field '{name}' length '{int_field}' must be of type integer")
  *         self.fields.append({             # <<<<<<<<<<<<<<
  *             'name': name,
  *             'field_type': field_type,
@@ -6500,16 +6496,16 @@
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("add_parameter (wrapper)", 0);
   {
     static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_self,&__pyx_n_s_name,&__pyx_n_s_parameter_type,&__pyx_n_s_direction,&__pyx_n_s_nuc_length,&__pyx_n_s_uc_length,&__pyx_n_s_decimals,&__pyx_n_s_default_value,&__pyx_n_s_parameter_text,&__pyx_n_s_optional,&__pyx_n_s_type_description,0};
     PyObject* values[11] = {0,0,0,0,0,0,0,0,0,0,0};
     values[6] = ((PyObject *)((PyObject *)__pyx_int_0));
-    values[7] = ((PyObject *)((PyObject*)__pyx_kp_s__5));
-    values[8] = ((PyObject *)((PyObject*)__pyx_kp_s__5));
+    values[7] = ((PyObject *)((PyObject*)__pyx_kp_u__5));
+    values[8] = ((PyObject *)((PyObject*)__pyx_kp_u__5));
 
     /* "pyrfc/_cyrfc.pyx":427
  *     def add_parameter(self, name, parameter_type, direction, nuc_length,
  *                       uc_length, decimals=0, default_value="", parameter_text="",
  *                       optional=False, type_description=None):             # <<<<<<<<<<<<<<
  *         """ Adds a parameter to the function description.
  * 
@@ -7072,96 +7068,96 @@
  *         self.parameters.append({
  *             'name': name,             # <<<<<<<<<<<<<<
  *             'parameter_type': parameter_type,
  *             'direction': direction,
  */
   __pyx_t_6 = __Pyx_PyDict_NewPresized(10); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 462, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_name, __pyx_v_name) < 0) __PYX_ERR(0, 462, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_u_name, __pyx_v_name) < 0) __PYX_ERR(0, 462, __pyx_L1_error)
 
   /* "pyrfc/_cyrfc.pyx":463
  *         self.parameters.append({
  *             'name': name,
  *             'parameter_type': parameter_type,             # <<<<<<<<<<<<<<
  *             'direction': direction,
  *             'nuc_length': nuc_length,
  */
-  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_parameter_type, __pyx_v_parameter_type) < 0) __PYX_ERR(0, 462, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_u_parameter_type, __pyx_v_parameter_type) < 0) __PYX_ERR(0, 462, __pyx_L1_error)
 
   /* "pyrfc/_cyrfc.pyx":464
  *             'name': name,
  *             'parameter_type': parameter_type,
  *             'direction': direction,             # <<<<<<<<<<<<<<
  *             'nuc_length': nuc_length,
  *             'uc_length': uc_length,
  */
-  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_direction, __pyx_v_direction) < 0) __PYX_ERR(0, 462, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_u_direction, __pyx_v_direction) < 0) __PYX_ERR(0, 462, __pyx_L1_error)
 
   /* "pyrfc/_cyrfc.pyx":465
  *             'parameter_type': parameter_type,
  *             'direction': direction,
  *             'nuc_length': nuc_length,             # <<<<<<<<<<<<<<
  *             'uc_length': uc_length,
  *             'decimals': decimals,
  */
-  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_nuc_length, __pyx_v_nuc_length) < 0) __PYX_ERR(0, 462, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_u_nuc_length, __pyx_v_nuc_length) < 0) __PYX_ERR(0, 462, __pyx_L1_error)
 
   /* "pyrfc/_cyrfc.pyx":466
  *             'direction': direction,
  *             'nuc_length': nuc_length,
  *             'uc_length': uc_length,             # <<<<<<<<<<<<<<
  *             'decimals': decimals,
  *             'default_value': default_value,
  */
-  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_uc_length, __pyx_v_uc_length) < 0) __PYX_ERR(0, 462, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_u_uc_length, __pyx_v_uc_length) < 0) __PYX_ERR(0, 462, __pyx_L1_error)
 
   /* "pyrfc/_cyrfc.pyx":467
  *             'nuc_length': nuc_length,
  *             'uc_length': uc_length,
  *             'decimals': decimals,             # <<<<<<<<<<<<<<
  *             'default_value': default_value,
  *             'parameter_text': parameter_text,
  */
-  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_decimals, __pyx_v_decimals) < 0) __PYX_ERR(0, 462, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_u_decimals, __pyx_v_decimals) < 0) __PYX_ERR(0, 462, __pyx_L1_error)
 
   /* "pyrfc/_cyrfc.pyx":468
  *             'uc_length': uc_length,
  *             'decimals': decimals,
  *             'default_value': default_value,             # <<<<<<<<<<<<<<
  *             'parameter_text': parameter_text,
  *             'optional': optional,
  */
-  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_default_value, __pyx_v_default_value) < 0) __PYX_ERR(0, 462, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_u_default_value, __pyx_v_default_value) < 0) __PYX_ERR(0, 462, __pyx_L1_error)
 
   /* "pyrfc/_cyrfc.pyx":469
  *             'decimals': decimals,
  *             'default_value': default_value,
  *             'parameter_text': parameter_text,             # <<<<<<<<<<<<<<
  *             'optional': optional,
  *             'type_description': type_description
  */
-  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_parameter_text, __pyx_v_parameter_text) < 0) __PYX_ERR(0, 462, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_u_parameter_text, __pyx_v_parameter_text) < 0) __PYX_ERR(0, 462, __pyx_L1_error)
 
   /* "pyrfc/_cyrfc.pyx":470
  *             'default_value': default_value,
  *             'parameter_text': parameter_text,
  *             'optional': optional,             # <<<<<<<<<<<<<<
  *             'type_description': type_description
  *         })
  */
-  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_optional, __pyx_v_optional) < 0) __PYX_ERR(0, 462, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_u_optional, __pyx_v_optional) < 0) __PYX_ERR(0, 462, __pyx_L1_error)
 
   /* "pyrfc/_cyrfc.pyx":471
  *             'parameter_text': parameter_text,
  *             'optional': optional,
  *             'type_description': type_description             # <<<<<<<<<<<<<<
  *         })
  * 
  */
-  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_type_description, __pyx_v_type_description) < 0) __PYX_ERR(0, 462, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_u_type_description, __pyx_v_type_description) < 0) __PYX_ERR(0, 462, __pyx_L1_error)
 
   /* "pyrfc/_cyrfc.pyx":461
  *         if len(parameter_text)>79:
  *             raise TypeError("'parameter_text' (string) '{parameter_text}' must not exceed 79 chars.")
  *         self.parameters.append({             # <<<<<<<<<<<<<<
  *             'name': name,
  *             'parameter_type': parameter_type,
@@ -7381,27 +7377,27 @@
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = __Pyx_PyDict_NewPresized(4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 562, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_2 = __Pyx_PyInt_From_unsigned_int(__pyx_v_major); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 562, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_major, __pyx_t_2) < 0) __PYX_ERR(0, 562, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_major, __pyx_t_2) < 0) __PYX_ERR(0, 562, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = __Pyx_PyInt_From_unsigned_int(__pyx_v_minor); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 562, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_minor, __pyx_t_2) < 0) __PYX_ERR(0, 562, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_minor, __pyx_t_2) < 0) __PYX_ERR(0, 562, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = __Pyx_PyInt_From_unsigned_int(__pyx_v_patchlevel); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 562, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_patchLevel, __pyx_t_2) < 0) __PYX_ERR(0, 562, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_patchLevel, __pyx_t_2) < 0) __PYX_ERR(0, 562, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_platform); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 562, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_platform, __pyx_t_2) < 0) __PYX_ERR(0, 562, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_platform, __pyx_t_2) < 0) __PYX_ERR(0, 562, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* "pyrfc/_cyrfc.pyx":554
  * 
@@ -7782,33 +7778,33 @@
  *         for k in config:
  *             if k not in['dtime', 'return_import_params', 'rstrip', 'timeout']:             # <<<<<<<<<<<<<<
  *                 raise RFCError(f"Connection configuration option '{k}' is not supported")
  *         self.__config = {}
  */
     __Pyx_INCREF(__pyx_v_k);
     __pyx_t_3 = __pyx_v_k;
-    __pyx_t_6 = (__Pyx_PyString_Equals(__pyx_t_3, __pyx_n_s_dtime, Py_NE)); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 596, __pyx_L1_error)
+    __pyx_t_6 = (__Pyx_PyUnicode_Equals(__pyx_t_3, __pyx_n_u_dtime, Py_NE)); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 596, __pyx_L1_error)
     if (__pyx_t_6) {
     } else {
       __pyx_t_2 = __pyx_t_6;
       goto __pyx_L8_bool_binop_done;
     }
-    __pyx_t_6 = (__Pyx_PyString_Equals(__pyx_t_3, __pyx_n_s_return_import_params, Py_NE)); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 596, __pyx_L1_error)
+    __pyx_t_6 = (__Pyx_PyUnicode_Equals(__pyx_t_3, __pyx_n_u_return_import_params, Py_NE)); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 596, __pyx_L1_error)
     if (__pyx_t_6) {
     } else {
       __pyx_t_2 = __pyx_t_6;
       goto __pyx_L8_bool_binop_done;
     }
-    __pyx_t_6 = (__Pyx_PyString_Equals(__pyx_t_3, __pyx_n_s_rstrip, Py_NE)); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 596, __pyx_L1_error)
+    __pyx_t_6 = (__Pyx_PyUnicode_Equals(__pyx_t_3, __pyx_n_u_rstrip, Py_NE)); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 596, __pyx_L1_error)
     if (__pyx_t_6) {
     } else {
       __pyx_t_2 = __pyx_t_6;
       goto __pyx_L8_bool_binop_done;
     }
-    __pyx_t_6 = (__Pyx_PyString_Equals(__pyx_t_3, __pyx_n_s_timeout, Py_NE)); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 596, __pyx_L1_error)
+    __pyx_t_6 = (__Pyx_PyUnicode_Equals(__pyx_t_3, __pyx_n_u_timeout, Py_NE)); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 596, __pyx_L1_error)
     __pyx_t_2 = __pyx_t_6;
     __pyx_L8_bool_binop_done:;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_6 = (__pyx_t_2 != 0);
     if (unlikely(__pyx_t_6)) {
 
       /* "pyrfc/_cyrfc.pyx":597
@@ -7908,15 +7904,15 @@
   __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 599, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (unlikely(__pyx_v_self->__config == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
     __PYX_ERR(0, 599, __pyx_L1_error)
   }
-  if (unlikely(PyDict_SetItem(__pyx_v_self->__config, __pyx_n_s_dtime, __pyx_t_3) < 0)) __PYX_ERR(0, 599, __pyx_L1_error)
+  if (unlikely(PyDict_SetItem(__pyx_v_self->__config, __pyx_n_u_dtime, __pyx_t_3) < 0)) __PYX_ERR(0, 599, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "pyrfc/_cyrfc.pyx":600
  *         self.__config = {}
  *         self.__config['dtime'] = config.get('dtime', False)
  *         self.__config['return_import_params'] = config.get('return_import_params', False)             # <<<<<<<<<<<<<<
  *         self.__config['rstrip'] = config.get('rstrip', True)
@@ -7927,15 +7923,15 @@
   __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 600, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (unlikely(__pyx_v_self->__config == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
     __PYX_ERR(0, 600, __pyx_L1_error)
   }
-  if (unlikely(PyDict_SetItem(__pyx_v_self->__config, __pyx_n_s_return_import_params, __pyx_t_1) < 0)) __PYX_ERR(0, 600, __pyx_L1_error)
+  if (unlikely(PyDict_SetItem(__pyx_v_self->__config, __pyx_n_u_return_import_params, __pyx_t_1) < 0)) __PYX_ERR(0, 600, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "pyrfc/_cyrfc.pyx":601
  *         self.__config['dtime'] = config.get('dtime', False)
  *         self.__config['return_import_params'] = config.get('return_import_params', False)
  *         self.__config['rstrip'] = config.get('rstrip', True)             # <<<<<<<<<<<<<<
  *         self.__config['timeout'] = config.get('timeout', None)
@@ -7946,15 +7942,15 @@
   __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 601, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (unlikely(__pyx_v_self->__config == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
     __PYX_ERR(0, 601, __pyx_L1_error)
   }
-  if (unlikely(PyDict_SetItem(__pyx_v_self->__config, __pyx_n_s_rstrip, __pyx_t_3) < 0)) __PYX_ERR(0, 601, __pyx_L1_error)
+  if (unlikely(PyDict_SetItem(__pyx_v_self->__config, __pyx_n_u_rstrip, __pyx_t_3) < 0)) __PYX_ERR(0, 601, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "pyrfc/_cyrfc.pyx":602
  *         self.__config['return_import_params'] = config.get('return_import_params', False)
  *         self.__config['rstrip'] = config.get('rstrip', True)
  *         self.__config['timeout'] = config.get('timeout', None)             # <<<<<<<<<<<<<<
  * 
@@ -7965,15 +7961,15 @@
   __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 602, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (unlikely(__pyx_v_self->__config == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
     __PYX_ERR(0, 602, __pyx_L1_error)
   }
-  if (unlikely(PyDict_SetItem(__pyx_v_self->__config, __pyx_n_s_timeout, __pyx_t_1) < 0)) __PYX_ERR(0, 602, __pyx_L1_error)
+  if (unlikely(PyDict_SetItem(__pyx_v_self->__config, __pyx_n_u_timeout, __pyx_t_1) < 0)) __PYX_ERR(0, 602, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "pyrfc/_cyrfc.pyx":605
  * 
  *         # set internal configuration
  *         self.__bconfig = 0             # <<<<<<<<<<<<<<
  *         if self.__config['dtime']:
@@ -7988,15 +7984,15 @@
  *             self.__bconfig |= _MASK_DTIME
  *         if self.__config['return_import_params']:
  */
   if (unlikely(__pyx_v_self->__config == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
     __PYX_ERR(0, 606, __pyx_L1_error)
   }
-  __pyx_t_1 = __Pyx_PyDict_GetItem(__pyx_v_self->__config, __pyx_n_s_dtime); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 606, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_GetItem(__pyx_v_self->__config, __pyx_n_u_dtime); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 606, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 606, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (__pyx_t_6) {
 
     /* "pyrfc/_cyrfc.pyx":607
  *         self.__bconfig = 0
@@ -8033,15 +8029,15 @@
  *             self.__bconfig |= _MASK_RETURN_IMPORT_PARAMS
  *         if self.__config['rstrip']:
  */
   if (unlikely(__pyx_v_self->__config == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
     __PYX_ERR(0, 608, __pyx_L1_error)
   }
-  __pyx_t_7 = __Pyx_PyDict_GetItem(__pyx_v_self->__config, __pyx_n_s_return_import_params); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 608, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyDict_GetItem(__pyx_v_self->__config, __pyx_n_u_return_import_params); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 608, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_7); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 608, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   if (__pyx_t_6) {
 
     /* "pyrfc/_cyrfc.pyx":609
  *             self.__bconfig |= _MASK_DTIME
@@ -8078,15 +8074,15 @@
  *             self.__bconfig |= _MASK_RSTRIP
  * 
  */
   if (unlikely(__pyx_v_self->__config == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
     __PYX_ERR(0, 610, __pyx_L1_error)
   }
-  __pyx_t_1 = __Pyx_PyDict_GetItem(__pyx_v_self->__config, __pyx_n_s_rstrip); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 610, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_GetItem(__pyx_v_self->__config, __pyx_n_u_rstrip); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 610, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 610, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (__pyx_t_6) {
 
     /* "pyrfc/_cyrfc.pyx":611
  *             self.__bconfig |= _MASK_RETURN_IMPORT_PARAMS
@@ -9645,15 +9641,15 @@
       goto __pyx_L5_bool_binop_done;
     }
     __pyx_t_6 = __Pyx_PyBool_FromLong(__pyx_v_self->active_transaction); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 790, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __pyx_t_5 = __pyx_t_6;
     __pyx_t_6 = 0;
     __pyx_L5_bool_binop_done:;
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_active_unit, __pyx_t_5) < 0) __PYX_ERR(0, 790, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_active_unit, __pyx_t_5) < 0) __PYX_ERR(0, 790, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __pyx_t_5 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
         __Pyx_INCREF(__pyx_t_5);
@@ -10101,15 +10097,15 @@
   /* "pyrfc/_cyrfc.pyx":878
  *         cdef RFC_ERROR_INFO openErrorInfo
  *         cdef SAP_UC *cName
  *         if type(func_name) is not str:             # <<<<<<<<<<<<<<
  *             raise RFCError("Remote function module name must be unicode string, received:", func_name, type(func_name))
  *         cdef SAP_UC *funcName = fillString(func_name)
  */
-  __pyx_t_1 = (((PyObject *)Py_TYPE(__pyx_v_func_name)) != ((PyObject *)(&PyString_Type)));
+  __pyx_t_1 = (((PyObject *)Py_TYPE(__pyx_v_func_name)) != ((PyObject *)(&PyUnicode_Type)));
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (unlikely(__pyx_t_2)) {
 
     /* "pyrfc/_cyrfc.pyx":879
  *         cdef SAP_UC *cName
  *         if type(func_name) is not str:
  *             raise RFCError("Remote function module name must be unicode string, received:", func_name, type(func_name))             # <<<<<<<<<<<<<<
@@ -10128,37 +10124,37 @@
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_4, function);
         __pyx_t_6 = 1;
       }
     }
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(__pyx_t_4)) {
-      PyObject *__pyx_temp[4] = {__pyx_t_5, __pyx_kp_s_Remote_function_module_name_must, __pyx_v_func_name, ((PyObject *)Py_TYPE(__pyx_v_func_name))};
+      PyObject *__pyx_temp[4] = {__pyx_t_5, __pyx_kp_u_Remote_function_module_name_must, __pyx_v_func_name, ((PyObject *)Py_TYPE(__pyx_v_func_name))};
       __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_6, 3+__pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 879, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_GOTREF(__pyx_t_3);
     } else
     #endif
     #if CYTHON_FAST_PYCCALL
     if (__Pyx_PyFastCFunction_Check(__pyx_t_4)) {
-      PyObject *__pyx_temp[4] = {__pyx_t_5, __pyx_kp_s_Remote_function_module_name_must, __pyx_v_func_name, ((PyObject *)Py_TYPE(__pyx_v_func_name))};
+      PyObject *__pyx_temp[4] = {__pyx_t_5, __pyx_kp_u_Remote_function_module_name_must, __pyx_v_func_name, ((PyObject *)Py_TYPE(__pyx_v_func_name))};
       __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_6, 3+__pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 879, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_GOTREF(__pyx_t_3);
     } else
     #endif
     {
       __pyx_t_7 = PyTuple_New(3+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 879, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       if (__pyx_t_5) {
         __Pyx_GIVEREF(__pyx_t_5); PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_5); __pyx_t_5 = NULL;
       }
-      __Pyx_INCREF(__pyx_kp_s_Remote_function_module_name_must);
-      __Pyx_GIVEREF(__pyx_kp_s_Remote_function_module_name_must);
-      PyTuple_SET_ITEM(__pyx_t_7, 0+__pyx_t_6, __pyx_kp_s_Remote_function_module_name_must);
+      __Pyx_INCREF(__pyx_kp_u_Remote_function_module_name_must);
+      __Pyx_GIVEREF(__pyx_kp_u_Remote_function_module_name_must);
+      PyTuple_SET_ITEM(__pyx_t_7, 0+__pyx_t_6, __pyx_kp_u_Remote_function_module_name_must);
       __Pyx_INCREF(__pyx_v_func_name);
       __Pyx_GIVEREF(__pyx_v_func_name);
       PyTuple_SET_ITEM(__pyx_t_7, 1+__pyx_t_6, __pyx_v_func_name);
       __Pyx_INCREF(((PyObject *)Py_TYPE(__pyx_v_func_name)));
       __Pyx_GIVEREF(((PyObject *)Py_TYPE(__pyx_v_func_name)));
       PyTuple_SET_ITEM(__pyx_t_7, 2+__pyx_t_6, ((PyObject *)Py_TYPE(__pyx_v_func_name)));
       __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_7, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 879, __pyx_L1_error)
@@ -10390,26 +10386,26 @@
     /* "pyrfc/_cyrfc.pyx":893
  *         options = options or {}
  *         try:  # now we have a function module
  *             if 'not_requested' in options:             # <<<<<<<<<<<<<<
  *                 skip_parameters = options['not_requested']
  *                 if type(skip_parameters) is not list:
  */
-    __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_n_s_not_requested, __pyx_v_options, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 893, __pyx_L10_error)
+    __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_n_u_not_requested, __pyx_v_options, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 893, __pyx_L10_error)
     __pyx_t_1 = (__pyx_t_2 != 0);
     if (__pyx_t_1) {
 
       /* "pyrfc/_cyrfc.pyx":894
  *         try:  # now we have a function module
  *             if 'not_requested' in options:
  *                 skip_parameters = options['not_requested']             # <<<<<<<<<<<<<<
  *                 if type(skip_parameters) is not list:
  *                     skip_parameters = [skip_parameters]
  */
-      __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_v_options, __pyx_n_s_not_requested); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 894, __pyx_L10_error)
+      __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_v_options, __pyx_n_u_not_requested); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 894, __pyx_L10_error)
       __Pyx_GOTREF(__pyx_t_3);
       __pyx_v_skip_parameters = __pyx_t_3;
       __pyx_t_3 = 0;
 
       /* "pyrfc/_cyrfc.pyx":895
  *             if 'not_requested' in options:
  *                 skip_parameters = options['not_requested']
@@ -10590,15 +10586,15 @@
  */
     __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_options, __pyx_n_s_get); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 905, __pyx_L10_error)
     __Pyx_GOTREF(__pyx_t_4);
     if (unlikely(__pyx_v_self->__config == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
       __PYX_ERR(0, 905, __pyx_L10_error)
     }
-    __pyx_t_5 = __Pyx_PyDict_GetItem(__pyx_v_self->__config, __pyx_n_s_timeout); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 905, __pyx_L10_error)
+    __pyx_t_5 = __Pyx_PyDict_GetItem(__pyx_v_self->__config, __pyx_n_u_timeout); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 905, __pyx_L10_error)
     __Pyx_GOTREF(__pyx_t_5);
     __pyx_t_7 = NULL;
     __pyx_t_6 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_7)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
@@ -10606,39 +10602,39 @@
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_4, function);
         __pyx_t_6 = 1;
       }
     }
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(__pyx_t_4)) {
-      PyObject *__pyx_temp[3] = {__pyx_t_7, __pyx_n_s_timeout, __pyx_t_5};
+      PyObject *__pyx_temp[3] = {__pyx_t_7, __pyx_n_u_timeout, __pyx_t_5};
       __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 905, __pyx_L10_error)
       __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     } else
     #endif
     #if CYTHON_FAST_PYCCALL
     if (__Pyx_PyFastCFunction_Check(__pyx_t_4)) {
-      PyObject *__pyx_temp[3] = {__pyx_t_7, __pyx_n_s_timeout, __pyx_t_5};
+      PyObject *__pyx_temp[3] = {__pyx_t_7, __pyx_n_u_timeout, __pyx_t_5};
       __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 905, __pyx_L10_error)
       __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     } else
     #endif
     {
       __pyx_t_12 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 905, __pyx_L10_error)
       __Pyx_GOTREF(__pyx_t_12);
       if (__pyx_t_7) {
         __Pyx_GIVEREF(__pyx_t_7); PyTuple_SET_ITEM(__pyx_t_12, 0, __pyx_t_7); __pyx_t_7 = NULL;
       }
-      __Pyx_INCREF(__pyx_n_s_timeout);
-      __Pyx_GIVEREF(__pyx_n_s_timeout);
-      PyTuple_SET_ITEM(__pyx_t_12, 0+__pyx_t_6, __pyx_n_s_timeout);
+      __Pyx_INCREF(__pyx_n_u_timeout);
+      __Pyx_GIVEREF(__pyx_n_u_timeout);
+      PyTuple_SET_ITEM(__pyx_t_12, 0+__pyx_t_6, __pyx_n_u_timeout);
       __Pyx_GIVEREF(__pyx_t_5);
       PyTuple_SET_ITEM(__pyx_t_12, 1+__pyx_t_6, __pyx_t_5);
       __pyx_t_5 = 0;
       __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_12, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 905, __pyx_L10_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
     }
@@ -12140,14 +12136,15 @@
   char const *__pyx_t_19;
   PyObject *__pyx_t_20 = NULL;
   PyObject *__pyx_t_21 = NULL;
   PyObject *__pyx_t_22 = NULL;
   PyObject *__pyx_t_23 = NULL;
   PyObject *__pyx_t_24 = NULL;
   PyObject *__pyx_t_25 = NULL;
+  char const *__pyx_t_26;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_create_and_submit_transaction", 0);
 
   /* "pyrfc/_cyrfc.pyx":1030
  *         cdef RFC_FUNCTION_HANDLE funcCont
@@ -12787,37 +12784,83 @@
       __Pyx_AddTraceback("pyrfc._cyrfc.Connection._create_and_submit_transaction", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_11, &__pyx_t_10, &__pyx_t_1) < 0) __PYX_ERR(0, 1071, __pyx_L9_except_error)
       __Pyx_GOTREF(__pyx_t_11);
       __Pyx_GOTREF(__pyx_t_10);
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_INCREF(__pyx_t_10);
       __pyx_v_e = __pyx_t_10;
+      /*try:*/ {
 
-      /* "pyrfc/_cyrfc.pyx":1073
+        /* "pyrfc/_cyrfc.pyx":1073
  *         except RFCError as e:
  *             # clean up actions
  *             RfcDestroyTransaction(self._tHandle, NULL)             # <<<<<<<<<<<<<<
  *             raise
  * 
  */
-      (void)(RfcDestroyTransaction(__pyx_v_self->_tHandle, NULL));
+        (void)(RfcDestroyTransaction(__pyx_v_self->_tHandle, NULL));
 
-      /* "pyrfc/_cyrfc.pyx":1074
+        /* "pyrfc/_cyrfc.pyx":1074
  *             # clean up actions
  *             RfcDestroyTransaction(self._tHandle, NULL)
  *             raise             # <<<<<<<<<<<<<<
  * 
  *     def _destroy_transaction(self):
  */
-      __Pyx_GIVEREF(__pyx_t_11);
-      __Pyx_GIVEREF(__pyx_t_10);
-      __Pyx_XGIVEREF(__pyx_t_1);
-      __Pyx_ErrRestoreWithState(__pyx_t_11, __pyx_t_10, __pyx_t_1);
-      __pyx_t_11 = 0; __pyx_t_10 = 0; __pyx_t_1 = 0; 
-      __PYX_ERR(0, 1074, __pyx_L9_except_error)
+        __Pyx_GIVEREF(__pyx_t_11);
+        __Pyx_GIVEREF(__pyx_t_10);
+        __Pyx_XGIVEREF(__pyx_t_1);
+        __Pyx_ErrRestoreWithState(__pyx_t_11, __pyx_t_10, __pyx_t_1);
+        __pyx_t_11 = 0; __pyx_t_10 = 0; __pyx_t_1 = 0; 
+        __PYX_ERR(0, 1074, __pyx_L40_error)
+      }
+
+      /* "pyrfc/_cyrfc.pyx":1071
+ *                 self._error(&errorInfo)
+ * 
+ *         except RFCError as e:             # <<<<<<<<<<<<<<
+ *             # clean up actions
+ *             RfcDestroyTransaction(self._tHandle, NULL)
+ */
+      /*finally:*/ {
+        __pyx_L40_error:;
+        /*exception exit:*/{
+          __Pyx_PyThreadState_declare
+          __Pyx_PyThreadState_assign
+          __pyx_t_25 = 0; __pyx_t_24 = 0; __pyx_t_23 = 0; __pyx_t_22 = 0; __pyx_t_21 = 0; __pyx_t_20 = 0;
+          __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
+          __Pyx_XDECREF(__pyx_t_13); __pyx_t_13 = 0;
+          if (PY_MAJOR_VERSION >= 3) __Pyx_ExceptionSwap(&__pyx_t_22, &__pyx_t_21, &__pyx_t_20);
+          if ((PY_MAJOR_VERSION < 3) || unlikely(__Pyx_GetException(&__pyx_t_25, &__pyx_t_24, &__pyx_t_23) < 0)) __Pyx_ErrFetch(&__pyx_t_25, &__pyx_t_24, &__pyx_t_23);
+          __Pyx_XGOTREF(__pyx_t_25);
+          __Pyx_XGOTREF(__pyx_t_24);
+          __Pyx_XGOTREF(__pyx_t_23);
+          __Pyx_XGOTREF(__pyx_t_22);
+          __Pyx_XGOTREF(__pyx_t_21);
+          __Pyx_XGOTREF(__pyx_t_20);
+          __pyx_t_18 = __pyx_lineno; __pyx_t_17 = __pyx_clineno; __pyx_t_26 = __pyx_filename;
+          {
+            __Pyx_DECREF(__pyx_v_e);
+            __pyx_v_e = NULL;
+          }
+          if (PY_MAJOR_VERSION >= 3) {
+            __Pyx_XGIVEREF(__pyx_t_22);
+            __Pyx_XGIVEREF(__pyx_t_21);
+            __Pyx_XGIVEREF(__pyx_t_20);
+            __Pyx_ExceptionReset(__pyx_t_22, __pyx_t_21, __pyx_t_20);
+          }
+          __Pyx_XGIVEREF(__pyx_t_25);
+          __Pyx_XGIVEREF(__pyx_t_24);
+          __Pyx_XGIVEREF(__pyx_t_23);
+          __Pyx_ErrRestore(__pyx_t_25, __pyx_t_24, __pyx_t_23);
+          __pyx_t_25 = 0; __pyx_t_24 = 0; __pyx_t_23 = 0; __pyx_t_22 = 0; __pyx_t_21 = 0; __pyx_t_20 = 0;
+          __pyx_lineno = __pyx_t_18; __pyx_clineno = __pyx_t_17; __pyx_filename = __pyx_t_26;
+          goto __pyx_L9_except_error;
+        }
+      }
     }
     goto __pyx_L9_except_error;
     __pyx_L9_except_error:;
 
     /* "pyrfc/_cyrfc.pyx":1046
  *         self.active_transaction = True
  * 
@@ -12924,15 +12967,15 @@
       if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_4);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
-    __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_kp_s_No_transaction_handle_for_this_c) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_kp_s_No_transaction_handle_for_this_c);
+    __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_kp_u_No_transaction_handle_for_this_c) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_kp_u_No_transaction_handle_for_this_c);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1080, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __PYX_ERR(0, 1080, __pyx_L1_error)
@@ -13112,15 +13155,15 @@
       if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_4);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
-    __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_kp_s_No_transaction_handle_for_this_c) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_kp_s_No_transaction_handle_for_this_c);
+    __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_kp_u_No_transaction_handle_for_this_c) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_kp_u_No_transaction_handle_for_this_c);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1092, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __PYX_ERR(0, 1092, __pyx_L1_error)
@@ -13573,14 +13616,15 @@
   char const *__pyx_t_21;
   PyObject *__pyx_t_22 = NULL;
   PyObject *__pyx_t_23 = NULL;
   PyObject *__pyx_t_24 = NULL;
   PyObject *__pyx_t_25 = NULL;
   PyObject *__pyx_t_26 = NULL;
   PyObject *__pyx_t_27 = NULL;
+  char const *__pyx_t_28;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_create_and_submit_unit", 0);
   __Pyx_INCREF(__pyx_v_queue_names);
 
   /* "pyrfc/_cyrfc.pyx":1132
@@ -13823,26 +13867,26 @@
     /* "pyrfc/_cyrfc.pyx":1178
  *         #                                In the client case the nwrfclib fills this automatically.
  *         if attributes is not None:
  *             if 'kernel_trace' in attributes:             # <<<<<<<<<<<<<<
  *                 unitAttr.kernelTrace = attributes['kernel_trace']
  *             if 'sat_trace' in attributes:
  */
-    __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_n_s_kernel_trace, __pyx_v_attributes, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 1178, __pyx_L1_error)
+    __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_n_u_kernel_trace, __pyx_v_attributes, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 1178, __pyx_L1_error)
     __pyx_t_3 = (__pyx_t_2 != 0);
     if (__pyx_t_3) {
 
       /* "pyrfc/_cyrfc.pyx":1179
  *         if attributes is not None:
  *             if 'kernel_trace' in attributes:
  *                 unitAttr.kernelTrace = attributes['kernel_trace']             # <<<<<<<<<<<<<<
  *             if 'sat_trace' in attributes:
  *                 unitAttr.satTrace = attributes['sat_trace']
  */
-      __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_attributes, __pyx_n_s_kernel_trace); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1179, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_attributes, __pyx_n_u_kernel_trace); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1179, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __pyx_t_10 = __Pyx_PyInt_As_short(__pyx_t_1); if (unlikely((__pyx_t_10 == (short)-1) && PyErr_Occurred())) __PYX_ERR(0, 1179, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __pyx_v_unitAttr.kernelTrace = __pyx_t_10;
 
       /* "pyrfc/_cyrfc.pyx":1178
  *         #                                In the client case the nwrfclib fills this automatically.
@@ -13856,26 +13900,26 @@
     /* "pyrfc/_cyrfc.pyx":1180
  *             if 'kernel_trace' in attributes:
  *                 unitAttr.kernelTrace = attributes['kernel_trace']
  *             if 'sat_trace' in attributes:             # <<<<<<<<<<<<<<
  *                 unitAttr.satTrace = attributes['sat_trace']
  *             if 'unit_history' in attributes:
  */
-    __pyx_t_3 = (__Pyx_PySequence_ContainsTF(__pyx_n_s_sat_trace, __pyx_v_attributes, Py_EQ)); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 1180, __pyx_L1_error)
+    __pyx_t_3 = (__Pyx_PySequence_ContainsTF(__pyx_n_u_sat_trace, __pyx_v_attributes, Py_EQ)); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 1180, __pyx_L1_error)
     __pyx_t_2 = (__pyx_t_3 != 0);
     if (__pyx_t_2) {
 
       /* "pyrfc/_cyrfc.pyx":1181
  *                 unitAttr.kernelTrace = attributes['kernel_trace']
  *             if 'sat_trace' in attributes:
  *                 unitAttr.satTrace = attributes['sat_trace']             # <<<<<<<<<<<<<<
  *             if 'unit_history' in attributes:
  *                 unitAttr.unitHistory = attributes['unit_history']
  */
-      __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_attributes, __pyx_n_s_sat_trace); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1181, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_attributes, __pyx_n_u_sat_trace); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1181, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __pyx_t_10 = __Pyx_PyInt_As_short(__pyx_t_1); if (unlikely((__pyx_t_10 == (short)-1) && PyErr_Occurred())) __PYX_ERR(0, 1181, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __pyx_v_unitAttr.satTrace = __pyx_t_10;
 
       /* "pyrfc/_cyrfc.pyx":1180
  *             if 'kernel_trace' in attributes:
@@ -13889,26 +13933,26 @@
     /* "pyrfc/_cyrfc.pyx":1182
  *             if 'sat_trace' in attributes:
  *                 unitAttr.satTrace = attributes['sat_trace']
  *             if 'unit_history' in attributes:             # <<<<<<<<<<<<<<
  *                 unitAttr.unitHistory = attributes['unit_history']
  *             if 'lock' in attributes:
  */
-    __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_n_s_unit_history, __pyx_v_attributes, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 1182, __pyx_L1_error)
+    __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_n_u_unit_history, __pyx_v_attributes, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 1182, __pyx_L1_error)
     __pyx_t_3 = (__pyx_t_2 != 0);
     if (__pyx_t_3) {
 
       /* "pyrfc/_cyrfc.pyx":1183
  *                 unitAttr.satTrace = attributes['sat_trace']
  *             if 'unit_history' in attributes:
  *                 unitAttr.unitHistory = attributes['unit_history']             # <<<<<<<<<<<<<<
  *             if 'lock' in attributes:
  *                 unitAttr.lock = attributes['lock']
  */
-      __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_attributes, __pyx_n_s_unit_history); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1183, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_attributes, __pyx_n_u_unit_history); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1183, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __pyx_t_10 = __Pyx_PyInt_As_short(__pyx_t_1); if (unlikely((__pyx_t_10 == (short)-1) && PyErr_Occurred())) __PYX_ERR(0, 1183, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __pyx_v_unitAttr.unitHistory = __pyx_t_10;
 
       /* "pyrfc/_cyrfc.pyx":1182
  *             if 'sat_trace' in attributes:
@@ -13922,26 +13966,26 @@
     /* "pyrfc/_cyrfc.pyx":1184
  *             if 'unit_history' in attributes:
  *                 unitAttr.unitHistory = attributes['unit_history']
  *             if 'lock' in attributes:             # <<<<<<<<<<<<<<
  *                 unitAttr.lock = attributes['lock']
  *             if 'no_commit_check' in attributes:
  */
-    __pyx_t_3 = (__Pyx_PySequence_ContainsTF(__pyx_n_s_lock, __pyx_v_attributes, Py_EQ)); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 1184, __pyx_L1_error)
+    __pyx_t_3 = (__Pyx_PySequence_ContainsTF(__pyx_n_u_lock, __pyx_v_attributes, Py_EQ)); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 1184, __pyx_L1_error)
     __pyx_t_2 = (__pyx_t_3 != 0);
     if (__pyx_t_2) {
 
       /* "pyrfc/_cyrfc.pyx":1185
  *                 unitAttr.unitHistory = attributes['unit_history']
  *             if 'lock' in attributes:
  *                 unitAttr.lock = attributes['lock']             # <<<<<<<<<<<<<<
  *             if 'no_commit_check' in attributes:
  *                 unitAttr.noCommitCheck = attributes['no_commit_check']
  */
-      __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_attributes, __pyx_n_s_lock); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1185, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_attributes, __pyx_n_u_lock); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1185, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __pyx_t_10 = __Pyx_PyInt_As_short(__pyx_t_1); if (unlikely((__pyx_t_10 == (short)-1) && PyErr_Occurred())) __PYX_ERR(0, 1185, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __pyx_v_unitAttr.lock = __pyx_t_10;
 
       /* "pyrfc/_cyrfc.pyx":1184
  *             if 'unit_history' in attributes:
@@ -13955,26 +13999,26 @@
     /* "pyrfc/_cyrfc.pyx":1186
  *             if 'lock' in attributes:
  *                 unitAttr.lock = attributes['lock']
  *             if 'no_commit_check' in attributes:             # <<<<<<<<<<<<<<
  *                 unitAttr.noCommitCheck = attributes['no_commit_check']
  *             if 'user' in attributes and attributes['user'] is not None:
  */
-    __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_n_s_no_commit_check, __pyx_v_attributes, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 1186, __pyx_L1_error)
+    __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_n_u_no_commit_check, __pyx_v_attributes, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 1186, __pyx_L1_error)
     __pyx_t_3 = (__pyx_t_2 != 0);
     if (__pyx_t_3) {
 
       /* "pyrfc/_cyrfc.pyx":1187
  *                 unitAttr.lock = attributes['lock']
  *             if 'no_commit_check' in attributes:
  *                 unitAttr.noCommitCheck = attributes['no_commit_check']             # <<<<<<<<<<<<<<
  *             if 'user' in attributes and attributes['user'] is not None:
  *                 # (SAP_UC[12+1]) Sender User (optional). Default is current operating system User.
  */
-      __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_attributes, __pyx_n_s_no_commit_check); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1187, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_attributes, __pyx_n_u_no_commit_check); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1187, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __pyx_t_10 = __Pyx_PyInt_As_short(__pyx_t_1); if (unlikely((__pyx_t_10 == (short)-1) && PyErr_Occurred())) __PYX_ERR(0, 1187, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __pyx_v_unitAttr.noCommitCheck = __pyx_t_10;
 
       /* "pyrfc/_cyrfc.pyx":1186
  *             if 'lock' in attributes:
@@ -13988,22 +14032,22 @@
     /* "pyrfc/_cyrfc.pyx":1188
  *             if 'no_commit_check' in attributes:
  *                 unitAttr.noCommitCheck = attributes['no_commit_check']
  *             if 'user' in attributes and attributes['user'] is not None:             # <<<<<<<<<<<<<<
  *                 # (SAP_UC[12+1]) Sender User (optional). Default is current operating system User.
  *                 sapuc = fillString(attributes['user'][0:12])
  */
-    __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_n_s_user, __pyx_v_attributes, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 1188, __pyx_L1_error)
+    __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_n_u_user, __pyx_v_attributes, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 1188, __pyx_L1_error)
     __pyx_t_11 = (__pyx_t_2 != 0);
     if (__pyx_t_11) {
     } else {
       __pyx_t_3 = __pyx_t_11;
       goto __pyx_L16_bool_binop_done;
     }
-    __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_attributes, __pyx_n_s_user); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1188, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_attributes, __pyx_n_u_user); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1188, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_11 = (__pyx_t_1 != Py_None);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_2 = (__pyx_t_11 != 0);
     __pyx_t_3 = __pyx_t_2;
     __pyx_L16_bool_binop_done:;
     if (__pyx_t_3) {
@@ -14011,15 +14055,15 @@
       /* "pyrfc/_cyrfc.pyx":1190
  *             if 'user' in attributes and attributes['user'] is not None:
  *                 # (SAP_UC[12+1]) Sender User (optional). Default is current operating system User.
  *                 sapuc = fillString(attributes['user'][0:12])             # <<<<<<<<<<<<<<
  *                 strncpyU(unitAttr.user, sapuc, len(attributes['user'][0:12]) + 1)
  *                 free(sapuc)
  */
-      __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_attributes, __pyx_n_s_user); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1190, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_attributes, __pyx_n_u_user); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1190, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __pyx_t_5 = __Pyx_PyObject_GetSlice(__pyx_t_1, 0, 12, NULL, NULL, &__pyx_slice__12, 1, 1, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1190, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __pyx_t_4 = __pyx_f_5pyrfc_6_cyrfc_fillString(__pyx_t_5); if (unlikely(__pyx_t_4 == ((SAP_UC *)NULL))) __PYX_ERR(0, 1190, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __pyx_v_sapuc = __pyx_t_4;
@@ -14027,15 +14071,15 @@
       /* "pyrfc/_cyrfc.pyx":1191
  *                 # (SAP_UC[12+1]) Sender User (optional). Default is current operating system User.
  *                 sapuc = fillString(attributes['user'][0:12])
  *                 strncpyU(unitAttr.user, sapuc, len(attributes['user'][0:12]) + 1)             # <<<<<<<<<<<<<<
  *                 free(sapuc)
  *             if 'client' in attributes:
  */
-      __pyx_t_5 = __Pyx_PyObject_Dict_GetItem(__pyx_v_attributes, __pyx_n_s_user); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1191, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyObject_Dict_GetItem(__pyx_v_attributes, __pyx_n_u_user); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1191, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __pyx_t_1 = __Pyx_PyObject_GetSlice(__pyx_t_5, 0, 12, NULL, NULL, &__pyx_slice__12, 1, 1, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1191, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __pyx_t_6 = PyObject_Length(__pyx_t_1); if (unlikely(__pyx_t_6 == ((Py_ssize_t)-1))) __PYX_ERR(0, 1191, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       strncpyU(__pyx_v_unitAttr.user, __pyx_v_sapuc, (__pyx_t_6 + 1));
@@ -14061,26 +14105,26 @@
     /* "pyrfc/_cyrfc.pyx":1193
  *                 strncpyU(unitAttr.user, sapuc, len(attributes['user'][0:12]) + 1)
  *                 free(sapuc)
  *             if 'client' in attributes:             # <<<<<<<<<<<<<<
  *                 # (SAP_UC[3+1]) Sender Client ("Mandant") (optional). Default is "000".
  *                 sapuc = fillString(attributes['client'][0:3])
  */
-    __pyx_t_3 = (__Pyx_PySequence_ContainsTF(__pyx_n_s_client, __pyx_v_attributes, Py_EQ)); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 1193, __pyx_L1_error)
+    __pyx_t_3 = (__Pyx_PySequence_ContainsTF(__pyx_n_u_client, __pyx_v_attributes, Py_EQ)); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 1193, __pyx_L1_error)
     __pyx_t_2 = (__pyx_t_3 != 0);
     if (__pyx_t_2) {
 
       /* "pyrfc/_cyrfc.pyx":1195
  *             if 'client' in attributes:
  *                 # (SAP_UC[3+1]) Sender Client ("Mandant") (optional). Default is "000".
  *                 sapuc = fillString(attributes['client'][0:3])             # <<<<<<<<<<<<<<
  *                 strncpyU(unitAttr.client, sapuc, len(attributes['client'][0:3]) + 1)
  *                 free(sapuc)
  */
-      __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_attributes, __pyx_n_s_client); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1195, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_attributes, __pyx_n_u_client); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1195, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __pyx_t_5 = __Pyx_PyObject_GetSlice(__pyx_t_1, 0, 3, NULL, NULL, &__pyx_slice__13, 1, 1, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1195, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __pyx_t_4 = __pyx_f_5pyrfc_6_cyrfc_fillString(__pyx_t_5); if (unlikely(__pyx_t_4 == ((SAP_UC *)NULL))) __PYX_ERR(0, 1195, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __pyx_v_sapuc = __pyx_t_4;
@@ -14088,15 +14132,15 @@
       /* "pyrfc/_cyrfc.pyx":1196
  *                 # (SAP_UC[3+1]) Sender Client ("Mandant") (optional). Default is "000".
  *                 sapuc = fillString(attributes['client'][0:3])
  *                 strncpyU(unitAttr.client, sapuc, len(attributes['client'][0:3]) + 1)             # <<<<<<<<<<<<<<
  *                 free(sapuc)
  *             if 't_code' in attributes:
  */
-      __pyx_t_5 = __Pyx_PyObject_Dict_GetItem(__pyx_v_attributes, __pyx_n_s_client); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1196, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyObject_Dict_GetItem(__pyx_v_attributes, __pyx_n_u_client); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1196, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __pyx_t_1 = __Pyx_PyObject_GetSlice(__pyx_t_5, 0, 3, NULL, NULL, &__pyx_slice__13, 1, 1, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1196, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __pyx_t_6 = PyObject_Length(__pyx_t_1); if (unlikely(__pyx_t_6 == ((Py_ssize_t)-1))) __PYX_ERR(0, 1196, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       strncpyU(__pyx_v_unitAttr.client, __pyx_v_sapuc, (__pyx_t_6 + 1));
@@ -14122,26 +14166,26 @@
     /* "pyrfc/_cyrfc.pyx":1198
  *                 strncpyU(unitAttr.client, sapuc, len(attributes['client'][0:3]) + 1)
  *                 free(sapuc)
  *             if 't_code' in attributes:             # <<<<<<<<<<<<<<
  *                 # (SAP_UC[20+1]) Sender Transaction Code (optional). Default is "".
  *                 sapuc = fillString(attributes['t_code'][0:20])
  */
-    __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_n_s_t_code, __pyx_v_attributes, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 1198, __pyx_L1_error)
+    __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_n_u_t_code, __pyx_v_attributes, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 1198, __pyx_L1_error)
     __pyx_t_3 = (__pyx_t_2 != 0);
     if (__pyx_t_3) {
 
       /* "pyrfc/_cyrfc.pyx":1200
  *             if 't_code' in attributes:
  *                 # (SAP_UC[20+1]) Sender Transaction Code (optional). Default is "".
  *                 sapuc = fillString(attributes['t_code'][0:20])             # <<<<<<<<<<<<<<
  *                 strncpyU(unitAttr.tCode, sapuc, len(attributes['t_code'][0:20]) + 1)
  *                 free(sapuc)
  */
-      __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_attributes, __pyx_n_s_t_code); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1200, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_attributes, __pyx_n_u_t_code); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1200, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __pyx_t_5 = __Pyx_PyObject_GetSlice(__pyx_t_1, 0, 20, NULL, NULL, &__pyx_slice__14, 1, 1, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1200, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __pyx_t_4 = __pyx_f_5pyrfc_6_cyrfc_fillString(__pyx_t_5); if (unlikely(__pyx_t_4 == ((SAP_UC *)NULL))) __PYX_ERR(0, 1200, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __pyx_v_sapuc = __pyx_t_4;
@@ -14149,15 +14193,15 @@
       /* "pyrfc/_cyrfc.pyx":1201
  *                 # (SAP_UC[20+1]) Sender Transaction Code (optional). Default is "".
  *                 sapuc = fillString(attributes['t_code'][0:20])
  *                 strncpyU(unitAttr.tCode, sapuc, len(attributes['t_code'][0:20]) + 1)             # <<<<<<<<<<<<<<
  *                 free(sapuc)
  *             if 'program' in attributes and attributes['program'] is not None:
  */
-      __pyx_t_5 = __Pyx_PyObject_Dict_GetItem(__pyx_v_attributes, __pyx_n_s_t_code); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1201, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyObject_Dict_GetItem(__pyx_v_attributes, __pyx_n_u_t_code); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1201, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __pyx_t_1 = __Pyx_PyObject_GetSlice(__pyx_t_5, 0, 20, NULL, NULL, &__pyx_slice__14, 1, 1, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1201, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __pyx_t_6 = PyObject_Length(__pyx_t_1); if (unlikely(__pyx_t_6 == ((Py_ssize_t)-1))) __PYX_ERR(0, 1201, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       strncpyU(__pyx_v_unitAttr.tCode, __pyx_v_sapuc, (__pyx_t_6 + 1));
@@ -14183,22 +14227,22 @@
     /* "pyrfc/_cyrfc.pyx":1203
  *                 strncpyU(unitAttr.tCode, sapuc, len(attributes['t_code'][0:20]) + 1)
  *                 free(sapuc)
  *             if 'program' in attributes and attributes['program'] is not None:             # <<<<<<<<<<<<<<
  *                 # (SAP_UC[40+1]) Sender Program (optional). Default is current executable name.
  *                 sapuc = fillString(attributes['program'][0:40])
  */
-    __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_n_s_program, __pyx_v_attributes, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 1203, __pyx_L1_error)
+    __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_n_u_program, __pyx_v_attributes, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 1203, __pyx_L1_error)
     __pyx_t_11 = (__pyx_t_2 != 0);
     if (__pyx_t_11) {
     } else {
       __pyx_t_3 = __pyx_t_11;
       goto __pyx_L21_bool_binop_done;
     }
-    __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_attributes, __pyx_n_s_program); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1203, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_attributes, __pyx_n_u_program); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1203, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_11 = (__pyx_t_1 != Py_None);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_2 = (__pyx_t_11 != 0);
     __pyx_t_3 = __pyx_t_2;
     __pyx_L21_bool_binop_done:;
     if (__pyx_t_3) {
@@ -14206,15 +14250,15 @@
       /* "pyrfc/_cyrfc.pyx":1205
  *             if 'program' in attributes and attributes['program'] is not None:
  *                 # (SAP_UC[40+1]) Sender Program (optional). Default is current executable name.
  *                 sapuc = fillString(attributes['program'][0:40])             # <<<<<<<<<<<<<<
  *                 strncpyU(unitAttr.program, sapuc, len(attributes['program'][0:40]) + 1)
  *                 free(sapuc)
  */
-      __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_attributes, __pyx_n_s_program); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1205, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_attributes, __pyx_n_u_program); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1205, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __pyx_t_5 = __Pyx_PyObject_GetSlice(__pyx_t_1, 0, 40, NULL, NULL, &__pyx_slice__15, 1, 1, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1205, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __pyx_t_4 = __pyx_f_5pyrfc_6_cyrfc_fillString(__pyx_t_5); if (unlikely(__pyx_t_4 == ((SAP_UC *)NULL))) __PYX_ERR(0, 1205, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __pyx_v_sapuc = __pyx_t_4;
@@ -14222,15 +14266,15 @@
       /* "pyrfc/_cyrfc.pyx":1206
  *                 # (SAP_UC[40+1]) Sender Program (optional). Default is current executable name.
  *                 sapuc = fillString(attributes['program'][0:40])
  *                 strncpyU(unitAttr.program, sapuc, len(attributes['program'][0:40]) + 1)             # <<<<<<<<<<<<<<
  *                 free(sapuc)
  * 
  */
-      __pyx_t_5 = __Pyx_PyObject_Dict_GetItem(__pyx_v_attributes, __pyx_n_s_program); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1206, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyObject_Dict_GetItem(__pyx_v_attributes, __pyx_n_u_program); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1206, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __pyx_t_1 = __Pyx_PyObject_GetSlice(__pyx_t_5, 0, 40, NULL, NULL, &__pyx_slice__15, 1, 1, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1206, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __pyx_t_6 = PyObject_Length(__pyx_t_1); if (unlikely(__pyx_t_6 == ((Py_ssize_t)-1))) __PYX_ERR(0, 1206, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       strncpyU(__pyx_v_unitAttr.program, __pyx_v_sapuc, (__pyx_t_6 + 1));
@@ -14790,15 +14834,17 @@
       /* "pyrfc/_cyrfc.pyx":1243
  *                     RfcDestroyFunction(funcCont, NULL)
  *             # execute
  *             print (" Invocation finished. submitting unit.")             # <<<<<<<<<<<<<<
  *             with nogil:
  *                 rc = RfcSubmitUnit(self._uHandle, &errorInfo)
  */
-      if (__Pyx_PrintOne(0, __pyx_kp_s_Invocation_finished_submitting) < 0) __PYX_ERR(0, 1243, __pyx_L27_error)
+      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_print, __pyx_tuple__16, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1243, __pyx_L27_error)
+      __Pyx_GOTREF(__pyx_t_1);
+      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
       /* "pyrfc/_cyrfc.pyx":1244
  *             # execute
  *             print (" Invocation finished. submitting unit.")
  *             with nogil:             # <<<<<<<<<<<<<<
  *                 rc = RfcSubmitUnit(self._uHandle, &errorInfo)
  *             if rc != RFC_OK:
@@ -14907,37 +14953,83 @@
       __Pyx_AddTraceback("pyrfc._cyrfc.Connection._create_and_submit_unit", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_8, &__pyx_t_5, &__pyx_t_1) < 0) __PYX_ERR(0, 1249, __pyx_L29_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_INCREF(__pyx_t_5);
       __pyx_v_e = __pyx_t_5;
+      /*try:*/ {
 
-      /* "pyrfc/_cyrfc.pyx":1251
+        /* "pyrfc/_cyrfc.pyx":1251
  *         except RFCError as e:
  *             # clean up actions
  *             RfcDestroyUnit(self._uHandle, NULL)             # <<<<<<<<<<<<<<
  *             raise
  * 
  */
-      (void)(RfcDestroyUnit(__pyx_v_self->_uHandle, NULL));
+        (void)(RfcDestroyUnit(__pyx_v_self->_uHandle, NULL));
 
-      /* "pyrfc/_cyrfc.pyx":1252
+        /* "pyrfc/_cyrfc.pyx":1252
  *             # clean up actions
  *             RfcDestroyUnit(self._uHandle, NULL)
  *             raise             # <<<<<<<<<<<<<<
  * 
  *         unit_identifier = wrapUnitIdentifier(uIdentifier)
  */
-      __Pyx_GIVEREF(__pyx_t_8);
-      __Pyx_GIVEREF(__pyx_t_5);
-      __Pyx_XGIVEREF(__pyx_t_1);
-      __Pyx_ErrRestoreWithState(__pyx_t_8, __pyx_t_5, __pyx_t_1);
-      __pyx_t_8 = 0; __pyx_t_5 = 0; __pyx_t_1 = 0; 
-      __PYX_ERR(0, 1252, __pyx_L29_except_error)
+        __Pyx_GIVEREF(__pyx_t_8);
+        __Pyx_GIVEREF(__pyx_t_5);
+        __Pyx_XGIVEREF(__pyx_t_1);
+        __Pyx_ErrRestoreWithState(__pyx_t_8, __pyx_t_5, __pyx_t_1);
+        __pyx_t_8 = 0; __pyx_t_5 = 0; __pyx_t_1 = 0; 
+        __PYX_ERR(0, 1252, __pyx_L60_error)
+      }
+
+      /* "pyrfc/_cyrfc.pyx":1249
+ *                 self._error(&errorInfo)
+ * 
+ *         except RFCError as e:             # <<<<<<<<<<<<<<
+ *             # clean up actions
+ *             RfcDestroyUnit(self._uHandle, NULL)
+ */
+      /*finally:*/ {
+        __pyx_L60_error:;
+        /*exception exit:*/{
+          __Pyx_PyThreadState_declare
+          __Pyx_PyThreadState_assign
+          __pyx_t_27 = 0; __pyx_t_26 = 0; __pyx_t_25 = 0; __pyx_t_24 = 0; __pyx_t_23 = 0; __pyx_t_22 = 0;
+          __Pyx_XDECREF(__pyx_t_15); __pyx_t_15 = 0;
+          __Pyx_XDECREF(__pyx_t_16); __pyx_t_16 = 0;
+          if (PY_MAJOR_VERSION >= 3) __Pyx_ExceptionSwap(&__pyx_t_24, &__pyx_t_23, &__pyx_t_22);
+          if ((PY_MAJOR_VERSION < 3) || unlikely(__Pyx_GetException(&__pyx_t_27, &__pyx_t_26, &__pyx_t_25) < 0)) __Pyx_ErrFetch(&__pyx_t_27, &__pyx_t_26, &__pyx_t_25);
+          __Pyx_XGOTREF(__pyx_t_27);
+          __Pyx_XGOTREF(__pyx_t_26);
+          __Pyx_XGOTREF(__pyx_t_25);
+          __Pyx_XGOTREF(__pyx_t_24);
+          __Pyx_XGOTREF(__pyx_t_23);
+          __Pyx_XGOTREF(__pyx_t_22);
+          __pyx_t_20 = __pyx_lineno; __pyx_t_19 = __pyx_clineno; __pyx_t_28 = __pyx_filename;
+          {
+            __Pyx_DECREF(__pyx_v_e);
+            __pyx_v_e = NULL;
+          }
+          if (PY_MAJOR_VERSION >= 3) {
+            __Pyx_XGIVEREF(__pyx_t_24);
+            __Pyx_XGIVEREF(__pyx_t_23);
+            __Pyx_XGIVEREF(__pyx_t_22);
+            __Pyx_ExceptionReset(__pyx_t_24, __pyx_t_23, __pyx_t_22);
+          }
+          __Pyx_XGIVEREF(__pyx_t_27);
+          __Pyx_XGIVEREF(__pyx_t_26);
+          __Pyx_XGIVEREF(__pyx_t_25);
+          __Pyx_ErrRestore(__pyx_t_27, __pyx_t_26, __pyx_t_25);
+          __pyx_t_27 = 0; __pyx_t_26 = 0; __pyx_t_25 = 0; __pyx_t_24 = 0; __pyx_t_23 = 0; __pyx_t_22 = 0;
+          __pyx_lineno = __pyx_t_20; __pyx_clineno = __pyx_t_19; __pyx_filename = __pyx_t_28;
+          goto __pyx_L29_except_error;
+        }
+      }
     }
     goto __pyx_L29_except_error;
     __pyx_L29_except_error:;
 
     /* "pyrfc/_cyrfc.pyx":1223
  *         self.active_unit = True
  * 
@@ -14969,15 +15061,15 @@
  * 
  *         unit_identifier = wrapUnitIdentifier(uIdentifier)
  *         return unit_identifier["queued"]             # <<<<<<<<<<<<<<
  * 
  *     def _get_unit_state(self, unit):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_unit_identifier, __pyx_n_s_queued); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1255, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_unit_identifier, __pyx_n_u_queued); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1255, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* "pyrfc/_cyrfc.pyx":1119
  *         return wrapString(uid, RFC_UNITID_LN)
@@ -15089,15 +15181,15 @@
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_4, function);
       }
     }
-    __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_kp_s_No_unit_handle_for_this_connecti) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_kp_s_No_unit_handle_for_this_connecti);
+    __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_kp_u_No_unit_handle_for_this_connecti) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_kp_u_No_unit_handle_for_this_connecti);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1264, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(0, 1264, __pyx_L1_error)
@@ -15232,15 +15324,15 @@
     __Pyx_GOTREF(__pyx_t_5);
     __pyx_t_9 = 0;
     __pyx_t_10 = 127;
     __Pyx_INCREF(__pyx_kp_u_Unit);
     __pyx_t_9 += 5;
     __Pyx_GIVEREF(__pyx_kp_u_Unit);
     PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_kp_u_Unit);
-    __pyx_t_7 = __Pyx_PyObject_Dict_GetItem(__pyx_v_unit, __pyx_n_s_id); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1271, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_Dict_GetItem(__pyx_v_unit, __pyx_n_u_id); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1271, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __pyx_t_8 = __Pyx_PyObject_FormatSimple(__pyx_t_7, __pyx_empty_unicode); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1271, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __pyx_t_10 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_8) > __pyx_t_10) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_8) : __pyx_t_10;
     __pyx_t_9 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_8);
     __Pyx_GIVEREF(__pyx_t_8);
@@ -15412,15 +15504,15 @@
       if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_4);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
-    __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_kp_s_No_unit_handle_for_this_connecti) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_kp_s_No_unit_handle_for_this_connecti);
+    __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_kp_u_No_unit_handle_for_this_connecti) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_kp_u_No_unit_handle_for_this_connecti);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1278, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __PYX_ERR(0, 1278, __pyx_L1_error)
@@ -15612,15 +15704,15 @@
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_4, function);
       }
     }
-    __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_kp_s_No_unit_handle_for_this_connecti) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_kp_s_No_unit_handle_for_this_connecti);
+    __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_kp_u_No_unit_handle_for_this_connecti) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_kp_u_No_unit_handle_for_this_connecti);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1292, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(0, 1292, __pyx_L1_error)
@@ -15972,15 +16064,15 @@
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_4, function);
       }
     }
-    __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_kp_s_Argument_background_must_be_a_bo) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_kp_s_Argument_background_must_be_a_bo);
+    __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_kp_u_Argument_background_must_be_a_bo) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_kp_u_Argument_background_must_be_a_bo);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1331, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(0, 1331, __pyx_L1_error)
@@ -15993,17 +16085,17 @@
  *         return {'background': background, 'id': id, "queued": False}             # <<<<<<<<<<<<<<
  * 
  *     def fill_and_submit_unit(self, unit, calls, queue_names=None, attributes=None):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_3 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1332, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_background, __pyx_v_background) < 0) __PYX_ERR(0, 1332, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_id, __pyx_v_id) < 0) __PYX_ERR(0, 1332, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_queued, Py_False) < 0) __PYX_ERR(0, 1332, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_background, __pyx_v_background) < 0) __PYX_ERR(0, 1332, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_id, __pyx_v_id) < 0) __PYX_ERR(0, 1332, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_queued, Py_False) < 0) __PYX_ERR(0, 1332, __pyx_L1_error)
   __pyx_r = __pyx_t_3;
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
   /* "pyrfc/_cyrfc.pyx":1311
  *     # * queued - boolean, set on fill_and_submit_unit() call
  * 
@@ -16164,35 +16256,35 @@
   __pyx_t_2 = (((PyObject *)Py_TYPE(__pyx_v_unit)) != ((PyObject *)(&PyDict_Type)));
   __pyx_t_3 = (__pyx_t_2 != 0);
   if (!__pyx_t_3) {
   } else {
     __pyx_t_1 = __pyx_t_3;
     goto __pyx_L4_bool_binop_done;
   }
-  __pyx_t_3 = (__Pyx_PySequence_ContainsTF(__pyx_n_s_id, __pyx_v_unit, Py_NE)); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 1387, __pyx_L1_error)
+  __pyx_t_3 = (__Pyx_PySequence_ContainsTF(__pyx_n_u_id, __pyx_v_unit, Py_NE)); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 1387, __pyx_L1_error)
   __pyx_t_2 = (__pyx_t_3 != 0);
   if (!__pyx_t_2) {
   } else {
     __pyx_t_1 = __pyx_t_2;
     goto __pyx_L4_bool_binop_done;
   }
-  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_n_s_background, __pyx_v_unit, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 1387, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_n_u_background, __pyx_v_unit, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 1387, __pyx_L1_error)
   __pyx_t_3 = (__pyx_t_2 != 0);
   __pyx_t_1 = __pyx_t_3;
   __pyx_L4_bool_binop_done:;
   if (unlikely(__pyx_t_1)) {
 
     /* "pyrfc/_cyrfc.pyx":1388
  * 
  *         if type(unit) is not dict or 'id' not in unit or 'background' not in unit:
  *             raise TypeError("Parameter 'unit' not valid. Please use initialize_unit() to retrieve a valid unit.")             # <<<<<<<<<<<<<<
  *         if not isinstance(calls, Iterable):
  *             raise TypeError("Parameter 'calls' must be iterable.")
  */
-    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__16, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1388, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__17, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1388, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __PYX_ERR(0, 1388, __pyx_L1_error)
 
     /* "pyrfc/_cyrfc.pyx":1387
  *         """
@@ -16220,15 +16312,15 @@
     /* "pyrfc/_cyrfc.pyx":1390
  *             raise TypeError("Parameter 'unit' not valid. Please use initialize_unit() to retrieve a valid unit.")
  *         if not isinstance(calls, Iterable):
  *             raise TypeError("Parameter 'calls' must be iterable.")             # <<<<<<<<<<<<<<
  *         if len(calls)==0:
  *             raise TypeError("Parameter 'calls' must contain at least on call description (func_name, params).")
  */
-    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__17, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1390, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__18, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1390, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __PYX_ERR(0, 1390, __pyx_L1_error)
 
     /* "pyrfc/_cyrfc.pyx":1389
  *         if type(unit) is not dict or 'id' not in unit or 'background' not in unit:
@@ -16253,15 +16345,15 @@
     /* "pyrfc/_cyrfc.pyx":1392
  *             raise TypeError("Parameter 'calls' must be iterable.")
  *         if len(calls)==0:
  *             raise TypeError("Parameter 'calls' must contain at least on call description (func_name, params).")             # <<<<<<<<<<<<<<
  *         for func_name, params in calls:
  *             if type(func_name) is not str or type(params) is not dict:
  */
-    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__18, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1392, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__19, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1392, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __PYX_ERR(0, 1392, __pyx_L1_error)
 
     /* "pyrfc/_cyrfc.pyx":1391
  *         if not isinstance(calls, Iterable):
@@ -16372,15 +16464,15 @@
     /* "pyrfc/_cyrfc.pyx":1394
  *             raise TypeError("Parameter 'calls' must contain at least on call description (func_name, params).")
  *         for func_name, params in calls:
  *             if type(func_name) is not str or type(params) is not dict:             # <<<<<<<<<<<<<<
  *                 raise TypeError("Parameter 'calls' must contain valid call descriptions (func_name, params dict).")
  *         if self.active_unit:
  */
-    __pyx_t_1 = (((PyObject *)Py_TYPE(__pyx_v_func_name)) != ((PyObject *)(&PyString_Type)));
+    __pyx_t_1 = (((PyObject *)Py_TYPE(__pyx_v_func_name)) != ((PyObject *)(&PyUnicode_Type)));
     __pyx_t_2 = (__pyx_t_1 != 0);
     if (!__pyx_t_2) {
     } else {
       __pyx_t_3 = __pyx_t_2;
       goto __pyx_L14_bool_binop_done;
     }
     __pyx_t_2 = (((PyObject *)Py_TYPE(__pyx_v_params)) != ((PyObject *)(&PyDict_Type)));
@@ -16392,15 +16484,15 @@
       /* "pyrfc/_cyrfc.pyx":1395
  *         for func_name, params in calls:
  *             if type(func_name) is not str or type(params) is not dict:
  *                 raise TypeError("Parameter 'calls' must contain valid call descriptions (func_name, params dict).")             # <<<<<<<<<<<<<<
  *         if self.active_unit:
  *             raise RFCError("There is an active unit for this connection. "
  */
-      __pyx_t_7 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__19, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1395, __pyx_L1_error)
+      __pyx_t_7 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__20, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1395, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_Raise(__pyx_t_7, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       __PYX_ERR(0, 1395, __pyx_L1_error)
 
       /* "pyrfc/_cyrfc.pyx":1394
  *             raise TypeError("Parameter 'calls' must contain at least on call description (func_name, params).")
@@ -16436,37 +16528,26 @@
  *         if self.active_unit:
  *             raise RFCError("There is an active unit for this connection. "             # <<<<<<<<<<<<<<
  *                            "Use destroy_unit() " +
  *                            "or confirm_unit().")
  */
     __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_RFCError); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1397, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-
-    /* "pyrfc/_cyrfc.pyx":1398
- *         if self.active_unit:
- *             raise RFCError("There is an active unit for this connection. "
- *                            "Use destroy_unit() " +             # <<<<<<<<<<<<<<
- *                            "or confirm_unit().")
- *         bg = unit['background']
- */
-    __pyx_t_9 = PyNumber_Add(__pyx_kp_s_There_is_an_active_unit_for_this, __pyx_kp_s_or_confirm_unit); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 1398, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_9);
-    __pyx_t_8 = NULL;
+    __pyx_t_9 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_7))) {
-      __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_7);
-      if (likely(__pyx_t_8)) {
+      __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_7);
+      if (likely(__pyx_t_9)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
-        __Pyx_INCREF(__pyx_t_8);
+        __Pyx_INCREF(__pyx_t_9);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_7, function);
       }
     }
-    __pyx_t_4 = (__pyx_t_8) ? __Pyx_PyObject_Call2Args(__pyx_t_7, __pyx_t_8, __pyx_t_9) : __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_t_9);
-    __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
-    __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+    __pyx_t_4 = (__pyx_t_9) ? __Pyx_PyObject_Call2Args(__pyx_t_7, __pyx_t_9, __pyx_kp_u_There_is_an_active_unit_for_this) : __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_kp_u_There_is_an_active_unit_for_this);
+    __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
     if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1397, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __PYX_ERR(0, 1397, __pyx_L1_error)
 
@@ -16482,27 +16563,27 @@
   /* "pyrfc/_cyrfc.pyx":1400
  *                            "Use destroy_unit() " +
  *                            "or confirm_unit().")
  *         bg = unit['background']             # <<<<<<<<<<<<<<
  *         unit_id = unit['id']
  * 
  */
-  __pyx_t_4 = __Pyx_PyObject_Dict_GetItem(__pyx_v_unit, __pyx_n_s_background); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1400, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Dict_GetItem(__pyx_v_unit, __pyx_n_u_background); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1400, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_v_bg = __pyx_t_4;
   __pyx_t_4 = 0;
 
   /* "pyrfc/_cyrfc.pyx":1401
  *                            "or confirm_unit().")
  *         bg = unit['background']
  *         unit_id = unit['id']             # <<<<<<<<<<<<<<
  * 
  *         if bg is True:
  */
-  __pyx_t_4 = __Pyx_PyObject_Dict_GetItem(__pyx_v_unit, __pyx_n_s_id); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1401, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Dict_GetItem(__pyx_v_unit, __pyx_n_u_id); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1401, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_v_unit_id = __pyx_t_4;
   __pyx_t_4 = 0;
 
   /* "pyrfc/_cyrfc.pyx":1403
  *         unit_id = unit['id']
  * 
@@ -16553,18 +16634,18 @@
       __pyx_t_13 = PyObject_Length(__pyx_v_unit_id); if (unlikely(__pyx_t_13 == ((Py_ssize_t)-1))) __PYX_ERR(0, 1405, __pyx_L1_error)
       __pyx_t_7 = __Pyx_PyUnicode_From_Py_ssize_t(__pyx_t_13, 0, ' ', 'd'); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1405, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       __pyx_t_5 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_7);
       __Pyx_GIVEREF(__pyx_t_7);
       PyTuple_SET_ITEM(__pyx_t_4, 3, __pyx_t_7);
       __pyx_t_7 = 0;
-      __Pyx_INCREF(__pyx_kp_u__20);
+      __Pyx_INCREF(__pyx_kp_u__21);
       __pyx_t_5 += 1;
-      __Pyx_GIVEREF(__pyx_kp_u__20);
-      PyTuple_SET_ITEM(__pyx_t_4, 4, __pyx_kp_u__20);
+      __Pyx_GIVEREF(__pyx_kp_u__21);
+      PyTuple_SET_ITEM(__pyx_t_4, 4, __pyx_kp_u__21);
       __pyx_t_7 = __Pyx_PyUnicode_Join(__pyx_t_4, 5, __pyx_t_5, __pyx_t_12); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1405, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_TypeError, __pyx_t_7); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1405, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       __Pyx_Raise(__pyx_t_4, 0, 0, 0);
@@ -16636,15 +16717,15 @@
       __Pyx_GIVEREF(__pyx_v_attributes);
       PyTuple_SET_ITEM(__pyx_t_8, 3+__pyx_t_14, __pyx_v_attributes);
       __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_t_8, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1406, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     }
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    if (unlikely(PyObject_SetItem(__pyx_v_unit, __pyx_n_s_queued, __pyx_t_4) < 0)) __PYX_ERR(0, 1406, __pyx_L1_error)
+    if (unlikely(PyObject_SetItem(__pyx_v_unit, __pyx_n_u_queued, __pyx_t_4) < 0)) __PYX_ERR(0, 1406, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "pyrfc/_cyrfc.pyx":1403
  *         unit_id = unit['id']
  * 
  *         if bg is True:             # <<<<<<<<<<<<<<
  *             if len(unit_id) != RFC_UNITID_LN:
@@ -16703,18 +16784,18 @@
       __pyx_t_13 = PyObject_Length(__pyx_v_unit_id); if (unlikely(__pyx_t_13 == ((Py_ssize_t)-1))) __PYX_ERR(0, 1409, __pyx_L1_error)
       __pyx_t_7 = __Pyx_PyUnicode_From_Py_ssize_t(__pyx_t_13, 0, ' ', 'd'); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1409, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       __pyx_t_5 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_7);
       __Pyx_GIVEREF(__pyx_t_7);
       PyTuple_SET_ITEM(__pyx_t_4, 3, __pyx_t_7);
       __pyx_t_7 = 0;
-      __Pyx_INCREF(__pyx_kp_u__20);
+      __Pyx_INCREF(__pyx_kp_u__21);
       __pyx_t_5 += 1;
-      __Pyx_GIVEREF(__pyx_kp_u__20);
-      PyTuple_SET_ITEM(__pyx_t_4, 4, __pyx_kp_u__20);
+      __Pyx_GIVEREF(__pyx_kp_u__21);
+      PyTuple_SET_ITEM(__pyx_t_4, 4, __pyx_kp_u__21);
       __pyx_t_7 = __Pyx_PyUnicode_Join(__pyx_t_4, 5, __pyx_t_5, __pyx_t_12); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1409, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_TypeError, __pyx_t_7); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1409, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       __Pyx_Raise(__pyx_t_4, 0, 0, 0);
@@ -16756,15 +16837,15 @@
         if (likely(__pyx_t_8)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
           __Pyx_INCREF(__pyx_t_8);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_7, function);
         }
       }
-      __pyx_t_4 = (__pyx_t_8) ? __Pyx_PyObject_Call2Args(__pyx_t_7, __pyx_t_8, __pyx_kp_s_Argument_attributes_not_valid_t) : __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_kp_s_Argument_attributes_not_valid_t);
+      __pyx_t_4 = (__pyx_t_8) ? __Pyx_PyObject_Call2Args(__pyx_t_7, __pyx_t_8, __pyx_kp_u_Argument_attributes_not_valid_t) : __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_kp_u_Argument_attributes_not_valid_t);
       __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
       if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1411, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       __Pyx_Raise(__pyx_t_4, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __PYX_ERR(0, 1411, __pyx_L1_error)
@@ -16864,15 +16945,15 @@
       /* "pyrfc/_cyrfc.pyx":1414
  *             if queue_names is None or type(queue_names) is list and len(queue_names) == 0:
  *                 self._create_and_submit_transaction(unit_id, calls)
  *                 unit['queued'] = False             # <<<<<<<<<<<<<<
  *             elif len(queue_names) == 1:
  *                 queue_name = queue_names[0]
  */
-      if (unlikely(PyObject_SetItem(__pyx_v_unit, __pyx_n_s_queued, Py_False) < 0)) __PYX_ERR(0, 1414, __pyx_L1_error)
+      if (unlikely(PyObject_SetItem(__pyx_v_unit, __pyx_n_u_queued, Py_False) < 0)) __PYX_ERR(0, 1414, __pyx_L1_error)
 
       /* "pyrfc/_cyrfc.pyx":1412
  *             if attributes is not None:
  *                 raise RFCError("Argument 'attributes' not valid. (t/qRFC does not support attributes.)")
  *             if queue_names is None or type(queue_names) is list and len(queue_names) == 0:             # <<<<<<<<<<<<<<
  *                 self._create_and_submit_transaction(unit_id, calls)
  *                 unit['queued'] = False
@@ -16965,15 +17046,15 @@
       /* "pyrfc/_cyrfc.pyx":1418
  *                 queue_name = queue_names[0]
  *                 self._create_and_submit_transaction(unit_id, calls, queue_name)
  *                 unit['queued'] = True             # <<<<<<<<<<<<<<
  *             else:
  *                 raise RFCError("Argument 'queue_names' not valid. (t/qRFC only support one queue name.)")
  */
-      if (unlikely(PyObject_SetItem(__pyx_v_unit, __pyx_n_s_queued, Py_True) < 0)) __PYX_ERR(0, 1418, __pyx_L1_error)
+      if (unlikely(PyObject_SetItem(__pyx_v_unit, __pyx_n_u_queued, Py_True) < 0)) __PYX_ERR(0, 1418, __pyx_L1_error)
 
       /* "pyrfc/_cyrfc.pyx":1415
  *                 self._create_and_submit_transaction(unit_id, calls)
  *                 unit['queued'] = False
  *             elif len(queue_names) == 1:             # <<<<<<<<<<<<<<
  *                 queue_name = queue_names[0]
  *                 self._create_and_submit_transaction(unit_id, calls, queue_name)
@@ -16997,15 +17078,15 @@
         if (likely(__pyx_t_8)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
           __Pyx_INCREF(__pyx_t_8);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_7, function);
         }
       }
-      __pyx_t_4 = (__pyx_t_8) ? __Pyx_PyObject_Call2Args(__pyx_t_7, __pyx_t_8, __pyx_kp_s_Argument_queue_names_not_valid_t) : __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_kp_s_Argument_queue_names_not_valid_t);
+      __pyx_t_4 = (__pyx_t_8) ? __Pyx_PyObject_Call2Args(__pyx_t_7, __pyx_t_8, __pyx_kp_u_Argument_queue_names_not_valid_t) : __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_kp_u_Argument_queue_names_not_valid_t);
       __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
       if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1420, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       __Pyx_Raise(__pyx_t_4, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __PYX_ERR(0, 1420, __pyx_L1_error)
@@ -17038,15 +17119,15 @@
       if (likely(__pyx_t_8)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
         __Pyx_INCREF(__pyx_t_8);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_7, function);
       }
     }
-    __pyx_t_4 = (__pyx_t_8) ? __Pyx_PyObject_Call2Args(__pyx_t_7, __pyx_t_8, __pyx_kp_s_Argument_unit_not_valid_Is_unit) : __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_kp_s_Argument_unit_not_valid_Is_unit);
+    __pyx_t_4 = (__pyx_t_8) ? __Pyx_PyObject_Call2Args(__pyx_t_7, __pyx_t_8, __pyx_kp_u_Argument_unit_not_valid_Is_unit) : __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_kp_u_Argument_unit_not_valid_Is_unit);
     __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
     if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1422, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __PYX_ERR(0, 1422, __pyx_L1_error)
@@ -17132,15 +17213,15 @@
   /* "pyrfc/_cyrfc.pyx":1440
  *             RFC_UNIT_CONFIRMED
  *         """
  *         bg = unit['background']             # <<<<<<<<<<<<<<
  *         if bg is True:
  *             return self._get_unit_state(unit)
  */
-  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_unit, __pyx_n_s_background); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1440, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_unit, __pyx_n_u_background); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1440, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_bg = __pyx_t_1;
   __pyx_t_1 = 0;
 
   /* "pyrfc/_cyrfc.pyx":1441
  *         """
  *         bg = unit['background']
@@ -17216,15 +17297,15 @@
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_4, function);
       }
     }
-    __pyx_t_1 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_kp_s_No_state_check_possible_of_non_b) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_kp_s_No_state_check_possible_of_non_b);
+    __pyx_t_1 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_kp_u_No_state_check_possible_of_non_b) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_kp_u_No_state_check_possible_of_non_b);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1444, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __PYX_ERR(0, 1444, __pyx_L1_error)
@@ -17254,15 +17335,15 @@
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_4, function);
       }
     }
-    __pyx_t_1 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_kp_s_Argument_unit_not_valid_Is_unit) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_kp_s_Argument_unit_not_valid_Is_unit);
+    __pyx_t_1 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_kp_u_Argument_unit_not_valid_Is_unit) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_kp_u_Argument_unit_not_valid_Is_unit);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1446, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __PYX_ERR(0, 1446, __pyx_L1_error)
@@ -17329,15 +17410,15 @@
   /* "pyrfc/_cyrfc.pyx":1458
  *                  thereof if the connection attempt fails.
  *         """
  *         bg = unit['background']             # <<<<<<<<<<<<<<
  *         if bg is True:
  *             self._destroy_unit()
  */
-  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_unit, __pyx_n_s_background); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1458, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_unit, __pyx_n_u_background); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1458, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_bg = __pyx_t_1;
   __pyx_t_1 = 0;
 
   /* "pyrfc/_cyrfc.pyx":1459
  *         """
  *         bg = unit['background']
@@ -17448,15 +17529,15 @@
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_4, function);
       }
     }
-    __pyx_t_1 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_kp_s_Argument_unit_not_valid_Is_unit) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_kp_s_Argument_unit_not_valid_Is_unit);
+    __pyx_t_1 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_kp_u_Argument_unit_not_valid_Is_unit) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_kp_u_Argument_unit_not_valid_Is_unit);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1464, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __PYX_ERR(0, 1464, __pyx_L1_error)
@@ -17526,15 +17607,15 @@
   /* "pyrfc/_cyrfc.pyx":1476
  *                  thereof if the connection attempt fails.
  *         """
  *         bg = unit['background']             # <<<<<<<<<<<<<<
  *         if bg is True:
  *             self._confirm_unit(unit)
  */
-  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_unit, __pyx_n_s_background); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1476, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_unit, __pyx_n_u_background); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1476, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_bg = __pyx_t_1;
   __pyx_t_1 = 0;
 
   /* "pyrfc/_cyrfc.pyx":1477
  *         """
  *         bg = unit['background']
@@ -17645,15 +17726,15 @@
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_4, function);
       }
     }
-    __pyx_t_1 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_kp_s_Argument_unit_not_valid_Is_unit) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_kp_s_Argument_unit_not_valid_Is_unit);
+    __pyx_t_1 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_kp_u_Argument_unit_not_valid_Is_unit) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_kp_u_Argument_unit_not_valid_Is_unit);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1482, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __PYX_ERR(0, 1482, __pyx_L1_error)
@@ -17822,15 +17903,15 @@
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("self._handle,self._tHandle,self._uHandle cannot be converted to a Python object for pickling")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("self._handle,self._tHandle,self._uHandle cannot be converted to a Python object for pickling")
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__21, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 2, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__22, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(1, 2, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
@@ -17878,15 +17959,15 @@
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":4
  *     raise TypeError("self._handle,self._tHandle,self._uHandle cannot be converted to a Python object for pickling")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("self._handle,self._tHandle,self._uHandle cannot be converted to a Python object for pickling")             # <<<<<<<<<<<<<<
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__22, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__23, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(1, 4, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
@@ -18055,15 +18136,15 @@
   __Pyx_INCREF(__pyx_kp_u__6);
   __pyx_t_5 += 1;
   __Pyx_GIVEREF(__pyx_kp_u__6);
   PyTuple_SET_ITEM(__pyx_t_4, 2, __pyx_kp_u__6);
   __pyx_t_7 = __Pyx_PyUnicode_Join(__pyx_t_4, 3, __pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1503, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_Dict_GetItem(__pyx_v_request_context, __pyx_n_s_server_context); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1503, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Dict_GetItem(__pyx_v_request_context, __pyx_n_u_server_context); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1503, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_8 = NULL;
   __pyx_t_9 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_8)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -18244,15 +18325,15 @@
  * def _server_log(origin, log_message):
  *     if server_context["server_log"]:             # <<<<<<<<<<<<<<
  *         print (f"[{datetime.utcnow()} UTC] {origin} '{log_message}'")
  * 
  */
   __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_server_context); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1508, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_Dict_GetItem(__pyx_t_1, __pyx_n_s_server_log_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1508, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Dict_GetItem(__pyx_t_1, __pyx_n_u_server_log_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1508, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 1508, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (__pyx_t_3) {
 
     /* "pyrfc/_cyrfc.pyx":1509
@@ -18262,18 +18343,18 @@
  * 
  * 
  */
     __pyx_t_2 = PyTuple_New(7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1509, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_4 = 0;
     __pyx_t_5 = 127;
-    __Pyx_INCREF(__pyx_kp_u__23);
+    __Pyx_INCREF(__pyx_kp_u__24);
     __pyx_t_4 += 1;
-    __Pyx_GIVEREF(__pyx_kp_u__23);
-    PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_kp_u__23);
+    __Pyx_GIVEREF(__pyx_kp_u__24);
+    PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_kp_u__24);
     __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_datetime); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1509, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_utcnow); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1509, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __pyx_t_6 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_7))) {
@@ -18305,34 +18386,36 @@
     __pyx_t_7 = __Pyx_PyObject_FormatSimple(__pyx_v_origin, __pyx_empty_unicode); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1509, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __pyx_t_5 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_7) > __pyx_t_5) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_7) : __pyx_t_5;
     __pyx_t_4 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_7);
     __Pyx_GIVEREF(__pyx_t_7);
     PyTuple_SET_ITEM(__pyx_t_2, 3, __pyx_t_7);
     __pyx_t_7 = 0;
-    __Pyx_INCREF(__pyx_kp_u__24);
+    __Pyx_INCREF(__pyx_kp_u__25);
     __pyx_t_4 += 2;
-    __Pyx_GIVEREF(__pyx_kp_u__24);
-    PyTuple_SET_ITEM(__pyx_t_2, 4, __pyx_kp_u__24);
+    __Pyx_GIVEREF(__pyx_kp_u__25);
+    PyTuple_SET_ITEM(__pyx_t_2, 4, __pyx_kp_u__25);
     __pyx_t_7 = __Pyx_PyObject_FormatSimple(__pyx_v_log_message, __pyx_empty_unicode); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1509, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __pyx_t_5 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_7) > __pyx_t_5) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_7) : __pyx_t_5;
     __pyx_t_4 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_7);
     __Pyx_GIVEREF(__pyx_t_7);
     PyTuple_SET_ITEM(__pyx_t_2, 5, __pyx_t_7);
     __pyx_t_7 = 0;
     __Pyx_INCREF(__pyx_kp_u__6);
     __pyx_t_4 += 1;
     __Pyx_GIVEREF(__pyx_kp_u__6);
     PyTuple_SET_ITEM(__pyx_t_2, 6, __pyx_kp_u__6);
     __pyx_t_7 = __Pyx_PyUnicode_Join(__pyx_t_2, 7, __pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1509, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (__Pyx_PrintOne(0, __pyx_t_7) < 0) __PYX_ERR(0, 1509, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_print, __pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1509, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
     /* "pyrfc/_cyrfc.pyx":1508
  * 
  * def _server_log(origin, log_message):
  *     if server_context["server_log"]:             # <<<<<<<<<<<<<<
  *         print (f"[{datetime.utcnow()} UTC] {origin} '{log_message}'")
  * 
@@ -18593,39 +18676,39 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
       __pyx_t_6 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_3)) {
-    PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_kp_s_Server_connection, __pyx_t_5};
+    PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_kp_u_Server_connection, __pyx_t_5};
     __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1530, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
-    PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_kp_s_Server_connection, __pyx_t_5};
+    PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_kp_u_Server_connection, __pyx_t_5};
     __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1530, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   } else
   #endif
   {
     __pyx_t_7 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1530, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     if (__pyx_t_4) {
       __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_4); __pyx_t_4 = NULL;
     }
-    __Pyx_INCREF(__pyx_kp_s_Server_connection);
-    __Pyx_GIVEREF(__pyx_kp_s_Server_connection);
-    PyTuple_SET_ITEM(__pyx_t_7, 0+__pyx_t_6, __pyx_kp_s_Server_connection);
+    __Pyx_INCREF(__pyx_kp_u_Server_connection);
+    __Pyx_GIVEREF(__pyx_kp_u_Server_connection);
+    PyTuple_SET_ITEM(__pyx_t_7, 0+__pyx_t_6, __pyx_kp_u_Server_connection);
     __Pyx_GIVEREF(__pyx_t_5);
     PyTuple_SET_ITEM(__pyx_t_7, 1+__pyx_t_6, __pyx_t_5);
     __pyx_t_5 = 0;
     __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_7, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1530, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   }
@@ -18711,39 +18794,39 @@
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
         __pyx_t_6 = 1;
       }
     }
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(__pyx_t_3)) {
-      PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_kp_s_Server_close, __pyx_t_4};
+      PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_kp_u_Server_close, __pyx_t_4};
       __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1534, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     } else
     #endif
     #if CYTHON_FAST_PYCCALL
     if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
-      PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_kp_s_Server_close, __pyx_t_4};
+      PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_kp_u_Server_close, __pyx_t_4};
       __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1534, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     } else
     #endif
     {
       __pyx_t_7 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1534, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       if (__pyx_t_5) {
         __Pyx_GIVEREF(__pyx_t_5); PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_5); __pyx_t_5 = NULL;
       }
-      __Pyx_INCREF(__pyx_kp_s_Server_close);
-      __Pyx_GIVEREF(__pyx_kp_s_Server_close);
-      PyTuple_SET_ITEM(__pyx_t_7, 0+__pyx_t_6, __pyx_kp_s_Server_close);
+      __Pyx_INCREF(__pyx_kp_u_Server_close);
+      __Pyx_GIVEREF(__pyx_kp_u_Server_close);
+      PyTuple_SET_ITEM(__pyx_t_7, 0+__pyx_t_6, __pyx_kp_u_Server_close);
       __Pyx_GIVEREF(__pyx_t_4);
       PyTuple_SET_ITEM(__pyx_t_7, 1+__pyx_t_6, __pyx_t_4);
       __pyx_t_4 = 0;
       __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_7, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1534, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     }
@@ -19445,15 +19528,15 @@
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("self._handle cannot be converted to a Python object for pickling")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("self._handle cannot be converted to a Python object for pickling")
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__25, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 2, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__26, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(1, 2, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
@@ -19501,15 +19584,15 @@
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":4
  *     raise TypeError("self._handle cannot be converted to a Python object for pickling")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("self._handle cannot be converted to a Python object for pickling")             # <<<<<<<<<<<<<<
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__26, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__27, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(1, 4, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
@@ -19606,18 +19689,18 @@
     __pyx_t_8 = __Pyx_PyObject_FormatSimple(__pyx_v_function_name, __pyx_empty_unicode); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1579, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __pyx_t_7 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_8) > __pyx_t_7) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_8) : __pyx_t_7;
     __pyx_t_6 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_8);
     __Pyx_GIVEREF(__pyx_t_8);
     PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_8);
     __pyx_t_8 = 0;
-    __Pyx_INCREF(__pyx_kp_u__27);
+    __Pyx_INCREF(__pyx_kp_u__28);
     __pyx_t_6 += 2;
-    __Pyx_GIVEREF(__pyx_kp_u__27);
-    PyTuple_SET_ITEM(__pyx_t_5, 2, __pyx_kp_u__27);
+    __Pyx_GIVEREF(__pyx_kp_u__28);
+    PyTuple_SET_ITEM(__pyx_t_5, 2, __pyx_kp_u__28);
     __pyx_t_8 = __Pyx_PyUnicode_Join(__pyx_t_5, 3, __pyx_t_6, __pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1579, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __pyx_t_5 = NULL;
     __pyx_t_9 = 0;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
@@ -19627,39 +19710,39 @@
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_4, function);
         __pyx_t_9 = 1;
       }
     }
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(__pyx_t_4)) {
-      PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_n_s_metadataLookup, __pyx_t_8};
+      PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_n_u_metadataLookup, __pyx_t_8};
       __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1579, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     } else
     #endif
     #if CYTHON_FAST_PYCCALL
     if (__Pyx_PyFastCFunction_Check(__pyx_t_4)) {
-      PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_n_s_metadataLookup, __pyx_t_8};
+      PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_n_u_metadataLookup, __pyx_t_8};
       __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1579, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     } else
     #endif
     {
       __pyx_t_10 = PyTuple_New(2+__pyx_t_9); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1579, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
       if (__pyx_t_5) {
         __Pyx_GIVEREF(__pyx_t_5); PyTuple_SET_ITEM(__pyx_t_10, 0, __pyx_t_5); __pyx_t_5 = NULL;
       }
-      __Pyx_INCREF(__pyx_n_s_metadataLookup);
-      __Pyx_GIVEREF(__pyx_n_s_metadataLookup);
-      PyTuple_SET_ITEM(__pyx_t_10, 0+__pyx_t_9, __pyx_n_s_metadataLookup);
+      __Pyx_INCREF(__pyx_n_u_metadataLookup);
+      __Pyx_GIVEREF(__pyx_n_u_metadataLookup);
+      PyTuple_SET_ITEM(__pyx_t_10, 0+__pyx_t_9, __pyx_n_u_metadataLookup);
       __Pyx_GIVEREF(__pyx_t_8);
       PyTuple_SET_ITEM(__pyx_t_10, 1+__pyx_t_9, __pyx_t_8);
       __pyx_t_8 = 0;
       __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_10, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1579, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
     }
@@ -19703,15 +19786,15 @@
   /* "pyrfc/_cyrfc.pyx":1583
  *     func_metadata = server_functions[function_name]
  *     # callback = func_metadata['callback']
  *     funcDescHandle[0] = <RFC_FUNCTION_DESC_HANDLE><uintptr_t>func_metadata['func_desc_handle']             # <<<<<<<<<<<<<<
  *     _server_log("metadataLookup", f"Function '{function_name}' handle {<uintptr_t>funcDescHandle[0]}.")
  *     return RFC_OK
  */
-  __pyx_t_4 = __Pyx_PyObject_Dict_GetItem(__pyx_v_func_metadata, __pyx_n_s_func_desc_handle); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1583, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Dict_GetItem(__pyx_v_func_metadata, __pyx_n_u_func_desc_handle); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1583, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_11 = __Pyx_PyInt_As_size_t(__pyx_t_4); if (unlikely((__pyx_t_11 == ((uintptr_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 1583, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   (__pyx_v_funcDescHandle[0]) = ((RFC_FUNCTION_DESC_HANDLE)((uintptr_t)__pyx_t_11));
 
   /* "pyrfc/_cyrfc.pyx":1584
  *     # callback = func_metadata['callback']
@@ -19747,18 +19830,18 @@
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   __pyx_t_7 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_5) > __pyx_t_7) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_5) : __pyx_t_7;
   __pyx_t_6 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_5);
   PyTuple_SET_ITEM(__pyx_t_10, 3, __pyx_t_5);
   __pyx_t_5 = 0;
-  __Pyx_INCREF(__pyx_kp_u__20);
+  __Pyx_INCREF(__pyx_kp_u__21);
   __pyx_t_6 += 1;
-  __Pyx_GIVEREF(__pyx_kp_u__20);
-  PyTuple_SET_ITEM(__pyx_t_10, 4, __pyx_kp_u__20);
+  __Pyx_GIVEREF(__pyx_kp_u__21);
+  PyTuple_SET_ITEM(__pyx_t_10, 4, __pyx_kp_u__21);
   __pyx_t_5 = __Pyx_PyUnicode_Join(__pyx_t_10, 5, __pyx_t_6, __pyx_t_7); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1584, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
   __pyx_t_10 = NULL;
   __pyx_t_9 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
     __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_1);
@@ -19768,39 +19851,39 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_1, function);
       __pyx_t_9 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_1)) {
-    PyObject *__pyx_temp[3] = {__pyx_t_10, __pyx_n_s_metadataLookup, __pyx_t_5};
+    PyObject *__pyx_temp[3] = {__pyx_t_10, __pyx_n_u_metadataLookup, __pyx_t_5};
     __pyx_t_4 = __Pyx_PyFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1584, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_1)) {
-    PyObject *__pyx_temp[3] = {__pyx_t_10, __pyx_n_s_metadataLookup, __pyx_t_5};
+    PyObject *__pyx_temp[3] = {__pyx_t_10, __pyx_n_u_metadataLookup, __pyx_t_5};
     __pyx_t_4 = __Pyx_PyCFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1584, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   } else
   #endif
   {
     __pyx_t_8 = PyTuple_New(2+__pyx_t_9); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1584, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     if (__pyx_t_10) {
       __Pyx_GIVEREF(__pyx_t_10); PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_10); __pyx_t_10 = NULL;
     }
-    __Pyx_INCREF(__pyx_n_s_metadataLookup);
-    __Pyx_GIVEREF(__pyx_n_s_metadataLookup);
-    PyTuple_SET_ITEM(__pyx_t_8, 0+__pyx_t_9, __pyx_n_s_metadataLookup);
+    __Pyx_INCREF(__pyx_n_u_metadataLookup);
+    __Pyx_GIVEREF(__pyx_n_u_metadataLookup);
+    PyTuple_SET_ITEM(__pyx_t_8, 0+__pyx_t_9, __pyx_n_u_metadataLookup);
     __Pyx_GIVEREF(__pyx_t_5);
     PyTuple_SET_ITEM(__pyx_t_8, 1+__pyx_t_9, __pyx_t_5);
     __pyx_t_5 = 0;
     __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_8, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1584, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   }
@@ -19942,27 +20025,27 @@
   }
   __pyx_t_4 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_7, __pyx_t_6) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_6);
   __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1594, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_call_type, __pyx_t_4) < 0) __PYX_ERR(0, 1594, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_call_type, __pyx_t_4) < 0) __PYX_ERR(0, 1594, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
   /* "pyrfc/_cyrfc.pyx":1595
  *     server_context = {
  *         "call_type": UnitCallType(context.type),
  *         "is_stateful": context.isStateful != 0             # <<<<<<<<<<<<<<
  *     }
  *     if context.type != RFC_SYNCHRONOUS:
  */
   __pyx_t_4 = __Pyx_PyBool_FromLong((__pyx_v_context.isStateful != 0)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1595, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_is_stateful, __pyx_t_4) < 0) __PYX_ERR(0, 1594, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_is_stateful, __pyx_t_4) < 0) __PYX_ERR(0, 1594, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_v_server_context = ((PyObject*)__pyx_t_3);
   __pyx_t_3 = 0;
 
   /* "pyrfc/_cyrfc.pyx":1597
  *         "is_stateful": context.isStateful != 0
  *     }
@@ -19978,15 +20061,15 @@
  *     if context.type != RFC_SYNCHRONOUS:
  *         server_context["unit_identifier"] = wrapUnitIdentifier(context.unitIdentifier[0])             # <<<<<<<<<<<<<<
  *     if context.type == RFC_BACKGROUND_UNIT:
  *         server_context ["unit_attributes"] = wrapUnitAttributes(context.unitAttributes)
  */
     __pyx_t_3 = __pyx_f_5pyrfc_6_cyrfc_wrapUnitIdentifier((__pyx_v_context.unitIdentifier[0])); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1598, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    if (unlikely(PyDict_SetItem(__pyx_v_server_context, __pyx_n_s_unit_identifier, __pyx_t_3) < 0)) __PYX_ERR(0, 1598, __pyx_L1_error)
+    if (unlikely(PyDict_SetItem(__pyx_v_server_context, __pyx_n_u_unit_identifier, __pyx_t_3) < 0)) __PYX_ERR(0, 1598, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
     /* "pyrfc/_cyrfc.pyx":1597
  *         "is_stateful": context.isStateful != 0
  *     }
  *     if context.type != RFC_SYNCHRONOUS:             # <<<<<<<<<<<<<<
  *         server_context["unit_identifier"] = wrapUnitIdentifier(context.unitIdentifier[0])
@@ -20009,15 +20092,15 @@
  *     if context.type == RFC_BACKGROUND_UNIT:
  *         server_context ["unit_attributes"] = wrapUnitAttributes(context.unitAttributes)             # <<<<<<<<<<<<<<
  * 
  *     return server_context
  */
     __pyx_t_3 = __pyx_f_5pyrfc_6_cyrfc_wrapUnitAttributes(__pyx_v_context.unitAttributes); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1600, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    if (unlikely(PyDict_SetItem(__pyx_v_server_context, __pyx_n_s_unit_attributes, __pyx_t_3) < 0)) __PYX_ERR(0, 1600, __pyx_L1_error)
+    if (unlikely(PyDict_SetItem(__pyx_v_server_context, __pyx_n_u_unit_attributes, __pyx_t_3) < 0)) __PYX_ERR(0, 1600, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
     /* "pyrfc/_cyrfc.pyx":1599
  *     if context.type != RFC_SYNCHRONOUS:
  *         server_context["unit_identifier"] = wrapUnitIdentifier(context.unitIdentifier[0])
  *     if context.type == RFC_BACKGROUND_UNIT:             # <<<<<<<<<<<<<<
  *         server_context ["unit_attributes"] = wrapUnitAttributes(context.unitAttributes)
@@ -20109,15 +20192,25 @@
   PyObject *__pyx_t_13 = NULL;
   RFC_RC __pyx_t_14;
   Py_ssize_t __pyx_t_15;
   int __pyx_t_16;
   PyObject *__pyx_t_17 = NULL;
   PyObject *__pyx_t_18 = NULL;
   PyObject *__pyx_t_19 = NULL;
-  PyObject *(*__pyx_t_20)(PyObject *);
+  char const *__pyx_t_20;
+  PyObject *__pyx_t_21 = NULL;
+  PyObject *__pyx_t_22 = NULL;
+  PyObject *__pyx_t_23 = NULL;
+  PyObject *__pyx_t_24 = NULL;
+  PyObject *__pyx_t_25 = NULL;
+  PyObject *__pyx_t_26 = NULL;
+  char const *__pyx_t_27;
+  char const *__pyx_t_28;
+  PyObject *(*__pyx_t_29)(PyObject *);
+  char const *__pyx_t_30;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
   #endif
   __Pyx_RefNannySetupContext("genericHandler", 0);
@@ -20356,39 +20449,39 @@
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_1, function);
         __pyx_t_10 = 1;
       }
     }
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(__pyx_t_1)) {
-      PyObject *__pyx_temp[3] = {__pyx_t_7, __pyx_n_s_genericHandler, __pyx_t_9};
+      PyObject *__pyx_temp[3] = {__pyx_t_7, __pyx_n_u_genericHandler, __pyx_t_9};
       __pyx_t_6 = __Pyx_PyFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_10, 2+__pyx_t_10); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1629, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
     } else
     #endif
     #if CYTHON_FAST_PYCCALL
     if (__Pyx_PyFastCFunction_Check(__pyx_t_1)) {
-      PyObject *__pyx_temp[3] = {__pyx_t_7, __pyx_n_s_genericHandler, __pyx_t_9};
+      PyObject *__pyx_temp[3] = {__pyx_t_7, __pyx_n_u_genericHandler, __pyx_t_9};
       __pyx_t_6 = __Pyx_PyCFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_10, 2+__pyx_t_10); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1629, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
     } else
     #endif
     {
       __pyx_t_8 = PyTuple_New(2+__pyx_t_10); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1629, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
       if (__pyx_t_7) {
         __Pyx_GIVEREF(__pyx_t_7); PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_7); __pyx_t_7 = NULL;
       }
-      __Pyx_INCREF(__pyx_n_s_genericHandler);
-      __Pyx_GIVEREF(__pyx_n_s_genericHandler);
-      PyTuple_SET_ITEM(__pyx_t_8, 0+__pyx_t_10, __pyx_n_s_genericHandler);
+      __Pyx_INCREF(__pyx_n_u_genericHandler);
+      __Pyx_GIVEREF(__pyx_n_u_genericHandler);
+      PyTuple_SET_ITEM(__pyx_t_8, 0+__pyx_t_10, __pyx_n_u_genericHandler);
       __Pyx_GIVEREF(__pyx_t_9);
       PyTuple_SET_ITEM(__pyx_t_8, 1+__pyx_t_10, __pyx_t_9);
       __pyx_t_9 = 0;
       __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_8, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1629, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     }
@@ -20432,27 +20525,27 @@
   /* "pyrfc/_cyrfc.pyx":1633
  * 
  *     func_data = server_functions[func_name]
  *     callback = func_data['callback']             # <<<<<<<<<<<<<<
  *     server = func_data['server']
  *     # func_desc = func_data['func_desc_handle']
  */
-  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_func_data, __pyx_n_s_callback); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1633, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_func_data, __pyx_n_u_callback); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1633, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_callback = __pyx_t_1;
   __pyx_t_1 = 0;
 
   /* "pyrfc/_cyrfc.pyx":1634
  *     func_data = server_functions[func_name]
  *     callback = func_data['callback']
  *     server = func_data['server']             # <<<<<<<<<<<<<<
  *     # func_desc = func_data['func_desc_handle']
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_func_data, __pyx_n_s_server); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1634, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_func_data, __pyx_n_u_server); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1634, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_server = __pyx_t_1;
   __pyx_t_1 = 0;
 
   /* "pyrfc/_cyrfc.pyx":1637
  *     # func_desc = func_data['func_desc_handle']
  * 
@@ -20519,18 +20612,18 @@
         __pyx_t_9 = __Pyx_PyUnicode_From_RFC_RC(__pyx_v_rc, 0, ' ', 'd'); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 1640, __pyx_L5_error)
         __Pyx_GOTREF(__pyx_t_9);
         __pyx_t_5 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_9) > __pyx_t_5) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_9) : __pyx_t_5;
         __pyx_t_4 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_9);
         __Pyx_GIVEREF(__pyx_t_9);
         PyTuple_SET_ITEM(__pyx_t_8, 3, __pyx_t_9);
         __pyx_t_9 = 0;
-        __Pyx_INCREF(__pyx_kp_u__28);
+        __Pyx_INCREF(__pyx_kp_u__29);
         __pyx_t_4 += 2;
-        __Pyx_GIVEREF(__pyx_kp_u__28);
-        PyTuple_SET_ITEM(__pyx_t_8, 4, __pyx_kp_u__28);
+        __Pyx_GIVEREF(__pyx_kp_u__29);
+        PyTuple_SET_ITEM(__pyx_t_8, 4, __pyx_kp_u__29);
         __pyx_t_9 = __Pyx_PyUnicode_Join(__pyx_t_8, 5, __pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 1640, __pyx_L5_error)
         __Pyx_GOTREF(__pyx_t_9);
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         __pyx_t_8 = NULL;
         __pyx_t_10 = 0;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_6))) {
           __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_6);
@@ -20540,39 +20633,39 @@
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_6, function);
             __pyx_t_10 = 1;
           }
         }
         #if CYTHON_FAST_PYCALL
         if (PyFunction_Check(__pyx_t_6)) {
-          PyObject *__pyx_temp[3] = {__pyx_t_8, __pyx_n_s_genericHandler, __pyx_t_9};
+          PyObject *__pyx_temp[3] = {__pyx_t_8, __pyx_n_u_genericHandler, __pyx_t_9};
           __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_10, 2+__pyx_t_10); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1640, __pyx_L5_error)
           __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
           __Pyx_GOTREF(__pyx_t_1);
           __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
         } else
         #endif
         #if CYTHON_FAST_PYCCALL
         if (__Pyx_PyFastCFunction_Check(__pyx_t_6)) {
-          PyObject *__pyx_temp[3] = {__pyx_t_8, __pyx_n_s_genericHandler, __pyx_t_9};
+          PyObject *__pyx_temp[3] = {__pyx_t_8, __pyx_n_u_genericHandler, __pyx_t_9};
           __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_10, 2+__pyx_t_10); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1640, __pyx_L5_error)
           __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
           __Pyx_GOTREF(__pyx_t_1);
           __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
         } else
         #endif
         {
           __pyx_t_7 = PyTuple_New(2+__pyx_t_10); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1640, __pyx_L5_error)
           __Pyx_GOTREF(__pyx_t_7);
           if (__pyx_t_8) {
             __Pyx_GIVEREF(__pyx_t_8); PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_8); __pyx_t_8 = NULL;
           }
-          __Pyx_INCREF(__pyx_n_s_genericHandler);
-          __Pyx_GIVEREF(__pyx_n_s_genericHandler);
-          PyTuple_SET_ITEM(__pyx_t_7, 0+__pyx_t_10, __pyx_n_s_genericHandler);
+          __Pyx_INCREF(__pyx_n_u_genericHandler);
+          __Pyx_GIVEREF(__pyx_n_u_genericHandler);
+          PyTuple_SET_ITEM(__pyx_t_7, 0+__pyx_t_10, __pyx_n_u_genericHandler);
           __Pyx_GIVEREF(__pyx_t_9);
           PyTuple_SET_ITEM(__pyx_t_7, 1+__pyx_t_10, __pyx_t_9);
           __pyx_t_9 = 0;
           __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1640, __pyx_L5_error)
           __Pyx_GOTREF(__pyx_t_1);
           __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
         }
@@ -20600,15 +20693,15 @@
  *             conn_attr = {}
  *         else:
  */
           __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_ExternalRuntimeError); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1642, __pyx_L5_error)
           __Pyx_GOTREF(__pyx_t_1);
           __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1642, __pyx_L5_error)
           __Pyx_GOTREF(__pyx_t_6);
-          if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_message, __pyx_kp_s_Invalid_connection_handle) < 0) __PYX_ERR(0, 1642, __pyx_L5_error)
+          if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_message, __pyx_kp_u_Invalid_connection_handle) < 0) __PYX_ERR(0, 1642, __pyx_L5_error)
           __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_empty_tuple, __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1642, __pyx_L5_error)
           __Pyx_GOTREF(__pyx_t_7);
           __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
           __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
           __Pyx_Raise(__pyx_t_7, 0, 0, 0);
           __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
           __PYX_ERR(0, 1642, __pyx_L5_error)
@@ -20670,15 +20763,15 @@
         /* "pyrfc/_cyrfc.pyx":1649
  *                 "genericHandler",
  *                 "User '{user}' from system '{sysId}' client '{client}' host '{partnerHost}' invokes '{func_name}'"
  *                 .format(func_name=func_name, **conn_attr)             # <<<<<<<<<<<<<<
  *             )
  * 
  */
-        __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_kp_s_User_user_from_system_sysId_clie, __pyx_n_s_format); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1649, __pyx_L5_error)
+        __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_User_user_from_system_sysId_clie, __pyx_n_s_format); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1649, __pyx_L5_error)
         __Pyx_GOTREF(__pyx_t_1);
         __pyx_t_8 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1649, __pyx_L5_error)
         __Pyx_GOTREF(__pyx_t_8);
         if (PyDict_SetItem(__pyx_t_8, __pyx_n_s_func_name, __pyx_v_func_name) < 0) __PYX_ERR(0, 1649, __pyx_L5_error)
         __pyx_t_9 = __pyx_t_8;
         __pyx_t_8 = 0;
         if (unlikely(__pyx_v_conn_attr == Py_None)) {
@@ -20700,39 +20793,39 @@
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_6, function);
             __pyx_t_10 = 1;
           }
         }
         #if CYTHON_FAST_PYCALL
         if (PyFunction_Check(__pyx_t_6)) {
-          PyObject *__pyx_temp[3] = {__pyx_t_9, __pyx_n_s_genericHandler, __pyx_t_8};
+          PyObject *__pyx_temp[3] = {__pyx_t_9, __pyx_n_u_genericHandler, __pyx_t_8};
           __pyx_t_7 = __Pyx_PyFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_10, 2+__pyx_t_10); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1646, __pyx_L5_error)
           __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
           __Pyx_GOTREF(__pyx_t_7);
           __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         } else
         #endif
         #if CYTHON_FAST_PYCCALL
         if (__Pyx_PyFastCFunction_Check(__pyx_t_6)) {
-          PyObject *__pyx_temp[3] = {__pyx_t_9, __pyx_n_s_genericHandler, __pyx_t_8};
+          PyObject *__pyx_temp[3] = {__pyx_t_9, __pyx_n_u_genericHandler, __pyx_t_8};
           __pyx_t_7 = __Pyx_PyCFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_10, 2+__pyx_t_10); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1646, __pyx_L5_error)
           __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
           __Pyx_GOTREF(__pyx_t_7);
           __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         } else
         #endif
         {
           __pyx_t_1 = PyTuple_New(2+__pyx_t_10); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1646, __pyx_L5_error)
           __Pyx_GOTREF(__pyx_t_1);
           if (__pyx_t_9) {
             __Pyx_GIVEREF(__pyx_t_9); PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_9); __pyx_t_9 = NULL;
           }
-          __Pyx_INCREF(__pyx_n_s_genericHandler);
-          __Pyx_GIVEREF(__pyx_n_s_genericHandler);
-          PyTuple_SET_ITEM(__pyx_t_1, 0+__pyx_t_10, __pyx_n_s_genericHandler);
+          __Pyx_INCREF(__pyx_n_u_genericHandler);
+          __Pyx_GIVEREF(__pyx_n_u_genericHandler);
+          PyTuple_SET_ITEM(__pyx_t_1, 0+__pyx_t_10, __pyx_n_u_genericHandler);
           __Pyx_GIVEREF(__pyx_t_8);
           PyTuple_SET_ITEM(__pyx_t_1, 1+__pyx_t_10, __pyx_t_8);
           __pyx_t_8 = 0;
           __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_1, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1646, __pyx_L5_error)
           __Pyx_GOTREF(__pyx_t_7);
           __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         }
@@ -20746,37 +20839,37 @@
  *         request_context = {
  *             'connection_attributes': conn_attr,             # <<<<<<<<<<<<<<
  *             'server_context': context
  *         }
  */
       __pyx_t_7 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1654, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_7);
-      if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_connection_attributes, __pyx_v_conn_attr) < 0) __PYX_ERR(0, 1654, __pyx_L5_error)
+      if (PyDict_SetItem(__pyx_t_7, __pyx_n_u_connection_attributes, __pyx_v_conn_attr) < 0) __PYX_ERR(0, 1654, __pyx_L5_error)
 
       /* "pyrfc/_cyrfc.pyx":1655
  *         request_context = {
  *             'connection_attributes': conn_attr,
  *             'server_context': context             # <<<<<<<<<<<<<<
  *         }
  * 
  */
-      if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_server_context, __pyx_v_context) < 0) __PYX_ERR(0, 1654, __pyx_L5_error)
+      if (PyDict_SetItem(__pyx_t_7, __pyx_n_u_server_context, __pyx_v_context) < 0) __PYX_ERR(0, 1654, __pyx_L5_error)
       __pyx_v_request_context = ((PyObject*)__pyx_t_7);
       __pyx_t_7 = 0;
 
       /* "pyrfc/_cyrfc.pyx":1659
  * 
  *         # Authorization check
  *         auth_function = server_context["auth_check"]             # <<<<<<<<<<<<<<
  *         rc = auth_function(func_name, request_context)
  *         if rc != RFC_OK:
  */
       __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_server_context); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1659, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_7);
-      __pyx_t_6 = __Pyx_PyObject_Dict_GetItem(__pyx_t_7, __pyx_n_s_auth_check); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1659, __pyx_L5_error)
+      __pyx_t_6 = __Pyx_PyObject_Dict_GetItem(__pyx_t_7, __pyx_n_u_auth_check); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1659, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       __pyx_v_auth_function = __pyx_t_6;
       __pyx_t_6 = 0;
 
       /* "pyrfc/_cyrfc.pyx":1660
  *         # Authorization check
@@ -20993,15 +21086,15 @@
       /* "pyrfc/_cyrfc.pyx":1677
  * 
  *         # Return results
  *         if context["call_type"] != UnitCallType.background_unit:             # <<<<<<<<<<<<<<
  *             for name, value in result.iteritems():
  *                 fillFunctionParameter(funcDesc, funcHandle, name, value)
  */
-      __pyx_t_6 = __Pyx_PyObject_Dict_GetItem(__pyx_v_context, __pyx_n_s_call_type); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1677, __pyx_L5_error)
+      __pyx_t_6 = __Pyx_PyObject_Dict_GetItem(__pyx_v_context, __pyx_n_u_call_type); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1677, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_UnitCallType); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1677, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_1);
       __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_background_unit); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1677, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __pyx_t_1 = PyObject_RichCompare(__pyx_t_6, __pyx_t_7, Py_NE); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1677, __pyx_L5_error)
@@ -21098,286 +21191,398 @@
       __Pyx_AddTraceback("pyrfc._cyrfc.genericHandler", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_7, &__pyx_t_6, &__pyx_t_1) < 0) __PYX_ERR(0, 1683, __pyx_L7_except_error)
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_INCREF(__pyx_t_6);
       __pyx_v_e = __pyx_t_6;
+      /*try:*/ {
 
-      /* "pyrfc/_cyrfc.pyx":1686
+        /* "pyrfc/_cyrfc.pyx":1686
  *         # Parameter: message (optional: msg_type, msg_class, msg_number, msg_v1-v4)
  *         # returns:   RFC_EXTERNAL_FAILURE
  *         fillError(e, serverErrorInfo)             # <<<<<<<<<<<<<<
  *         serverErrorInfo.code = RFC_EXTERNAL_FAILURE  # Overwrite code, if set.
  *         _server_log("genericHandler", f"Request for '{func_name}' raises ExternalRuntimeError {e} - code set to RFC_EXTERNAL_FAILURE.")
  */
-      __pyx_t_8 = __pyx_f_5pyrfc_6_cyrfc_fillError(__pyx_v_e, __pyx_v_serverErrorInfo); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1686, __pyx_L7_except_error)
-      __Pyx_GOTREF(__pyx_t_8);
-      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+        __pyx_t_8 = __pyx_f_5pyrfc_6_cyrfc_fillError(__pyx_v_e, __pyx_v_serverErrorInfo); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1686, __pyx_L22_error)
+        __Pyx_GOTREF(__pyx_t_8);
+        __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-      /* "pyrfc/_cyrfc.pyx":1687
+        /* "pyrfc/_cyrfc.pyx":1687
  *         # returns:   RFC_EXTERNAL_FAILURE
  *         fillError(e, serverErrorInfo)
  *         serverErrorInfo.code = RFC_EXTERNAL_FAILURE  # Overwrite code, if set.             # <<<<<<<<<<<<<<
  *         _server_log("genericHandler", f"Request for '{func_name}' raises ExternalRuntimeError {e} - code set to RFC_EXTERNAL_FAILURE.")
  *         return RFC_EXTERNAL_FAILURE
  */
-      __pyx_v_serverErrorInfo->code = RFC_EXTERNAL_FAILURE;
+        __pyx_v_serverErrorInfo->code = RFC_EXTERNAL_FAILURE;
 
-      /* "pyrfc/_cyrfc.pyx":1688
+        /* "pyrfc/_cyrfc.pyx":1688
  *         fillError(e, serverErrorInfo)
  *         serverErrorInfo.code = RFC_EXTERNAL_FAILURE  # Overwrite code, if set.
  *         _server_log("genericHandler", f"Request for '{func_name}' raises ExternalRuntimeError {e} - code set to RFC_EXTERNAL_FAILURE.")             # <<<<<<<<<<<<<<
  *         return RFC_EXTERNAL_FAILURE
  *     except ABAPRuntimeError as e:  # ABAP Message
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_server_log); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 1688, __pyx_L7_except_error)
-      __Pyx_GOTREF(__pyx_t_9);
-      __pyx_t_17 = PyTuple_New(5); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 1688, __pyx_L7_except_error)
-      __Pyx_GOTREF(__pyx_t_17);
-      __pyx_t_15 = 0;
-      __pyx_t_5 = 127;
-      __Pyx_INCREF(__pyx_kp_u_Request_for);
-      __pyx_t_15 += 13;
-      __Pyx_GIVEREF(__pyx_kp_u_Request_for);
-      PyTuple_SET_ITEM(__pyx_t_17, 0, __pyx_kp_u_Request_for);
-      __pyx_t_18 = __Pyx_PyObject_FormatSimple(__pyx_v_func_name, __pyx_empty_unicode); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 1688, __pyx_L7_except_error)
-      __Pyx_GOTREF(__pyx_t_18);
-      __pyx_t_5 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_18) > __pyx_t_5) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_18) : __pyx_t_5;
-      __pyx_t_15 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_18);
-      __Pyx_GIVEREF(__pyx_t_18);
-      PyTuple_SET_ITEM(__pyx_t_17, 1, __pyx_t_18);
-      __pyx_t_18 = 0;
-      __Pyx_INCREF(__pyx_kp_u_raises_ExternalRuntimeError);
-      __pyx_t_15 += 30;
-      __Pyx_GIVEREF(__pyx_kp_u_raises_ExternalRuntimeError);
-      PyTuple_SET_ITEM(__pyx_t_17, 2, __pyx_kp_u_raises_ExternalRuntimeError);
-      __pyx_t_18 = __Pyx_PyObject_FormatSimple(__pyx_v_e, __pyx_empty_unicode); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 1688, __pyx_L7_except_error)
-      __Pyx_GOTREF(__pyx_t_18);
-      __pyx_t_5 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_18) > __pyx_t_5) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_18) : __pyx_t_5;
-      __pyx_t_15 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_18);
-      __Pyx_GIVEREF(__pyx_t_18);
-      PyTuple_SET_ITEM(__pyx_t_17, 3, __pyx_t_18);
-      __pyx_t_18 = 0;
-      __Pyx_INCREF(__pyx_kp_u_code_set_to_RFC_EXTERNAL_FAILUR);
-      __pyx_t_15 += 36;
-      __Pyx_GIVEREF(__pyx_kp_u_code_set_to_RFC_EXTERNAL_FAILUR);
-      PyTuple_SET_ITEM(__pyx_t_17, 4, __pyx_kp_u_code_set_to_RFC_EXTERNAL_FAILUR);
-      __pyx_t_18 = __Pyx_PyUnicode_Join(__pyx_t_17, 5, __pyx_t_15, __pyx_t_5); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 1688, __pyx_L7_except_error)
-      __Pyx_GOTREF(__pyx_t_18);
-      __Pyx_DECREF(__pyx_t_17); __pyx_t_17 = 0;
-      __pyx_t_17 = NULL;
-      __pyx_t_10 = 0;
-      if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_9))) {
-        __pyx_t_17 = PyMethod_GET_SELF(__pyx_t_9);
-        if (likely(__pyx_t_17)) {
-          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_9);
-          __Pyx_INCREF(__pyx_t_17);
-          __Pyx_INCREF(function);
-          __Pyx_DECREF_SET(__pyx_t_9, function);
-          __pyx_t_10 = 1;
-        }
-      }
-      #if CYTHON_FAST_PYCALL
-      if (PyFunction_Check(__pyx_t_9)) {
-        PyObject *__pyx_temp[3] = {__pyx_t_17, __pyx_n_s_genericHandler, __pyx_t_18};
-        __pyx_t_8 = __Pyx_PyFunction_FastCall(__pyx_t_9, __pyx_temp+1-__pyx_t_10, 2+__pyx_t_10); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1688, __pyx_L7_except_error)
-        __Pyx_XDECREF(__pyx_t_17); __pyx_t_17 = 0;
-        __Pyx_GOTREF(__pyx_t_8);
-        __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
-      } else
-      #endif
-      #if CYTHON_FAST_PYCCALL
-      if (__Pyx_PyFastCFunction_Check(__pyx_t_9)) {
-        PyObject *__pyx_temp[3] = {__pyx_t_17, __pyx_n_s_genericHandler, __pyx_t_18};
-        __pyx_t_8 = __Pyx_PyCFunction_FastCall(__pyx_t_9, __pyx_temp+1-__pyx_t_10, 2+__pyx_t_10); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1688, __pyx_L7_except_error)
-        __Pyx_XDECREF(__pyx_t_17); __pyx_t_17 = 0;
-        __Pyx_GOTREF(__pyx_t_8);
-        __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
-      } else
-      #endif
-      {
-        __pyx_t_19 = PyTuple_New(2+__pyx_t_10); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 1688, __pyx_L7_except_error)
-        __Pyx_GOTREF(__pyx_t_19);
-        if (__pyx_t_17) {
-          __Pyx_GIVEREF(__pyx_t_17); PyTuple_SET_ITEM(__pyx_t_19, 0, __pyx_t_17); __pyx_t_17 = NULL;
-        }
-        __Pyx_INCREF(__pyx_n_s_genericHandler);
-        __Pyx_GIVEREF(__pyx_n_s_genericHandler);
-        PyTuple_SET_ITEM(__pyx_t_19, 0+__pyx_t_10, __pyx_n_s_genericHandler);
+        __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_server_log); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 1688, __pyx_L22_error)
+        __Pyx_GOTREF(__pyx_t_9);
+        __pyx_t_17 = PyTuple_New(5); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 1688, __pyx_L22_error)
+        __Pyx_GOTREF(__pyx_t_17);
+        __pyx_t_15 = 0;
+        __pyx_t_5 = 127;
+        __Pyx_INCREF(__pyx_kp_u_Request_for);
+        __pyx_t_15 += 13;
+        __Pyx_GIVEREF(__pyx_kp_u_Request_for);
+        PyTuple_SET_ITEM(__pyx_t_17, 0, __pyx_kp_u_Request_for);
+        __pyx_t_18 = __Pyx_PyObject_FormatSimple(__pyx_v_func_name, __pyx_empty_unicode); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 1688, __pyx_L22_error)
+        __Pyx_GOTREF(__pyx_t_18);
+        __pyx_t_5 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_18) > __pyx_t_5) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_18) : __pyx_t_5;
+        __pyx_t_15 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_18);
         __Pyx_GIVEREF(__pyx_t_18);
-        PyTuple_SET_ITEM(__pyx_t_19, 1+__pyx_t_10, __pyx_t_18);
+        PyTuple_SET_ITEM(__pyx_t_17, 1, __pyx_t_18);
         __pyx_t_18 = 0;
-        __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_9, __pyx_t_19, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1688, __pyx_L7_except_error)
-        __Pyx_GOTREF(__pyx_t_8);
-        __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
-      }
-      __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+        __Pyx_INCREF(__pyx_kp_u_raises_ExternalRuntimeError);
+        __pyx_t_15 += 30;
+        __Pyx_GIVEREF(__pyx_kp_u_raises_ExternalRuntimeError);
+        PyTuple_SET_ITEM(__pyx_t_17, 2, __pyx_kp_u_raises_ExternalRuntimeError);
+        __pyx_t_18 = __Pyx_PyObject_FormatSimple(__pyx_v_e, __pyx_empty_unicode); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 1688, __pyx_L22_error)
+        __Pyx_GOTREF(__pyx_t_18);
+        __pyx_t_5 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_18) > __pyx_t_5) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_18) : __pyx_t_5;
+        __pyx_t_15 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_18);
+        __Pyx_GIVEREF(__pyx_t_18);
+        PyTuple_SET_ITEM(__pyx_t_17, 3, __pyx_t_18);
+        __pyx_t_18 = 0;
+        __Pyx_INCREF(__pyx_kp_u_code_set_to_RFC_EXTERNAL_FAILUR);
+        __pyx_t_15 += 36;
+        __Pyx_GIVEREF(__pyx_kp_u_code_set_to_RFC_EXTERNAL_FAILUR);
+        PyTuple_SET_ITEM(__pyx_t_17, 4, __pyx_kp_u_code_set_to_RFC_EXTERNAL_FAILUR);
+        __pyx_t_18 = __Pyx_PyUnicode_Join(__pyx_t_17, 5, __pyx_t_15, __pyx_t_5); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 1688, __pyx_L22_error)
+        __Pyx_GOTREF(__pyx_t_18);
+        __Pyx_DECREF(__pyx_t_17); __pyx_t_17 = 0;
+        __pyx_t_17 = NULL;
+        __pyx_t_10 = 0;
+        if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_9))) {
+          __pyx_t_17 = PyMethod_GET_SELF(__pyx_t_9);
+          if (likely(__pyx_t_17)) {
+            PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_9);
+            __Pyx_INCREF(__pyx_t_17);
+            __Pyx_INCREF(function);
+            __Pyx_DECREF_SET(__pyx_t_9, function);
+            __pyx_t_10 = 1;
+          }
+        }
+        #if CYTHON_FAST_PYCALL
+        if (PyFunction_Check(__pyx_t_9)) {
+          PyObject *__pyx_temp[3] = {__pyx_t_17, __pyx_n_u_genericHandler, __pyx_t_18};
+          __pyx_t_8 = __Pyx_PyFunction_FastCall(__pyx_t_9, __pyx_temp+1-__pyx_t_10, 2+__pyx_t_10); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1688, __pyx_L22_error)
+          __Pyx_XDECREF(__pyx_t_17); __pyx_t_17 = 0;
+          __Pyx_GOTREF(__pyx_t_8);
+          __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
+        } else
+        #endif
+        #if CYTHON_FAST_PYCCALL
+        if (__Pyx_PyFastCFunction_Check(__pyx_t_9)) {
+          PyObject *__pyx_temp[3] = {__pyx_t_17, __pyx_n_u_genericHandler, __pyx_t_18};
+          __pyx_t_8 = __Pyx_PyCFunction_FastCall(__pyx_t_9, __pyx_temp+1-__pyx_t_10, 2+__pyx_t_10); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1688, __pyx_L22_error)
+          __Pyx_XDECREF(__pyx_t_17); __pyx_t_17 = 0;
+          __Pyx_GOTREF(__pyx_t_8);
+          __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
+        } else
+        #endif
+        {
+          __pyx_t_19 = PyTuple_New(2+__pyx_t_10); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 1688, __pyx_L22_error)
+          __Pyx_GOTREF(__pyx_t_19);
+          if (__pyx_t_17) {
+            __Pyx_GIVEREF(__pyx_t_17); PyTuple_SET_ITEM(__pyx_t_19, 0, __pyx_t_17); __pyx_t_17 = NULL;
+          }
+          __Pyx_INCREF(__pyx_n_u_genericHandler);
+          __Pyx_GIVEREF(__pyx_n_u_genericHandler);
+          PyTuple_SET_ITEM(__pyx_t_19, 0+__pyx_t_10, __pyx_n_u_genericHandler);
+          __Pyx_GIVEREF(__pyx_t_18);
+          PyTuple_SET_ITEM(__pyx_t_19, 1+__pyx_t_10, __pyx_t_18);
+          __pyx_t_18 = 0;
+          __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_9, __pyx_t_19, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1688, __pyx_L22_error)
+          __Pyx_GOTREF(__pyx_t_8);
+          __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
+        }
+        __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+        __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-      /* "pyrfc/_cyrfc.pyx":1689
+        /* "pyrfc/_cyrfc.pyx":1689
  *         serverErrorInfo.code = RFC_EXTERNAL_FAILURE  # Overwrite code, if set.
  *         _server_log("genericHandler", f"Request for '{func_name}' raises ExternalRuntimeError {e} - code set to RFC_EXTERNAL_FAILURE.")
  *         return RFC_EXTERNAL_FAILURE             # <<<<<<<<<<<<<<
  *     except ABAPRuntimeError as e:  # ABAP Message
  *         # Parameter: msg_type, msg_class, msg_number, msg_v1-v4
  */
-      __pyx_r = RFC_EXTERNAL_FAILURE;
-      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-      goto __pyx_L8_except_return;
+        __pyx_r = RFC_EXTERNAL_FAILURE;
+        __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+        __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+        __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+        goto __pyx_L21_return;
+      }
+
+      /* "pyrfc/_cyrfc.pyx":1683
+ *     # Server exception handling: cf. SAP NetWeaver RFC SDK 7.50
+ *     # 5.1 Preparing a Server Program for Receiving RFC Requests
+ *     except ExternalRuntimeError as e:  # System failure             # <<<<<<<<<<<<<<
+ *         # Parameter: message (optional: msg_type, msg_class, msg_number, msg_v1-v4)
+ *         # returns:   RFC_EXTERNAL_FAILURE
+ */
+      /*finally:*/ {
+        __pyx_L22_error:;
+        /*exception exit:*/{
+          __Pyx_PyThreadState_declare
+          __Pyx_PyThreadState_assign
+          __pyx_t_21 = 0; __pyx_t_22 = 0; __pyx_t_23 = 0; __pyx_t_24 = 0; __pyx_t_25 = 0; __pyx_t_26 = 0;
+          __Pyx_XDECREF(__pyx_t_17); __pyx_t_17 = 0;
+          __Pyx_XDECREF(__pyx_t_18); __pyx_t_18 = 0;
+          __Pyx_XDECREF(__pyx_t_19); __pyx_t_19 = 0;
+          __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
+          __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
+          if (PY_MAJOR_VERSION >= 3) __Pyx_ExceptionSwap(&__pyx_t_24, &__pyx_t_25, &__pyx_t_26);
+          if ((PY_MAJOR_VERSION < 3) || unlikely(__Pyx_GetException(&__pyx_t_21, &__pyx_t_22, &__pyx_t_23) < 0)) __Pyx_ErrFetch(&__pyx_t_21, &__pyx_t_22, &__pyx_t_23);
+          __Pyx_XGOTREF(__pyx_t_21);
+          __Pyx_XGOTREF(__pyx_t_22);
+          __Pyx_XGOTREF(__pyx_t_23);
+          __Pyx_XGOTREF(__pyx_t_24);
+          __Pyx_XGOTREF(__pyx_t_25);
+          __Pyx_XGOTREF(__pyx_t_26);
+          __pyx_t_10 = __pyx_lineno; __pyx_t_16 = __pyx_clineno; __pyx_t_20 = __pyx_filename;
+          {
+            __Pyx_DECREF(__pyx_v_e);
+            __pyx_v_e = NULL;
+          }
+          if (PY_MAJOR_VERSION >= 3) {
+            __Pyx_XGIVEREF(__pyx_t_24);
+            __Pyx_XGIVEREF(__pyx_t_25);
+            __Pyx_XGIVEREF(__pyx_t_26);
+            __Pyx_ExceptionReset(__pyx_t_24, __pyx_t_25, __pyx_t_26);
+          }
+          __Pyx_XGIVEREF(__pyx_t_21);
+          __Pyx_XGIVEREF(__pyx_t_22);
+          __Pyx_XGIVEREF(__pyx_t_23);
+          __Pyx_ErrRestore(__pyx_t_21, __pyx_t_22, __pyx_t_23);
+          __pyx_t_21 = 0; __pyx_t_22 = 0; __pyx_t_23 = 0; __pyx_t_24 = 0; __pyx_t_25 = 0; __pyx_t_26 = 0;
+          __pyx_lineno = __pyx_t_10; __pyx_clineno = __pyx_t_16; __pyx_filename = __pyx_t_20;
+          goto __pyx_L7_except_error;
+        }
+        __pyx_L21_return: {
+          __pyx_t_14 = __pyx_r;
+          __Pyx_DECREF(__pyx_v_e);
+          __pyx_v_e = NULL;
+          __pyx_r = __pyx_t_14;
+          goto __pyx_L8_except_return;
+        }
+      }
     }
 
     /* "pyrfc/_cyrfc.pyx":1690
  *         _server_log("genericHandler", f"Request for '{func_name}' raises ExternalRuntimeError {e} - code set to RFC_EXTERNAL_FAILURE.")
  *         return RFC_EXTERNAL_FAILURE
  *     except ABAPRuntimeError as e:  # ABAP Message             # <<<<<<<<<<<<<<
  *         # Parameter: msg_type, msg_class, msg_number, msg_v1-v4
  *         # returns:   RFC_ABAP_MESSAGE
  */
     __Pyx_ErrFetch(&__pyx_t_1, &__pyx_t_6, &__pyx_t_7);
     __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_ABAPRuntimeError); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1690, __pyx_L7_except_error)
     __Pyx_GOTREF(__pyx_t_8);
-    __pyx_t_10 = __Pyx_PyErr_GivenExceptionMatches(__pyx_t_1, __pyx_t_8);
+    __pyx_t_16 = __Pyx_PyErr_GivenExceptionMatches(__pyx_t_1, __pyx_t_8);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     __Pyx_ErrRestore(__pyx_t_1, __pyx_t_6, __pyx_t_7);
     __pyx_t_1 = 0; __pyx_t_6 = 0; __pyx_t_7 = 0;
-    if (__pyx_t_10) {
+    if (__pyx_t_16) {
       __Pyx_AddTraceback("pyrfc._cyrfc.genericHandler", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_7, &__pyx_t_6, &__pyx_t_1) < 0) __PYX_ERR(0, 1690, __pyx_L7_except_error)
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_INCREF(__pyx_t_6);
       __pyx_v_e = __pyx_t_6;
+      /*try:*/ {
 
-      /* "pyrfc/_cyrfc.pyx":1693
+        /* "pyrfc/_cyrfc.pyx":1693
  *         # Parameter: msg_type, msg_class, msg_number, msg_v1-v4
  *         # returns:   RFC_ABAP_MESSAGE
  *         fillError(e, serverErrorInfo)             # <<<<<<<<<<<<<<
  *         serverErrorInfo.code = RFC_ABAP_MESSAGE  # Overwrite code, if set.
  *         _server_log("genericHandler", f"Request for '{func_name}' raises ABAPRuntimeError {e} - code set to RFC_ABAP_MESSAGE.")
  */
-      __pyx_t_8 = __pyx_f_5pyrfc_6_cyrfc_fillError(__pyx_v_e, __pyx_v_serverErrorInfo); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1693, __pyx_L7_except_error)
-      __Pyx_GOTREF(__pyx_t_8);
-      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+        __pyx_t_8 = __pyx_f_5pyrfc_6_cyrfc_fillError(__pyx_v_e, __pyx_v_serverErrorInfo); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1693, __pyx_L33_error)
+        __Pyx_GOTREF(__pyx_t_8);
+        __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-      /* "pyrfc/_cyrfc.pyx":1694
+        /* "pyrfc/_cyrfc.pyx":1694
  *         # returns:   RFC_ABAP_MESSAGE
  *         fillError(e, serverErrorInfo)
  *         serverErrorInfo.code = RFC_ABAP_MESSAGE  # Overwrite code, if set.             # <<<<<<<<<<<<<<
  *         _server_log("genericHandler", f"Request for '{func_name}' raises ABAPRuntimeError {e} - code set to RFC_ABAP_MESSAGE.")
  *         return RFC_ABAP_MESSAGE
  */
-      __pyx_v_serverErrorInfo->code = RFC_ABAP_MESSAGE;
+        __pyx_v_serverErrorInfo->code = RFC_ABAP_MESSAGE;
 
-      /* "pyrfc/_cyrfc.pyx":1695
+        /* "pyrfc/_cyrfc.pyx":1695
  *         fillError(e, serverErrorInfo)
  *         serverErrorInfo.code = RFC_ABAP_MESSAGE  # Overwrite code, if set.
  *         _server_log("genericHandler", f"Request for '{func_name}' raises ABAPRuntimeError {e} - code set to RFC_ABAP_MESSAGE.")             # <<<<<<<<<<<<<<
  *         return RFC_ABAP_MESSAGE
  *     except ABAPApplicationError as e:  # ABAP Exception in implementing function
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_server_log); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 1695, __pyx_L7_except_error)
-      __Pyx_GOTREF(__pyx_t_9);
-      __pyx_t_19 = PyTuple_New(5); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 1695, __pyx_L7_except_error)
-      __Pyx_GOTREF(__pyx_t_19);
-      __pyx_t_15 = 0;
-      __pyx_t_5 = 127;
-      __Pyx_INCREF(__pyx_kp_u_Request_for);
-      __pyx_t_15 += 13;
-      __Pyx_GIVEREF(__pyx_kp_u_Request_for);
-      PyTuple_SET_ITEM(__pyx_t_19, 0, __pyx_kp_u_Request_for);
-      __pyx_t_18 = __Pyx_PyObject_FormatSimple(__pyx_v_func_name, __pyx_empty_unicode); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 1695, __pyx_L7_except_error)
-      __Pyx_GOTREF(__pyx_t_18);
-      __pyx_t_5 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_18) > __pyx_t_5) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_18) : __pyx_t_5;
-      __pyx_t_15 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_18);
-      __Pyx_GIVEREF(__pyx_t_18);
-      PyTuple_SET_ITEM(__pyx_t_19, 1, __pyx_t_18);
-      __pyx_t_18 = 0;
-      __Pyx_INCREF(__pyx_kp_u_raises_ABAPRuntimeError);
-      __pyx_t_15 += 26;
-      __Pyx_GIVEREF(__pyx_kp_u_raises_ABAPRuntimeError);
-      PyTuple_SET_ITEM(__pyx_t_19, 2, __pyx_kp_u_raises_ABAPRuntimeError);
-      __pyx_t_18 = __Pyx_PyObject_FormatSimple(__pyx_v_e, __pyx_empty_unicode); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 1695, __pyx_L7_except_error)
-      __Pyx_GOTREF(__pyx_t_18);
-      __pyx_t_5 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_18) > __pyx_t_5) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_18) : __pyx_t_5;
-      __pyx_t_15 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_18);
-      __Pyx_GIVEREF(__pyx_t_18);
-      PyTuple_SET_ITEM(__pyx_t_19, 3, __pyx_t_18);
-      __pyx_t_18 = 0;
-      __Pyx_INCREF(__pyx_kp_u_code_set_to_RFC_ABAP_MESSAGE);
-      __pyx_t_15 += 32;
-      __Pyx_GIVEREF(__pyx_kp_u_code_set_to_RFC_ABAP_MESSAGE);
-      PyTuple_SET_ITEM(__pyx_t_19, 4, __pyx_kp_u_code_set_to_RFC_ABAP_MESSAGE);
-      __pyx_t_18 = __Pyx_PyUnicode_Join(__pyx_t_19, 5, __pyx_t_15, __pyx_t_5); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 1695, __pyx_L7_except_error)
-      __Pyx_GOTREF(__pyx_t_18);
-      __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
-      __pyx_t_19 = NULL;
-      __pyx_t_10 = 0;
-      if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_9))) {
-        __pyx_t_19 = PyMethod_GET_SELF(__pyx_t_9);
-        if (likely(__pyx_t_19)) {
-          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_9);
-          __Pyx_INCREF(__pyx_t_19);
-          __Pyx_INCREF(function);
-          __Pyx_DECREF_SET(__pyx_t_9, function);
-          __pyx_t_10 = 1;
-        }
-      }
-      #if CYTHON_FAST_PYCALL
-      if (PyFunction_Check(__pyx_t_9)) {
-        PyObject *__pyx_temp[3] = {__pyx_t_19, __pyx_n_s_genericHandler, __pyx_t_18};
-        __pyx_t_8 = __Pyx_PyFunction_FastCall(__pyx_t_9, __pyx_temp+1-__pyx_t_10, 2+__pyx_t_10); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1695, __pyx_L7_except_error)
-        __Pyx_XDECREF(__pyx_t_19); __pyx_t_19 = 0;
-        __Pyx_GOTREF(__pyx_t_8);
-        __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
-      } else
-      #endif
-      #if CYTHON_FAST_PYCCALL
-      if (__Pyx_PyFastCFunction_Check(__pyx_t_9)) {
-        PyObject *__pyx_temp[3] = {__pyx_t_19, __pyx_n_s_genericHandler, __pyx_t_18};
-        __pyx_t_8 = __Pyx_PyCFunction_FastCall(__pyx_t_9, __pyx_temp+1-__pyx_t_10, 2+__pyx_t_10); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1695, __pyx_L7_except_error)
-        __Pyx_XDECREF(__pyx_t_19); __pyx_t_19 = 0;
-        __Pyx_GOTREF(__pyx_t_8);
-        __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
-      } else
-      #endif
-      {
-        __pyx_t_17 = PyTuple_New(2+__pyx_t_10); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 1695, __pyx_L7_except_error)
-        __Pyx_GOTREF(__pyx_t_17);
-        if (__pyx_t_19) {
-          __Pyx_GIVEREF(__pyx_t_19); PyTuple_SET_ITEM(__pyx_t_17, 0, __pyx_t_19); __pyx_t_19 = NULL;
-        }
-        __Pyx_INCREF(__pyx_n_s_genericHandler);
-        __Pyx_GIVEREF(__pyx_n_s_genericHandler);
-        PyTuple_SET_ITEM(__pyx_t_17, 0+__pyx_t_10, __pyx_n_s_genericHandler);
+        __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_server_log); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 1695, __pyx_L33_error)
+        __Pyx_GOTREF(__pyx_t_9);
+        __pyx_t_19 = PyTuple_New(5); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 1695, __pyx_L33_error)
+        __Pyx_GOTREF(__pyx_t_19);
+        __pyx_t_15 = 0;
+        __pyx_t_5 = 127;
+        __Pyx_INCREF(__pyx_kp_u_Request_for);
+        __pyx_t_15 += 13;
+        __Pyx_GIVEREF(__pyx_kp_u_Request_for);
+        PyTuple_SET_ITEM(__pyx_t_19, 0, __pyx_kp_u_Request_for);
+        __pyx_t_18 = __Pyx_PyObject_FormatSimple(__pyx_v_func_name, __pyx_empty_unicode); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 1695, __pyx_L33_error)
+        __Pyx_GOTREF(__pyx_t_18);
+        __pyx_t_5 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_18) > __pyx_t_5) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_18) : __pyx_t_5;
+        __pyx_t_15 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_18);
         __Pyx_GIVEREF(__pyx_t_18);
-        PyTuple_SET_ITEM(__pyx_t_17, 1+__pyx_t_10, __pyx_t_18);
+        PyTuple_SET_ITEM(__pyx_t_19, 1, __pyx_t_18);
         __pyx_t_18 = 0;
-        __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_9, __pyx_t_17, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1695, __pyx_L7_except_error)
-        __Pyx_GOTREF(__pyx_t_8);
-        __Pyx_DECREF(__pyx_t_17); __pyx_t_17 = 0;
-      }
-      __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+        __Pyx_INCREF(__pyx_kp_u_raises_ABAPRuntimeError);
+        __pyx_t_15 += 26;
+        __Pyx_GIVEREF(__pyx_kp_u_raises_ABAPRuntimeError);
+        PyTuple_SET_ITEM(__pyx_t_19, 2, __pyx_kp_u_raises_ABAPRuntimeError);
+        __pyx_t_18 = __Pyx_PyObject_FormatSimple(__pyx_v_e, __pyx_empty_unicode); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 1695, __pyx_L33_error)
+        __Pyx_GOTREF(__pyx_t_18);
+        __pyx_t_5 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_18) > __pyx_t_5) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_18) : __pyx_t_5;
+        __pyx_t_15 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_18);
+        __Pyx_GIVEREF(__pyx_t_18);
+        PyTuple_SET_ITEM(__pyx_t_19, 3, __pyx_t_18);
+        __pyx_t_18 = 0;
+        __Pyx_INCREF(__pyx_kp_u_code_set_to_RFC_ABAP_MESSAGE);
+        __pyx_t_15 += 32;
+        __Pyx_GIVEREF(__pyx_kp_u_code_set_to_RFC_ABAP_MESSAGE);
+        PyTuple_SET_ITEM(__pyx_t_19, 4, __pyx_kp_u_code_set_to_RFC_ABAP_MESSAGE);
+        __pyx_t_18 = __Pyx_PyUnicode_Join(__pyx_t_19, 5, __pyx_t_15, __pyx_t_5); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 1695, __pyx_L33_error)
+        __Pyx_GOTREF(__pyx_t_18);
+        __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
+        __pyx_t_19 = NULL;
+        __pyx_t_16 = 0;
+        if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_9))) {
+          __pyx_t_19 = PyMethod_GET_SELF(__pyx_t_9);
+          if (likely(__pyx_t_19)) {
+            PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_9);
+            __Pyx_INCREF(__pyx_t_19);
+            __Pyx_INCREF(function);
+            __Pyx_DECREF_SET(__pyx_t_9, function);
+            __pyx_t_16 = 1;
+          }
+        }
+        #if CYTHON_FAST_PYCALL
+        if (PyFunction_Check(__pyx_t_9)) {
+          PyObject *__pyx_temp[3] = {__pyx_t_19, __pyx_n_u_genericHandler, __pyx_t_18};
+          __pyx_t_8 = __Pyx_PyFunction_FastCall(__pyx_t_9, __pyx_temp+1-__pyx_t_16, 2+__pyx_t_16); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1695, __pyx_L33_error)
+          __Pyx_XDECREF(__pyx_t_19); __pyx_t_19 = 0;
+          __Pyx_GOTREF(__pyx_t_8);
+          __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
+        } else
+        #endif
+        #if CYTHON_FAST_PYCCALL
+        if (__Pyx_PyFastCFunction_Check(__pyx_t_9)) {
+          PyObject *__pyx_temp[3] = {__pyx_t_19, __pyx_n_u_genericHandler, __pyx_t_18};
+          __pyx_t_8 = __Pyx_PyCFunction_FastCall(__pyx_t_9, __pyx_temp+1-__pyx_t_16, 2+__pyx_t_16); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1695, __pyx_L33_error)
+          __Pyx_XDECREF(__pyx_t_19); __pyx_t_19 = 0;
+          __Pyx_GOTREF(__pyx_t_8);
+          __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
+        } else
+        #endif
+        {
+          __pyx_t_17 = PyTuple_New(2+__pyx_t_16); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 1695, __pyx_L33_error)
+          __Pyx_GOTREF(__pyx_t_17);
+          if (__pyx_t_19) {
+            __Pyx_GIVEREF(__pyx_t_19); PyTuple_SET_ITEM(__pyx_t_17, 0, __pyx_t_19); __pyx_t_19 = NULL;
+          }
+          __Pyx_INCREF(__pyx_n_u_genericHandler);
+          __Pyx_GIVEREF(__pyx_n_u_genericHandler);
+          PyTuple_SET_ITEM(__pyx_t_17, 0+__pyx_t_16, __pyx_n_u_genericHandler);
+          __Pyx_GIVEREF(__pyx_t_18);
+          PyTuple_SET_ITEM(__pyx_t_17, 1+__pyx_t_16, __pyx_t_18);
+          __pyx_t_18 = 0;
+          __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_9, __pyx_t_17, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1695, __pyx_L33_error)
+          __Pyx_GOTREF(__pyx_t_8);
+          __Pyx_DECREF(__pyx_t_17); __pyx_t_17 = 0;
+        }
+        __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+        __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-      /* "pyrfc/_cyrfc.pyx":1696
+        /* "pyrfc/_cyrfc.pyx":1696
  *         serverErrorInfo.code = RFC_ABAP_MESSAGE  # Overwrite code, if set.
  *         _server_log("genericHandler", f"Request for '{func_name}' raises ABAPRuntimeError {e} - code set to RFC_ABAP_MESSAGE.")
  *         return RFC_ABAP_MESSAGE             # <<<<<<<<<<<<<<
  *     except ABAPApplicationError as e:  # ABAP Exception in implementing function
  *         # Parameter: key (optional: msg_type, msg_class, msg_number, msg_v1-v4)
  */
-      __pyx_r = RFC_ABAP_MESSAGE;
-      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-      goto __pyx_L8_except_return;
+        __pyx_r = RFC_ABAP_MESSAGE;
+        __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+        __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+        __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+        goto __pyx_L32_return;
+      }
+
+      /* "pyrfc/_cyrfc.pyx":1690
+ *         _server_log("genericHandler", f"Request for '{func_name}' raises ExternalRuntimeError {e} - code set to RFC_EXTERNAL_FAILURE.")
+ *         return RFC_EXTERNAL_FAILURE
+ *     except ABAPRuntimeError as e:  # ABAP Message             # <<<<<<<<<<<<<<
+ *         # Parameter: msg_type, msg_class, msg_number, msg_v1-v4
+ *         # returns:   RFC_ABAP_MESSAGE
+ */
+      /*finally:*/ {
+        __pyx_L33_error:;
+        /*exception exit:*/{
+          __Pyx_PyThreadState_declare
+          __Pyx_PyThreadState_assign
+          __pyx_t_26 = 0; __pyx_t_25 = 0; __pyx_t_24 = 0; __pyx_t_23 = 0; __pyx_t_22 = 0; __pyx_t_21 = 0;
+          __Pyx_XDECREF(__pyx_t_17); __pyx_t_17 = 0;
+          __Pyx_XDECREF(__pyx_t_18); __pyx_t_18 = 0;
+          __Pyx_XDECREF(__pyx_t_19); __pyx_t_19 = 0;
+          __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
+          __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
+          if (PY_MAJOR_VERSION >= 3) __Pyx_ExceptionSwap(&__pyx_t_23, &__pyx_t_22, &__pyx_t_21);
+          if ((PY_MAJOR_VERSION < 3) || unlikely(__Pyx_GetException(&__pyx_t_26, &__pyx_t_25, &__pyx_t_24) < 0)) __Pyx_ErrFetch(&__pyx_t_26, &__pyx_t_25, &__pyx_t_24);
+          __Pyx_XGOTREF(__pyx_t_26);
+          __Pyx_XGOTREF(__pyx_t_25);
+          __Pyx_XGOTREF(__pyx_t_24);
+          __Pyx_XGOTREF(__pyx_t_23);
+          __Pyx_XGOTREF(__pyx_t_22);
+          __Pyx_XGOTREF(__pyx_t_21);
+          __pyx_t_16 = __pyx_lineno; __pyx_t_10 = __pyx_clineno; __pyx_t_27 = __pyx_filename;
+          {
+            __Pyx_DECREF(__pyx_v_e);
+            __pyx_v_e = NULL;
+          }
+          if (PY_MAJOR_VERSION >= 3) {
+            __Pyx_XGIVEREF(__pyx_t_23);
+            __Pyx_XGIVEREF(__pyx_t_22);
+            __Pyx_XGIVEREF(__pyx_t_21);
+            __Pyx_ExceptionReset(__pyx_t_23, __pyx_t_22, __pyx_t_21);
+          }
+          __Pyx_XGIVEREF(__pyx_t_26);
+          __Pyx_XGIVEREF(__pyx_t_25);
+          __Pyx_XGIVEREF(__pyx_t_24);
+          __Pyx_ErrRestore(__pyx_t_26, __pyx_t_25, __pyx_t_24);
+          __pyx_t_26 = 0; __pyx_t_25 = 0; __pyx_t_24 = 0; __pyx_t_23 = 0; __pyx_t_22 = 0; __pyx_t_21 = 0;
+          __pyx_lineno = __pyx_t_16; __pyx_clineno = __pyx_t_10; __pyx_filename = __pyx_t_27;
+          goto __pyx_L7_except_error;
+        }
+        __pyx_L32_return: {
+          __pyx_t_14 = __pyx_r;
+          __Pyx_DECREF(__pyx_v_e);
+          __pyx_v_e = NULL;
+          __pyx_r = __pyx_t_14;
+          goto __pyx_L8_except_return;
+        }
+      }
     }
 
     /* "pyrfc/_cyrfc.pyx":1697
  *         _server_log("genericHandler", f"Request for '{func_name}' raises ABAPRuntimeError {e} - code set to RFC_ABAP_MESSAGE.")
  *         return RFC_ABAP_MESSAGE
  *     except ABAPApplicationError as e:  # ABAP Exception in implementing function             # <<<<<<<<<<<<<<
  *         # Parameter: key (optional: msg_type, msg_class, msg_number, msg_v1-v4)
@@ -21394,451 +21599,563 @@
       __Pyx_AddTraceback("pyrfc._cyrfc.genericHandler", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_7, &__pyx_t_6, &__pyx_t_1) < 0) __PYX_ERR(0, 1697, __pyx_L7_except_error)
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_INCREF(__pyx_t_6);
       __pyx_v_e = __pyx_t_6;
+      /*try:*/ {
 
-      /* "pyrfc/_cyrfc.pyx":1700
+        /* "pyrfc/_cyrfc.pyx":1700
  *         # Parameter: key (optional: msg_type, msg_class, msg_number, msg_v1-v4)
  *         # returns:   RFC_ABAP_EXCEPTION
  *         fillError(e, serverErrorInfo)             # <<<<<<<<<<<<<<
  *         serverErrorInfo.code = RFC_ABAP_EXCEPTION  # Overwrite code, if set.
  *         _server_log("genericHandler", f"Request for '{func_name}' raises ABAPApplicationError {e} - code set to RFC_ABAP_EXCEPTION.")
  */
-      __pyx_t_8 = __pyx_f_5pyrfc_6_cyrfc_fillError(__pyx_v_e, __pyx_v_serverErrorInfo); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1700, __pyx_L7_except_error)
-      __Pyx_GOTREF(__pyx_t_8);
-      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+        __pyx_t_8 = __pyx_f_5pyrfc_6_cyrfc_fillError(__pyx_v_e, __pyx_v_serverErrorInfo); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1700, __pyx_L44_error)
+        __Pyx_GOTREF(__pyx_t_8);
+        __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-      /* "pyrfc/_cyrfc.pyx":1701
+        /* "pyrfc/_cyrfc.pyx":1701
  *         # returns:   RFC_ABAP_EXCEPTION
  *         fillError(e, serverErrorInfo)
  *         serverErrorInfo.code = RFC_ABAP_EXCEPTION  # Overwrite code, if set.             # <<<<<<<<<<<<<<
  *         _server_log("genericHandler", f"Request for '{func_name}' raises ABAPApplicationError {e} - code set to RFC_ABAP_EXCEPTION.")
  *         return RFC_ABAP_EXCEPTION
  */
-      __pyx_v_serverErrorInfo->code = RFC_ABAP_EXCEPTION;
+        __pyx_v_serverErrorInfo->code = RFC_ABAP_EXCEPTION;
 
-      /* "pyrfc/_cyrfc.pyx":1702
+        /* "pyrfc/_cyrfc.pyx":1702
  *         fillError(e, serverErrorInfo)
  *         serverErrorInfo.code = RFC_ABAP_EXCEPTION  # Overwrite code, if set.
  *         _server_log("genericHandler", f"Request for '{func_name}' raises ABAPApplicationError {e} - code set to RFC_ABAP_EXCEPTION.")             # <<<<<<<<<<<<<<
  *         return RFC_ABAP_EXCEPTION
  *     except Exception as ex:
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_server_log); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 1702, __pyx_L7_except_error)
-      __Pyx_GOTREF(__pyx_t_9);
-      __pyx_t_17 = PyTuple_New(5); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 1702, __pyx_L7_except_error)
-      __Pyx_GOTREF(__pyx_t_17);
-      __pyx_t_15 = 0;
-      __pyx_t_5 = 127;
-      __Pyx_INCREF(__pyx_kp_u_Request_for);
-      __pyx_t_15 += 13;
-      __Pyx_GIVEREF(__pyx_kp_u_Request_for);
-      PyTuple_SET_ITEM(__pyx_t_17, 0, __pyx_kp_u_Request_for);
-      __pyx_t_18 = __Pyx_PyObject_FormatSimple(__pyx_v_func_name, __pyx_empty_unicode); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 1702, __pyx_L7_except_error)
-      __Pyx_GOTREF(__pyx_t_18);
-      __pyx_t_5 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_18) > __pyx_t_5) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_18) : __pyx_t_5;
-      __pyx_t_15 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_18);
-      __Pyx_GIVEREF(__pyx_t_18);
-      PyTuple_SET_ITEM(__pyx_t_17, 1, __pyx_t_18);
-      __pyx_t_18 = 0;
-      __Pyx_INCREF(__pyx_kp_u_raises_ABAPApplicationError);
-      __pyx_t_15 += 30;
-      __Pyx_GIVEREF(__pyx_kp_u_raises_ABAPApplicationError);
-      PyTuple_SET_ITEM(__pyx_t_17, 2, __pyx_kp_u_raises_ABAPApplicationError);
-      __pyx_t_18 = __Pyx_PyObject_FormatSimple(__pyx_v_e, __pyx_empty_unicode); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 1702, __pyx_L7_except_error)
-      __Pyx_GOTREF(__pyx_t_18);
-      __pyx_t_5 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_18) > __pyx_t_5) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_18) : __pyx_t_5;
-      __pyx_t_15 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_18);
-      __Pyx_GIVEREF(__pyx_t_18);
-      PyTuple_SET_ITEM(__pyx_t_17, 3, __pyx_t_18);
-      __pyx_t_18 = 0;
-      __Pyx_INCREF(__pyx_kp_u_code_set_to_RFC_ABAP_EXCEPTION);
-      __pyx_t_15 += 34;
-      __Pyx_GIVEREF(__pyx_kp_u_code_set_to_RFC_ABAP_EXCEPTION);
-      PyTuple_SET_ITEM(__pyx_t_17, 4, __pyx_kp_u_code_set_to_RFC_ABAP_EXCEPTION);
-      __pyx_t_18 = __Pyx_PyUnicode_Join(__pyx_t_17, 5, __pyx_t_15, __pyx_t_5); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 1702, __pyx_L7_except_error)
-      __Pyx_GOTREF(__pyx_t_18);
-      __Pyx_DECREF(__pyx_t_17); __pyx_t_17 = 0;
-      __pyx_t_17 = NULL;
-      __pyx_t_10 = 0;
-      if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_9))) {
-        __pyx_t_17 = PyMethod_GET_SELF(__pyx_t_9);
-        if (likely(__pyx_t_17)) {
-          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_9);
-          __Pyx_INCREF(__pyx_t_17);
-          __Pyx_INCREF(function);
-          __Pyx_DECREF_SET(__pyx_t_9, function);
-          __pyx_t_10 = 1;
-        }
-      }
-      #if CYTHON_FAST_PYCALL
-      if (PyFunction_Check(__pyx_t_9)) {
-        PyObject *__pyx_temp[3] = {__pyx_t_17, __pyx_n_s_genericHandler, __pyx_t_18};
-        __pyx_t_8 = __Pyx_PyFunction_FastCall(__pyx_t_9, __pyx_temp+1-__pyx_t_10, 2+__pyx_t_10); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1702, __pyx_L7_except_error)
-        __Pyx_XDECREF(__pyx_t_17); __pyx_t_17 = 0;
-        __Pyx_GOTREF(__pyx_t_8);
-        __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
-      } else
-      #endif
-      #if CYTHON_FAST_PYCCALL
-      if (__Pyx_PyFastCFunction_Check(__pyx_t_9)) {
-        PyObject *__pyx_temp[3] = {__pyx_t_17, __pyx_n_s_genericHandler, __pyx_t_18};
-        __pyx_t_8 = __Pyx_PyCFunction_FastCall(__pyx_t_9, __pyx_temp+1-__pyx_t_10, 2+__pyx_t_10); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1702, __pyx_L7_except_error)
-        __Pyx_XDECREF(__pyx_t_17); __pyx_t_17 = 0;
-        __Pyx_GOTREF(__pyx_t_8);
-        __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
-      } else
-      #endif
-      {
-        __pyx_t_19 = PyTuple_New(2+__pyx_t_10); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 1702, __pyx_L7_except_error)
-        __Pyx_GOTREF(__pyx_t_19);
-        if (__pyx_t_17) {
-          __Pyx_GIVEREF(__pyx_t_17); PyTuple_SET_ITEM(__pyx_t_19, 0, __pyx_t_17); __pyx_t_17 = NULL;
-        }
-        __Pyx_INCREF(__pyx_n_s_genericHandler);
-        __Pyx_GIVEREF(__pyx_n_s_genericHandler);
-        PyTuple_SET_ITEM(__pyx_t_19, 0+__pyx_t_10, __pyx_n_s_genericHandler);
+        __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_server_log); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 1702, __pyx_L44_error)
+        __Pyx_GOTREF(__pyx_t_9);
+        __pyx_t_17 = PyTuple_New(5); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 1702, __pyx_L44_error)
+        __Pyx_GOTREF(__pyx_t_17);
+        __pyx_t_15 = 0;
+        __pyx_t_5 = 127;
+        __Pyx_INCREF(__pyx_kp_u_Request_for);
+        __pyx_t_15 += 13;
+        __Pyx_GIVEREF(__pyx_kp_u_Request_for);
+        PyTuple_SET_ITEM(__pyx_t_17, 0, __pyx_kp_u_Request_for);
+        __pyx_t_18 = __Pyx_PyObject_FormatSimple(__pyx_v_func_name, __pyx_empty_unicode); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 1702, __pyx_L44_error)
+        __Pyx_GOTREF(__pyx_t_18);
+        __pyx_t_5 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_18) > __pyx_t_5) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_18) : __pyx_t_5;
+        __pyx_t_15 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_18);
         __Pyx_GIVEREF(__pyx_t_18);
-        PyTuple_SET_ITEM(__pyx_t_19, 1+__pyx_t_10, __pyx_t_18);
+        PyTuple_SET_ITEM(__pyx_t_17, 1, __pyx_t_18);
         __pyx_t_18 = 0;
-        __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_9, __pyx_t_19, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1702, __pyx_L7_except_error)
-        __Pyx_GOTREF(__pyx_t_8);
-        __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
-      }
-      __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+        __Pyx_INCREF(__pyx_kp_u_raises_ABAPApplicationError);
+        __pyx_t_15 += 30;
+        __Pyx_GIVEREF(__pyx_kp_u_raises_ABAPApplicationError);
+        PyTuple_SET_ITEM(__pyx_t_17, 2, __pyx_kp_u_raises_ABAPApplicationError);
+        __pyx_t_18 = __Pyx_PyObject_FormatSimple(__pyx_v_e, __pyx_empty_unicode); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 1702, __pyx_L44_error)
+        __Pyx_GOTREF(__pyx_t_18);
+        __pyx_t_5 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_18) > __pyx_t_5) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_18) : __pyx_t_5;
+        __pyx_t_15 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_18);
+        __Pyx_GIVEREF(__pyx_t_18);
+        PyTuple_SET_ITEM(__pyx_t_17, 3, __pyx_t_18);
+        __pyx_t_18 = 0;
+        __Pyx_INCREF(__pyx_kp_u_code_set_to_RFC_ABAP_EXCEPTION);
+        __pyx_t_15 += 34;
+        __Pyx_GIVEREF(__pyx_kp_u_code_set_to_RFC_ABAP_EXCEPTION);
+        PyTuple_SET_ITEM(__pyx_t_17, 4, __pyx_kp_u_code_set_to_RFC_ABAP_EXCEPTION);
+        __pyx_t_18 = __Pyx_PyUnicode_Join(__pyx_t_17, 5, __pyx_t_15, __pyx_t_5); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 1702, __pyx_L44_error)
+        __Pyx_GOTREF(__pyx_t_18);
+        __Pyx_DECREF(__pyx_t_17); __pyx_t_17 = 0;
+        __pyx_t_17 = NULL;
+        __pyx_t_10 = 0;
+        if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_9))) {
+          __pyx_t_17 = PyMethod_GET_SELF(__pyx_t_9);
+          if (likely(__pyx_t_17)) {
+            PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_9);
+            __Pyx_INCREF(__pyx_t_17);
+            __Pyx_INCREF(function);
+            __Pyx_DECREF_SET(__pyx_t_9, function);
+            __pyx_t_10 = 1;
+          }
+        }
+        #if CYTHON_FAST_PYCALL
+        if (PyFunction_Check(__pyx_t_9)) {
+          PyObject *__pyx_temp[3] = {__pyx_t_17, __pyx_n_u_genericHandler, __pyx_t_18};
+          __pyx_t_8 = __Pyx_PyFunction_FastCall(__pyx_t_9, __pyx_temp+1-__pyx_t_10, 2+__pyx_t_10); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1702, __pyx_L44_error)
+          __Pyx_XDECREF(__pyx_t_17); __pyx_t_17 = 0;
+          __Pyx_GOTREF(__pyx_t_8);
+          __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
+        } else
+        #endif
+        #if CYTHON_FAST_PYCCALL
+        if (__Pyx_PyFastCFunction_Check(__pyx_t_9)) {
+          PyObject *__pyx_temp[3] = {__pyx_t_17, __pyx_n_u_genericHandler, __pyx_t_18};
+          __pyx_t_8 = __Pyx_PyCFunction_FastCall(__pyx_t_9, __pyx_temp+1-__pyx_t_10, 2+__pyx_t_10); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1702, __pyx_L44_error)
+          __Pyx_XDECREF(__pyx_t_17); __pyx_t_17 = 0;
+          __Pyx_GOTREF(__pyx_t_8);
+          __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
+        } else
+        #endif
+        {
+          __pyx_t_19 = PyTuple_New(2+__pyx_t_10); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 1702, __pyx_L44_error)
+          __Pyx_GOTREF(__pyx_t_19);
+          if (__pyx_t_17) {
+            __Pyx_GIVEREF(__pyx_t_17); PyTuple_SET_ITEM(__pyx_t_19, 0, __pyx_t_17); __pyx_t_17 = NULL;
+          }
+          __Pyx_INCREF(__pyx_n_u_genericHandler);
+          __Pyx_GIVEREF(__pyx_n_u_genericHandler);
+          PyTuple_SET_ITEM(__pyx_t_19, 0+__pyx_t_10, __pyx_n_u_genericHandler);
+          __Pyx_GIVEREF(__pyx_t_18);
+          PyTuple_SET_ITEM(__pyx_t_19, 1+__pyx_t_10, __pyx_t_18);
+          __pyx_t_18 = 0;
+          __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_9, __pyx_t_19, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1702, __pyx_L44_error)
+          __Pyx_GOTREF(__pyx_t_8);
+          __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
+        }
+        __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+        __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-      /* "pyrfc/_cyrfc.pyx":1703
+        /* "pyrfc/_cyrfc.pyx":1703
  *         serverErrorInfo.code = RFC_ABAP_EXCEPTION  # Overwrite code, if set.
  *         _server_log("genericHandler", f"Request for '{func_name}' raises ABAPApplicationError {e} - code set to RFC_ABAP_EXCEPTION.")
  *         return RFC_ABAP_EXCEPTION             # <<<<<<<<<<<<<<
  *     except Exception as ex:
  *         exctype, value = exc_info()[:2]
  */
-      __pyx_r = RFC_ABAP_EXCEPTION;
-      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-      goto __pyx_L8_except_return;
+        __pyx_r = RFC_ABAP_EXCEPTION;
+        __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+        __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+        __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+        goto __pyx_L43_return;
+      }
+
+      /* "pyrfc/_cyrfc.pyx":1697
+ *         _server_log("genericHandler", f"Request for '{func_name}' raises ABAPRuntimeError {e} - code set to RFC_ABAP_MESSAGE.")
+ *         return RFC_ABAP_MESSAGE
+ *     except ABAPApplicationError as e:  # ABAP Exception in implementing function             # <<<<<<<<<<<<<<
+ *         # Parameter: key (optional: msg_type, msg_class, msg_number, msg_v1-v4)
+ *         # returns:   RFC_ABAP_EXCEPTION
+ */
+      /*finally:*/ {
+        __pyx_L44_error:;
+        /*exception exit:*/{
+          __Pyx_PyThreadState_declare
+          __Pyx_PyThreadState_assign
+          __pyx_t_21 = 0; __pyx_t_22 = 0; __pyx_t_23 = 0; __pyx_t_24 = 0; __pyx_t_25 = 0; __pyx_t_26 = 0;
+          __Pyx_XDECREF(__pyx_t_17); __pyx_t_17 = 0;
+          __Pyx_XDECREF(__pyx_t_18); __pyx_t_18 = 0;
+          __Pyx_XDECREF(__pyx_t_19); __pyx_t_19 = 0;
+          __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
+          __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
+          if (PY_MAJOR_VERSION >= 3) __Pyx_ExceptionSwap(&__pyx_t_24, &__pyx_t_25, &__pyx_t_26);
+          if ((PY_MAJOR_VERSION < 3) || unlikely(__Pyx_GetException(&__pyx_t_21, &__pyx_t_22, &__pyx_t_23) < 0)) __Pyx_ErrFetch(&__pyx_t_21, &__pyx_t_22, &__pyx_t_23);
+          __Pyx_XGOTREF(__pyx_t_21);
+          __Pyx_XGOTREF(__pyx_t_22);
+          __Pyx_XGOTREF(__pyx_t_23);
+          __Pyx_XGOTREF(__pyx_t_24);
+          __Pyx_XGOTREF(__pyx_t_25);
+          __Pyx_XGOTREF(__pyx_t_26);
+          __pyx_t_10 = __pyx_lineno; __pyx_t_16 = __pyx_clineno; __pyx_t_28 = __pyx_filename;
+          {
+            __Pyx_DECREF(__pyx_v_e);
+            __pyx_v_e = NULL;
+          }
+          if (PY_MAJOR_VERSION >= 3) {
+            __Pyx_XGIVEREF(__pyx_t_24);
+            __Pyx_XGIVEREF(__pyx_t_25);
+            __Pyx_XGIVEREF(__pyx_t_26);
+            __Pyx_ExceptionReset(__pyx_t_24, __pyx_t_25, __pyx_t_26);
+          }
+          __Pyx_XGIVEREF(__pyx_t_21);
+          __Pyx_XGIVEREF(__pyx_t_22);
+          __Pyx_XGIVEREF(__pyx_t_23);
+          __Pyx_ErrRestore(__pyx_t_21, __pyx_t_22, __pyx_t_23);
+          __pyx_t_21 = 0; __pyx_t_22 = 0; __pyx_t_23 = 0; __pyx_t_24 = 0; __pyx_t_25 = 0; __pyx_t_26 = 0;
+          __pyx_lineno = __pyx_t_10; __pyx_clineno = __pyx_t_16; __pyx_filename = __pyx_t_28;
+          goto __pyx_L7_except_error;
+        }
+        __pyx_L43_return: {
+          __pyx_t_14 = __pyx_r;
+          __Pyx_DECREF(__pyx_v_e);
+          __pyx_v_e = NULL;
+          __pyx_r = __pyx_t_14;
+          goto __pyx_L8_except_return;
+        }
+      }
     }
 
     /* "pyrfc/_cyrfc.pyx":1704
  *         _server_log("genericHandler", f"Request for '{func_name}' raises ABAPApplicationError {e} - code set to RFC_ABAP_EXCEPTION.")
  *         return RFC_ABAP_EXCEPTION
  *     except Exception as ex:             # <<<<<<<<<<<<<<
  *         exctype, value = exc_info()[:2]
  *         _server_log(
  */
-    __pyx_t_10 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
-    if (__pyx_t_10) {
+    __pyx_t_16 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
+    if (__pyx_t_16) {
       __Pyx_AddTraceback("pyrfc._cyrfc.genericHandler", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_1, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(0, 1704, __pyx_L7_except_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_INCREF(__pyx_t_6);
       __pyx_v_ex = __pyx_t_6;
+      /*try:*/ {
 
-      /* "pyrfc/_cyrfc.pyx":1705
+        /* "pyrfc/_cyrfc.pyx":1705
  *         return RFC_ABAP_EXCEPTION
  *     except Exception as ex:
  *         exctype, value = exc_info()[:2]             # <<<<<<<<<<<<<<
  *         _server_log(
  *             "genericHandler",
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_exc_info); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 1705, __pyx_L7_except_error)
-      __Pyx_GOTREF(__pyx_t_9);
-      __pyx_t_19 = NULL;
-      if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_9))) {
-        __pyx_t_19 = PyMethod_GET_SELF(__pyx_t_9);
-        if (likely(__pyx_t_19)) {
-          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_9);
-          __Pyx_INCREF(__pyx_t_19);
-          __Pyx_INCREF(function);
-          __Pyx_DECREF_SET(__pyx_t_9, function);
-        }
-      }
-      __pyx_t_8 = (__pyx_t_19) ? __Pyx_PyObject_CallOneArg(__pyx_t_9, __pyx_t_19) : __Pyx_PyObject_CallNoArg(__pyx_t_9);
-      __Pyx_XDECREF(__pyx_t_19); __pyx_t_19 = 0;
-      if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1705, __pyx_L7_except_error)
-      __Pyx_GOTREF(__pyx_t_8);
-      __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-      __pyx_t_9 = __Pyx_PyObject_GetSlice(__pyx_t_8, 0, 2, NULL, NULL, &__pyx_slice__29, 0, 1, 1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 1705, __pyx_L7_except_error)
-      __Pyx_GOTREF(__pyx_t_9);
-      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      if ((likely(PyTuple_CheckExact(__pyx_t_9))) || (PyList_CheckExact(__pyx_t_9))) {
-        PyObject* sequence = __pyx_t_9;
-        Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
-        if (unlikely(size != 2)) {
-          if (size > 2) __Pyx_RaiseTooManyValuesError(2);
-          else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-          __PYX_ERR(0, 1705, __pyx_L7_except_error)
-        }
-        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        if (likely(PyTuple_CheckExact(sequence))) {
-          __pyx_t_8 = PyTuple_GET_ITEM(sequence, 0); 
-          __pyx_t_19 = PyTuple_GET_ITEM(sequence, 1); 
-        } else {
-          __pyx_t_8 = PyList_GET_ITEM(sequence, 0); 
-          __pyx_t_19 = PyList_GET_ITEM(sequence, 1); 
+        __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_exc_info); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 1705, __pyx_L55_error)
+        __Pyx_GOTREF(__pyx_t_9);
+        __pyx_t_19 = NULL;
+        if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_9))) {
+          __pyx_t_19 = PyMethod_GET_SELF(__pyx_t_9);
+          if (likely(__pyx_t_19)) {
+            PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_9);
+            __Pyx_INCREF(__pyx_t_19);
+            __Pyx_INCREF(function);
+            __Pyx_DECREF_SET(__pyx_t_9, function);
+          }
         }
-        __Pyx_INCREF(__pyx_t_8);
-        __Pyx_INCREF(__pyx_t_19);
-        #else
-        __pyx_t_8 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1705, __pyx_L7_except_error)
+        __pyx_t_8 = (__pyx_t_19) ? __Pyx_PyObject_CallOneArg(__pyx_t_9, __pyx_t_19) : __Pyx_PyObject_CallNoArg(__pyx_t_9);
+        __Pyx_XDECREF(__pyx_t_19); __pyx_t_19 = 0;
+        if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1705, __pyx_L55_error)
         __Pyx_GOTREF(__pyx_t_8);
-        __pyx_t_19 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 1705, __pyx_L7_except_error)
-        __Pyx_GOTREF(__pyx_t_19);
-        #endif
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-      } else {
-        Py_ssize_t index = -1;
-        __pyx_t_18 = PyObject_GetIter(__pyx_t_9); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 1705, __pyx_L7_except_error)
-        __Pyx_GOTREF(__pyx_t_18);
-        __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-        __pyx_t_20 = Py_TYPE(__pyx_t_18)->tp_iternext;
-        index = 0; __pyx_t_8 = __pyx_t_20(__pyx_t_18); if (unlikely(!__pyx_t_8)) goto __pyx_L25_unpacking_failed;
-        __Pyx_GOTREF(__pyx_t_8);
-        index = 1; __pyx_t_19 = __pyx_t_20(__pyx_t_18); if (unlikely(!__pyx_t_19)) goto __pyx_L25_unpacking_failed;
-        __Pyx_GOTREF(__pyx_t_19);
-        if (__Pyx_IternextUnpackEndCheck(__pyx_t_20(__pyx_t_18), 2) < 0) __PYX_ERR(0, 1705, __pyx_L7_except_error)
-        __pyx_t_20 = NULL;
-        __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
-        goto __pyx_L26_unpacking_done;
-        __pyx_L25_unpacking_failed:;
-        __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
-        __pyx_t_20 = NULL;
-        if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-        __PYX_ERR(0, 1705, __pyx_L7_except_error)
-        __pyx_L26_unpacking_done:;
-      }
-      __pyx_v_exctype = __pyx_t_8;
-      __pyx_t_8 = 0;
-      __Pyx_XDECREF_SET(__pyx_v_value, __pyx_t_19);
-      __pyx_t_19 = 0;
+        __pyx_t_9 = __Pyx_PyObject_GetSlice(__pyx_t_8, 0, 2, NULL, NULL, &__pyx_slice__30, 0, 1, 1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 1705, __pyx_L55_error)
+        __Pyx_GOTREF(__pyx_t_9);
+        __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+        if ((likely(PyTuple_CheckExact(__pyx_t_9))) || (PyList_CheckExact(__pyx_t_9))) {
+          PyObject* sequence = __pyx_t_9;
+          Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
+          if (unlikely(size != 2)) {
+            if (size > 2) __Pyx_RaiseTooManyValuesError(2);
+            else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
+            __PYX_ERR(0, 1705, __pyx_L55_error)
+          }
+          #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+          if (likely(PyTuple_CheckExact(sequence))) {
+            __pyx_t_8 = PyTuple_GET_ITEM(sequence, 0); 
+            __pyx_t_19 = PyTuple_GET_ITEM(sequence, 1); 
+          } else {
+            __pyx_t_8 = PyList_GET_ITEM(sequence, 0); 
+            __pyx_t_19 = PyList_GET_ITEM(sequence, 1); 
+          }
+          __Pyx_INCREF(__pyx_t_8);
+          __Pyx_INCREF(__pyx_t_19);
+          #else
+          __pyx_t_8 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1705, __pyx_L55_error)
+          __Pyx_GOTREF(__pyx_t_8);
+          __pyx_t_19 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 1705, __pyx_L55_error)
+          __Pyx_GOTREF(__pyx_t_19);
+          #endif
+          __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+        } else {
+          Py_ssize_t index = -1;
+          __pyx_t_18 = PyObject_GetIter(__pyx_t_9); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 1705, __pyx_L55_error)
+          __Pyx_GOTREF(__pyx_t_18);
+          __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+          __pyx_t_29 = Py_TYPE(__pyx_t_18)->tp_iternext;
+          index = 0; __pyx_t_8 = __pyx_t_29(__pyx_t_18); if (unlikely(!__pyx_t_8)) goto __pyx_L57_unpacking_failed;
+          __Pyx_GOTREF(__pyx_t_8);
+          index = 1; __pyx_t_19 = __pyx_t_29(__pyx_t_18); if (unlikely(!__pyx_t_19)) goto __pyx_L57_unpacking_failed;
+          __Pyx_GOTREF(__pyx_t_19);
+          if (__Pyx_IternextUnpackEndCheck(__pyx_t_29(__pyx_t_18), 2) < 0) __PYX_ERR(0, 1705, __pyx_L55_error)
+          __pyx_t_29 = NULL;
+          __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
+          goto __pyx_L58_unpacking_done;
+          __pyx_L57_unpacking_failed:;
+          __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
+          __pyx_t_29 = NULL;
+          if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
+          __PYX_ERR(0, 1705, __pyx_L55_error)
+          __pyx_L58_unpacking_done:;
+        }
+        __pyx_v_exctype = __pyx_t_8;
+        __pyx_t_8 = 0;
+        __Pyx_XDECREF_SET(__pyx_v_value, __pyx_t_19);
+        __pyx_t_19 = 0;
 
-      /* "pyrfc/_cyrfc.pyx":1706
+        /* "pyrfc/_cyrfc.pyx":1706
  *     except Exception as ex:
  *         exctype, value = exc_info()[:2]
  *         _server_log(             # <<<<<<<<<<<<<<
  *             "genericHandler",
  *             f"Request for '{func_name}' raises an invalid exception:\n Exception: {exctype}\n Values: {value}\n"
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_19, __pyx_n_s_server_log); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 1706, __pyx_L7_except_error)
-      __Pyx_GOTREF(__pyx_t_19);
+        __Pyx_GetModuleGlobalName(__pyx_t_19, __pyx_n_s_server_log); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 1706, __pyx_L55_error)
+        __Pyx_GOTREF(__pyx_t_19);
 
-      /* "pyrfc/_cyrfc.pyx":1708
+        /* "pyrfc/_cyrfc.pyx":1708
  *         _server_log(
  *             "genericHandler",
  *             f"Request for '{func_name}' raises an invalid exception:\n Exception: {exctype}\n Values: {value}\n"             # <<<<<<<<<<<<<<
  *             "Callback functions may only raise ABAPApplicationError, ABAPRuntimeError, or ExternalRuntimeError.\n"
  *             "The values of the request were:\n"
  */
-      __pyx_t_8 = PyTuple_New(10); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1708, __pyx_L7_except_error)
-      __Pyx_GOTREF(__pyx_t_8);
-      __pyx_t_15 = 0;
-      __pyx_t_5 = 127;
-      __Pyx_INCREF(__pyx_kp_u_Request_for);
-      __pyx_t_15 += 13;
-      __Pyx_GIVEREF(__pyx_kp_u_Request_for);
-      PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_kp_u_Request_for);
-      __pyx_t_18 = __Pyx_PyObject_FormatSimple(__pyx_v_func_name, __pyx_empty_unicode); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 1708, __pyx_L7_except_error)
-      __Pyx_GOTREF(__pyx_t_18);
-      __pyx_t_5 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_18) > __pyx_t_5) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_18) : __pyx_t_5;
-      __pyx_t_15 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_18);
-      __Pyx_GIVEREF(__pyx_t_18);
-      PyTuple_SET_ITEM(__pyx_t_8, 1, __pyx_t_18);
-      __pyx_t_18 = 0;
-      __Pyx_INCREF(__pyx_kp_u_raises_an_invalid_exception_Exc);
-      __pyx_t_15 += 43;
-      __Pyx_GIVEREF(__pyx_kp_u_raises_an_invalid_exception_Exc);
-      PyTuple_SET_ITEM(__pyx_t_8, 2, __pyx_kp_u_raises_an_invalid_exception_Exc);
-      __pyx_t_18 = __Pyx_PyObject_FormatSimple(__pyx_v_exctype, __pyx_empty_unicode); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 1708, __pyx_L7_except_error)
-      __Pyx_GOTREF(__pyx_t_18);
-      __pyx_t_5 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_18) > __pyx_t_5) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_18) : __pyx_t_5;
-      __pyx_t_15 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_18);
-      __Pyx_GIVEREF(__pyx_t_18);
-      PyTuple_SET_ITEM(__pyx_t_8, 3, __pyx_t_18);
-      __pyx_t_18 = 0;
-      __Pyx_INCREF(__pyx_kp_u_Values);
-      __pyx_t_15 += 10;
-      __Pyx_GIVEREF(__pyx_kp_u_Values);
-      PyTuple_SET_ITEM(__pyx_t_8, 4, __pyx_kp_u_Values);
-      __pyx_t_18 = __Pyx_PyObject_FormatSimple(__pyx_v_value, __pyx_empty_unicode); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 1708, __pyx_L7_except_error)
-      __Pyx_GOTREF(__pyx_t_18);
-      __pyx_t_5 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_18) > __pyx_t_5) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_18) : __pyx_t_5;
-      __pyx_t_15 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_18);
-      __Pyx_GIVEREF(__pyx_t_18);
-      PyTuple_SET_ITEM(__pyx_t_8, 5, __pyx_t_18);
-      __pyx_t_18 = 0;
-      __Pyx_INCREF(__pyx_kp_u_Callback_functions_may_only_rai);
-      __pyx_t_15 += 140;
-      __Pyx_GIVEREF(__pyx_kp_u_Callback_functions_may_only_rai);
-      PyTuple_SET_ITEM(__pyx_t_8, 6, __pyx_kp_u_Callback_functions_may_only_rai);
+        __pyx_t_8 = PyTuple_New(10); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1708, __pyx_L55_error)
+        __Pyx_GOTREF(__pyx_t_8);
+        __pyx_t_15 = 0;
+        __pyx_t_5 = 127;
+        __Pyx_INCREF(__pyx_kp_u_Request_for);
+        __pyx_t_15 += 13;
+        __Pyx_GIVEREF(__pyx_kp_u_Request_for);
+        PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_kp_u_Request_for);
+        __pyx_t_18 = __Pyx_PyObject_FormatSimple(__pyx_v_func_name, __pyx_empty_unicode); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 1708, __pyx_L55_error)
+        __Pyx_GOTREF(__pyx_t_18);
+        __pyx_t_5 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_18) > __pyx_t_5) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_18) : __pyx_t_5;
+        __pyx_t_15 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_18);
+        __Pyx_GIVEREF(__pyx_t_18);
+        PyTuple_SET_ITEM(__pyx_t_8, 1, __pyx_t_18);
+        __pyx_t_18 = 0;
+        __Pyx_INCREF(__pyx_kp_u_raises_an_invalid_exception_Exc);
+        __pyx_t_15 += 43;
+        __Pyx_GIVEREF(__pyx_kp_u_raises_an_invalid_exception_Exc);
+        PyTuple_SET_ITEM(__pyx_t_8, 2, __pyx_kp_u_raises_an_invalid_exception_Exc);
+        __pyx_t_18 = __Pyx_PyObject_FormatSimple(__pyx_v_exctype, __pyx_empty_unicode); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 1708, __pyx_L55_error)
+        __Pyx_GOTREF(__pyx_t_18);
+        __pyx_t_5 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_18) > __pyx_t_5) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_18) : __pyx_t_5;
+        __pyx_t_15 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_18);
+        __Pyx_GIVEREF(__pyx_t_18);
+        PyTuple_SET_ITEM(__pyx_t_8, 3, __pyx_t_18);
+        __pyx_t_18 = 0;
+        __Pyx_INCREF(__pyx_kp_u_Values);
+        __pyx_t_15 += 10;
+        __Pyx_GIVEREF(__pyx_kp_u_Values);
+        PyTuple_SET_ITEM(__pyx_t_8, 4, __pyx_kp_u_Values);
+        __pyx_t_18 = __Pyx_PyObject_FormatSimple(__pyx_v_value, __pyx_empty_unicode); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 1708, __pyx_L55_error)
+        __Pyx_GOTREF(__pyx_t_18);
+        __pyx_t_5 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_18) > __pyx_t_5) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_18) : __pyx_t_5;
+        __pyx_t_15 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_18);
+        __Pyx_GIVEREF(__pyx_t_18);
+        PyTuple_SET_ITEM(__pyx_t_8, 5, __pyx_t_18);
+        __pyx_t_18 = 0;
+        __Pyx_INCREF(__pyx_kp_u_Callback_functions_may_only_rai);
+        __pyx_t_15 += 140;
+        __Pyx_GIVEREF(__pyx_kp_u_Callback_functions_may_only_rai);
+        PyTuple_SET_ITEM(__pyx_t_8, 6, __pyx_kp_u_Callback_functions_may_only_rai);
 
-      /* "pyrfc/_cyrfc.pyx":1711
+        /* "pyrfc/_cyrfc.pyx":1711
  *             "Callback functions may only raise ABAPApplicationError, ABAPRuntimeError, or ExternalRuntimeError.\n"
  *             "The values of the request were:\n"
  *             f"params: {func_handle_variables}\nrequest_context: {request_context}"             # <<<<<<<<<<<<<<
  *         )
  *         new_error = ExternalRuntimeError(
  */
-      if (unlikely(!__pyx_v_func_handle_variables)) { __Pyx_RaiseUnboundLocalError("func_handle_variables"); __PYX_ERR(0, 1711, __pyx_L7_except_error) }
-      __pyx_t_18 = __Pyx_PyObject_FormatSimple(__pyx_v_func_handle_variables, __pyx_empty_unicode); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 1711, __pyx_L7_except_error)
-      __Pyx_GOTREF(__pyx_t_18);
-      __pyx_t_5 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_18) > __pyx_t_5) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_18) : __pyx_t_5;
-      __pyx_t_15 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_18);
-      __Pyx_GIVEREF(__pyx_t_18);
-      PyTuple_SET_ITEM(__pyx_t_8, 7, __pyx_t_18);
-      __pyx_t_18 = 0;
-      __Pyx_INCREF(__pyx_kp_u_request_context_2);
-      __pyx_t_15 += 18;
-      __Pyx_GIVEREF(__pyx_kp_u_request_context_2);
-      PyTuple_SET_ITEM(__pyx_t_8, 8, __pyx_kp_u_request_context_2);
-      if (unlikely(!__pyx_v_request_context)) { __Pyx_RaiseUnboundLocalError("request_context"); __PYX_ERR(0, 1711, __pyx_L7_except_error) }
-      __pyx_t_18 = __Pyx_PyObject_FormatSimple(__pyx_v_request_context, __pyx_empty_unicode); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 1711, __pyx_L7_except_error)
-      __Pyx_GOTREF(__pyx_t_18);
-      __pyx_t_5 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_18) > __pyx_t_5) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_18) : __pyx_t_5;
-      __pyx_t_15 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_18);
-      __Pyx_GIVEREF(__pyx_t_18);
-      PyTuple_SET_ITEM(__pyx_t_8, 9, __pyx_t_18);
-      __pyx_t_18 = 0;
+        if (unlikely(!__pyx_v_func_handle_variables)) { __Pyx_RaiseUnboundLocalError("func_handle_variables"); __PYX_ERR(0, 1711, __pyx_L55_error) }
+        __pyx_t_18 = __Pyx_PyObject_FormatSimple(__pyx_v_func_handle_variables, __pyx_empty_unicode); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 1711, __pyx_L55_error)
+        __Pyx_GOTREF(__pyx_t_18);
+        __pyx_t_5 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_18) > __pyx_t_5) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_18) : __pyx_t_5;
+        __pyx_t_15 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_18);
+        __Pyx_GIVEREF(__pyx_t_18);
+        PyTuple_SET_ITEM(__pyx_t_8, 7, __pyx_t_18);
+        __pyx_t_18 = 0;
+        __Pyx_INCREF(__pyx_kp_u_request_context_2);
+        __pyx_t_15 += 18;
+        __Pyx_GIVEREF(__pyx_kp_u_request_context_2);
+        PyTuple_SET_ITEM(__pyx_t_8, 8, __pyx_kp_u_request_context_2);
+        if (unlikely(!__pyx_v_request_context)) { __Pyx_RaiseUnboundLocalError("request_context"); __PYX_ERR(0, 1711, __pyx_L55_error) }
+        __pyx_t_18 = __Pyx_PyObject_FormatSimple(__pyx_v_request_context, __pyx_empty_unicode); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 1711, __pyx_L55_error)
+        __Pyx_GOTREF(__pyx_t_18);
+        __pyx_t_5 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_18) > __pyx_t_5) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_18) : __pyx_t_5;
+        __pyx_t_15 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_18);
+        __Pyx_GIVEREF(__pyx_t_18);
+        PyTuple_SET_ITEM(__pyx_t_8, 9, __pyx_t_18);
+        __pyx_t_18 = 0;
 
-      /* "pyrfc/_cyrfc.pyx":1708
+        /* "pyrfc/_cyrfc.pyx":1708
  *         _server_log(
  *             "genericHandler",
  *             f"Request for '{func_name}' raises an invalid exception:\n Exception: {exctype}\n Values: {value}\n"             # <<<<<<<<<<<<<<
  *             "Callback functions may only raise ABAPApplicationError, ABAPRuntimeError, or ExternalRuntimeError.\n"
  *             "The values of the request were:\n"
  */
-      __pyx_t_18 = __Pyx_PyUnicode_Join(__pyx_t_8, 10, __pyx_t_15, __pyx_t_5); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 1708, __pyx_L7_except_error)
-      __Pyx_GOTREF(__pyx_t_18);
-      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __pyx_t_8 = NULL;
-      __pyx_t_10 = 0;
-      if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_19))) {
-        __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_19);
-        if (likely(__pyx_t_8)) {
-          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_19);
-          __Pyx_INCREF(__pyx_t_8);
-          __Pyx_INCREF(function);
-          __Pyx_DECREF_SET(__pyx_t_19, function);
-          __pyx_t_10 = 1;
+        __pyx_t_18 = __Pyx_PyUnicode_Join(__pyx_t_8, 10, __pyx_t_15, __pyx_t_5); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 1708, __pyx_L55_error)
+        __Pyx_GOTREF(__pyx_t_18);
+        __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+        __pyx_t_8 = NULL;
+        __pyx_t_16 = 0;
+        if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_19))) {
+          __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_19);
+          if (likely(__pyx_t_8)) {
+            PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_19);
+            __Pyx_INCREF(__pyx_t_8);
+            __Pyx_INCREF(function);
+            __Pyx_DECREF_SET(__pyx_t_19, function);
+            __pyx_t_16 = 1;
+          }
         }
-      }
-      #if CYTHON_FAST_PYCALL
-      if (PyFunction_Check(__pyx_t_19)) {
-        PyObject *__pyx_temp[3] = {__pyx_t_8, __pyx_n_s_genericHandler, __pyx_t_18};
-        __pyx_t_9 = __Pyx_PyFunction_FastCall(__pyx_t_19, __pyx_temp+1-__pyx_t_10, 2+__pyx_t_10); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 1706, __pyx_L7_except_error)
-        __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
-        __Pyx_GOTREF(__pyx_t_9);
-        __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
-      } else
-      #endif
-      #if CYTHON_FAST_PYCCALL
-      if (__Pyx_PyFastCFunction_Check(__pyx_t_19)) {
-        PyObject *__pyx_temp[3] = {__pyx_t_8, __pyx_n_s_genericHandler, __pyx_t_18};
-        __pyx_t_9 = __Pyx_PyCFunction_FastCall(__pyx_t_19, __pyx_temp+1-__pyx_t_10, 2+__pyx_t_10); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 1706, __pyx_L7_except_error)
-        __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
-        __Pyx_GOTREF(__pyx_t_9);
-        __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
-      } else
-      #endif
-      {
-        __pyx_t_17 = PyTuple_New(2+__pyx_t_10); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 1706, __pyx_L7_except_error)
-        __Pyx_GOTREF(__pyx_t_17);
-        if (__pyx_t_8) {
-          __Pyx_GIVEREF(__pyx_t_8); PyTuple_SET_ITEM(__pyx_t_17, 0, __pyx_t_8); __pyx_t_8 = NULL;
+        #if CYTHON_FAST_PYCALL
+        if (PyFunction_Check(__pyx_t_19)) {
+          PyObject *__pyx_temp[3] = {__pyx_t_8, __pyx_n_u_genericHandler, __pyx_t_18};
+          __pyx_t_9 = __Pyx_PyFunction_FastCall(__pyx_t_19, __pyx_temp+1-__pyx_t_16, 2+__pyx_t_16); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 1706, __pyx_L55_error)
+          __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
+          __Pyx_GOTREF(__pyx_t_9);
+          __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
+        } else
+        #endif
+        #if CYTHON_FAST_PYCCALL
+        if (__Pyx_PyFastCFunction_Check(__pyx_t_19)) {
+          PyObject *__pyx_temp[3] = {__pyx_t_8, __pyx_n_u_genericHandler, __pyx_t_18};
+          __pyx_t_9 = __Pyx_PyCFunction_FastCall(__pyx_t_19, __pyx_temp+1-__pyx_t_16, 2+__pyx_t_16); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 1706, __pyx_L55_error)
+          __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
+          __Pyx_GOTREF(__pyx_t_9);
+          __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
+        } else
+        #endif
+        {
+          __pyx_t_17 = PyTuple_New(2+__pyx_t_16); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 1706, __pyx_L55_error)
+          __Pyx_GOTREF(__pyx_t_17);
+          if (__pyx_t_8) {
+            __Pyx_GIVEREF(__pyx_t_8); PyTuple_SET_ITEM(__pyx_t_17, 0, __pyx_t_8); __pyx_t_8 = NULL;
+          }
+          __Pyx_INCREF(__pyx_n_u_genericHandler);
+          __Pyx_GIVEREF(__pyx_n_u_genericHandler);
+          PyTuple_SET_ITEM(__pyx_t_17, 0+__pyx_t_16, __pyx_n_u_genericHandler);
+          __Pyx_GIVEREF(__pyx_t_18);
+          PyTuple_SET_ITEM(__pyx_t_17, 1+__pyx_t_16, __pyx_t_18);
+          __pyx_t_18 = 0;
+          __pyx_t_9 = __Pyx_PyObject_Call(__pyx_t_19, __pyx_t_17, NULL); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 1706, __pyx_L55_error)
+          __Pyx_GOTREF(__pyx_t_9);
+          __Pyx_DECREF(__pyx_t_17); __pyx_t_17 = 0;
         }
-        __Pyx_INCREF(__pyx_n_s_genericHandler);
-        __Pyx_GIVEREF(__pyx_n_s_genericHandler);
-        PyTuple_SET_ITEM(__pyx_t_17, 0+__pyx_t_10, __pyx_n_s_genericHandler);
-        __Pyx_GIVEREF(__pyx_t_18);
-        PyTuple_SET_ITEM(__pyx_t_17, 1+__pyx_t_10, __pyx_t_18);
-        __pyx_t_18 = 0;
-        __pyx_t_9 = __Pyx_PyObject_Call(__pyx_t_19, __pyx_t_17, NULL); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 1706, __pyx_L7_except_error)
-        __Pyx_GOTREF(__pyx_t_9);
-        __Pyx_DECREF(__pyx_t_17); __pyx_t_17 = 0;
-      }
-      __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
-      __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+        __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
+        __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
 
-      /* "pyrfc/_cyrfc.pyx":1713
+        /* "pyrfc/_cyrfc.pyx":1713
  *             f"params: {func_handle_variables}\nrequest_context: {request_context}"
  *         )
  *         new_error = ExternalRuntimeError(             # <<<<<<<<<<<<<<
  *             message="Invalid exception raised by callback function.",
  *             code=RFC_EXTERNAL_FAILURE
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_ExternalRuntimeError); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 1713, __pyx_L7_except_error)
-      __Pyx_GOTREF(__pyx_t_9);
+        __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_ExternalRuntimeError); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 1713, __pyx_L55_error)
+        __Pyx_GOTREF(__pyx_t_9);
 
-      /* "pyrfc/_cyrfc.pyx":1714
+        /* "pyrfc/_cyrfc.pyx":1714
  *         )
  *         new_error = ExternalRuntimeError(
  *             message="Invalid exception raised by callback function.",             # <<<<<<<<<<<<<<
  *             code=RFC_EXTERNAL_FAILURE
  *         )
  */
-      __pyx_t_19 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 1714, __pyx_L7_except_error)
-      __Pyx_GOTREF(__pyx_t_19);
-      if (PyDict_SetItem(__pyx_t_19, __pyx_n_s_message, __pyx_kp_s_Invalid_exception_raised_by_call) < 0) __PYX_ERR(0, 1714, __pyx_L7_except_error)
+        __pyx_t_19 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 1714, __pyx_L55_error)
+        __Pyx_GOTREF(__pyx_t_19);
+        if (PyDict_SetItem(__pyx_t_19, __pyx_n_s_message, __pyx_kp_u_Invalid_exception_raised_by_call) < 0) __PYX_ERR(0, 1714, __pyx_L55_error)
 
-      /* "pyrfc/_cyrfc.pyx":1715
+        /* "pyrfc/_cyrfc.pyx":1715
  *         new_error = ExternalRuntimeError(
  *             message="Invalid exception raised by callback function.",
  *             code=RFC_EXTERNAL_FAILURE             # <<<<<<<<<<<<<<
  *         )
  *         fillError(new_error, serverErrorInfo)
  */
-      __pyx_t_17 = __Pyx_PyInt_From_RFC_RC(RFC_EXTERNAL_FAILURE); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 1715, __pyx_L7_except_error)
-      __Pyx_GOTREF(__pyx_t_17);
-      if (PyDict_SetItem(__pyx_t_19, __pyx_n_s_code, __pyx_t_17) < 0) __PYX_ERR(0, 1714, __pyx_L7_except_error)
-      __Pyx_DECREF(__pyx_t_17); __pyx_t_17 = 0;
+        __pyx_t_17 = __Pyx_PyInt_From_RFC_RC(RFC_EXTERNAL_FAILURE); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 1715, __pyx_L55_error)
+        __Pyx_GOTREF(__pyx_t_17);
+        if (PyDict_SetItem(__pyx_t_19, __pyx_n_s_code, __pyx_t_17) < 0) __PYX_ERR(0, 1714, __pyx_L55_error)
+        __Pyx_DECREF(__pyx_t_17); __pyx_t_17 = 0;
 
-      /* "pyrfc/_cyrfc.pyx":1713
+        /* "pyrfc/_cyrfc.pyx":1713
  *             f"params: {func_handle_variables}\nrequest_context: {request_context}"
  *         )
  *         new_error = ExternalRuntimeError(             # <<<<<<<<<<<<<<
  *             message="Invalid exception raised by callback function.",
  *             code=RFC_EXTERNAL_FAILURE
  */
-      __pyx_t_17 = __Pyx_PyObject_Call(__pyx_t_9, __pyx_empty_tuple, __pyx_t_19); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 1713, __pyx_L7_except_error)
-      __Pyx_GOTREF(__pyx_t_17);
-      __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-      __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
-      __Pyx_XDECREF_SET(__pyx_v_new_error, __pyx_t_17);
-      __pyx_t_17 = 0;
+        __pyx_t_17 = __Pyx_PyObject_Call(__pyx_t_9, __pyx_empty_tuple, __pyx_t_19); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 1713, __pyx_L55_error)
+        __Pyx_GOTREF(__pyx_t_17);
+        __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+        __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
+        __Pyx_XDECREF_SET(__pyx_v_new_error, __pyx_t_17);
+        __pyx_t_17 = 0;
 
-      /* "pyrfc/_cyrfc.pyx":1717
+        /* "pyrfc/_cyrfc.pyx":1717
  *             code=RFC_EXTERNAL_FAILURE
  *         )
  *         fillError(new_error, serverErrorInfo)             # <<<<<<<<<<<<<<
  *         return RFC_EXTERNAL_FAILURE
  * 
  */
-      __pyx_t_17 = __pyx_f_5pyrfc_6_cyrfc_fillError(__pyx_v_new_error, __pyx_v_serverErrorInfo); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 1717, __pyx_L7_except_error)
-      __Pyx_GOTREF(__pyx_t_17);
-      __Pyx_DECREF(__pyx_t_17); __pyx_t_17 = 0;
+        __pyx_t_17 = __pyx_f_5pyrfc_6_cyrfc_fillError(__pyx_v_new_error, __pyx_v_serverErrorInfo); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 1717, __pyx_L55_error)
+        __Pyx_GOTREF(__pyx_t_17);
+        __Pyx_DECREF(__pyx_t_17); __pyx_t_17 = 0;
 
-      /* "pyrfc/_cyrfc.pyx":1718
+        /* "pyrfc/_cyrfc.pyx":1718
  *         )
  *         fillError(new_error, serverErrorInfo)
  *         return RFC_EXTERNAL_FAILURE             # <<<<<<<<<<<<<<
  * 
  *     return RFC_OK
  */
-      __pyx_r = RFC_EXTERNAL_FAILURE;
-      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-      goto __pyx_L8_except_return;
+        __pyx_r = RFC_EXTERNAL_FAILURE;
+        __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+        __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+        __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+        goto __pyx_L54_return;
+      }
+
+      /* "pyrfc/_cyrfc.pyx":1704
+ *         _server_log("genericHandler", f"Request for '{func_name}' raises ABAPApplicationError {e} - code set to RFC_ABAP_EXCEPTION.")
+ *         return RFC_ABAP_EXCEPTION
+ *     except Exception as ex:             # <<<<<<<<<<<<<<
+ *         exctype, value = exc_info()[:2]
+ *         _server_log(
+ */
+      /*finally:*/ {
+        __pyx_L55_error:;
+        /*exception exit:*/{
+          __Pyx_PyThreadState_declare
+          __Pyx_PyThreadState_assign
+          __pyx_t_26 = 0; __pyx_t_25 = 0; __pyx_t_24 = 0; __pyx_t_23 = 0; __pyx_t_22 = 0; __pyx_t_21 = 0;
+          __Pyx_XDECREF(__pyx_t_17); __pyx_t_17 = 0;
+          __Pyx_XDECREF(__pyx_t_18); __pyx_t_18 = 0;
+          __Pyx_XDECREF(__pyx_t_19); __pyx_t_19 = 0;
+          __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
+          __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
+          if (PY_MAJOR_VERSION >= 3) __Pyx_ExceptionSwap(&__pyx_t_23, &__pyx_t_22, &__pyx_t_21);
+          if ((PY_MAJOR_VERSION < 3) || unlikely(__Pyx_GetException(&__pyx_t_26, &__pyx_t_25, &__pyx_t_24) < 0)) __Pyx_ErrFetch(&__pyx_t_26, &__pyx_t_25, &__pyx_t_24);
+          __Pyx_XGOTREF(__pyx_t_26);
+          __Pyx_XGOTREF(__pyx_t_25);
+          __Pyx_XGOTREF(__pyx_t_24);
+          __Pyx_XGOTREF(__pyx_t_23);
+          __Pyx_XGOTREF(__pyx_t_22);
+          __Pyx_XGOTREF(__pyx_t_21);
+          __pyx_t_16 = __pyx_lineno; __pyx_t_10 = __pyx_clineno; __pyx_t_30 = __pyx_filename;
+          {
+            __Pyx_DECREF(__pyx_v_ex);
+            __pyx_v_ex = NULL;
+          }
+          if (PY_MAJOR_VERSION >= 3) {
+            __Pyx_XGIVEREF(__pyx_t_23);
+            __Pyx_XGIVEREF(__pyx_t_22);
+            __Pyx_XGIVEREF(__pyx_t_21);
+            __Pyx_ExceptionReset(__pyx_t_23, __pyx_t_22, __pyx_t_21);
+          }
+          __Pyx_XGIVEREF(__pyx_t_26);
+          __Pyx_XGIVEREF(__pyx_t_25);
+          __Pyx_XGIVEREF(__pyx_t_24);
+          __Pyx_ErrRestore(__pyx_t_26, __pyx_t_25, __pyx_t_24);
+          __pyx_t_26 = 0; __pyx_t_25 = 0; __pyx_t_24 = 0; __pyx_t_23 = 0; __pyx_t_22 = 0; __pyx_t_21 = 0;
+          __pyx_lineno = __pyx_t_16; __pyx_clineno = __pyx_t_10; __pyx_filename = __pyx_t_30;
+          goto __pyx_L7_except_error;
+        }
+        __pyx_L54_return: {
+          __pyx_t_14 = __pyx_r;
+          __Pyx_DECREF(__pyx_v_ex);
+          __pyx_v_ex = NULL;
+          __pyx_r = __pyx_t_14;
+          goto __pyx_L8_except_return;
+        }
+      }
     }
     goto __pyx_L7_except_error;
     __pyx_L7_except_error:;
 
     /* "pyrfc/_cyrfc.pyx":1637
  *     # func_desc = func_data['func_desc_handle']
  * 
@@ -22052,15 +22369,15 @@
  *         config = config or {}
  *         self.debug = config.get('debug', False)             # <<<<<<<<<<<<<<
  *         self.rstrip = config.get('rstrip', True)
  *         server_context["server_log"] = config.get("server_log", False)
  */
   __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_config, __pyx_n_s_get); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1772, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_tuple__30, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1772, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_tuple__31, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1772, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely((__pyx_t_2 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 1772, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_self->debug = __pyx_t_2;
 
   /* "pyrfc/_cyrfc.pyx":1773
@@ -22084,20 +22401,20 @@
  *         self.rstrip = config.get('rstrip', True)
  *         server_context["server_log"] = config.get("server_log", False)             # <<<<<<<<<<<<<<
  *         server_context["auth_check"] = config.get("auth_check", default_auth_check)
  *         server_context["port"] = config.get("port", 8080)
  */
   __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_config, __pyx_n_s_get); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1774, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_tuple__31, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1774, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_tuple__32, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1774, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_server_context); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1774, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (unlikely(PyObject_SetItem(__pyx_t_1, __pyx_n_s_server_log_2, __pyx_t_3) < 0)) __PYX_ERR(0, 1774, __pyx_L1_error)
+  if (unlikely(PyObject_SetItem(__pyx_t_1, __pyx_n_u_server_log_2, __pyx_t_3) < 0)) __PYX_ERR(0, 1774, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "pyrfc/_cyrfc.pyx":1775
  *         self.rstrip = config.get('rstrip', True)
  *         server_context["server_log"] = config.get("server_log", False)
  *         server_context["auth_check"] = config.get("auth_check", default_auth_check)             # <<<<<<<<<<<<<<
@@ -22118,68 +22435,68 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_1, function);
       __pyx_t_6 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_1)) {
-    PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_n_s_auth_check, __pyx_t_4};
+    PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_n_u_auth_check, __pyx_t_4};
     __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1775, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_1)) {
-    PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_n_s_auth_check, __pyx_t_4};
+    PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_n_u_auth_check, __pyx_t_4};
     __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1775, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   } else
   #endif
   {
     __pyx_t_7 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1775, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     if (__pyx_t_5) {
       __Pyx_GIVEREF(__pyx_t_5); PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_5); __pyx_t_5 = NULL;
     }
-    __Pyx_INCREF(__pyx_n_s_auth_check);
-    __Pyx_GIVEREF(__pyx_n_s_auth_check);
-    PyTuple_SET_ITEM(__pyx_t_7, 0+__pyx_t_6, __pyx_n_s_auth_check);
+    __Pyx_INCREF(__pyx_n_u_auth_check);
+    __Pyx_GIVEREF(__pyx_n_u_auth_check);
+    PyTuple_SET_ITEM(__pyx_t_7, 0+__pyx_t_6, __pyx_n_u_auth_check);
     __Pyx_GIVEREF(__pyx_t_4);
     PyTuple_SET_ITEM(__pyx_t_7, 1+__pyx_t_6, __pyx_t_4);
     __pyx_t_4 = 0;
     __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_7, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1775, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_server_context); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1775, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (unlikely(PyObject_SetItem(__pyx_t_1, __pyx_n_s_auth_check, __pyx_t_3) < 0)) __PYX_ERR(0, 1775, __pyx_L1_error)
+  if (unlikely(PyObject_SetItem(__pyx_t_1, __pyx_n_u_auth_check, __pyx_t_3) < 0)) __PYX_ERR(0, 1775, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "pyrfc/_cyrfc.pyx":1776
  *         server_context["server_log"] = config.get("server_log", False)
  *         server_context["auth_check"] = config.get("auth_check", default_auth_check)
  *         server_context["port"] = config.get("port", 8080)             # <<<<<<<<<<<<<<
  * 
  *         self._client_connection = Connection(**client_params)
  */
   __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_config, __pyx_n_s_get); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1776, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__32, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1776, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__33, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1776, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_server_context); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1776, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (unlikely(PyObject_SetItem(__pyx_t_3, __pyx_n_s_port, __pyx_t_1) < 0)) __PYX_ERR(0, 1776, __pyx_L1_error)
+  if (unlikely(PyObject_SetItem(__pyx_t_3, __pyx_n_u_port, __pyx_t_1) < 0)) __PYX_ERR(0, 1776, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "pyrfc/_cyrfc.pyx":1778
  *         server_context["port"] = config.get("port", 8080)
  * 
  *         self._client_connection = Connection(**client_params)             # <<<<<<<<<<<<<<
@@ -22307,14 +22624,22 @@
   PyObject *__pyx_t_8 = NULL;
   PyObject *__pyx_t_9 = NULL;
   PyObject *__pyx_t_10 = NULL;
   int __pyx_t_11;
   PyObject *__pyx_t_12 = NULL;
   PyObject *__pyx_t_13 = NULL;
   PyObject *__pyx_t_14 = NULL;
+  int __pyx_t_15;
+  char const *__pyx_t_16;
+  PyObject *__pyx_t_17 = NULL;
+  PyObject *__pyx_t_18 = NULL;
+  PyObject *__pyx_t_19 = NULL;
+  PyObject *__pyx_t_20 = NULL;
+  PyObject *__pyx_t_21 = NULL;
+  PyObject *__pyx_t_22 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
   #endif
   __Pyx_RefNannySetupContext("__onCheckFunction", 0);
@@ -22324,15 +22649,15 @@
  *     cdef RFC_RC __onCheckFunction(RFC_CONNECTION_HANDLE rfcHandle, const RFC_UNIT_IDENTIFIER *identifier) with gil:
  *         handler = Server.__bgRfcFunction["check"]             # <<<<<<<<<<<<<<
  *         if handler is None:
  *             return RCStatus.OK.value
  */
   __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_5pyrfc_6_cyrfc_Server), __pyx_n_s_bgRfcFunction); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1784, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_Dict_GetItem(__pyx_t_1, __pyx_n_s_check); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1784, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Dict_GetItem(__pyx_t_1, __pyx_n_u_check); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1784, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_handler = __pyx_t_2;
   __pyx_t_2 = 0;
 
   /* "pyrfc/_cyrfc.pyx":1785
  *     cdef RFC_RC __onCheckFunction(RFC_CONNECTION_HANDLE rfcHandle, const RFC_UNIT_IDENTIFIER *identifier) with gil:
@@ -22494,93 +22819,148 @@
       __Pyx_AddTraceback("pyrfc._cyrfc.Server.__onCheckFunction", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_9, &__pyx_t_2, &__pyx_t_12) < 0) __PYX_ERR(0, 1790, __pyx_L6_except_error)
       __Pyx_GOTREF(__pyx_t_9);
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_GOTREF(__pyx_t_12);
       __Pyx_INCREF(__pyx_t_2);
       __pyx_v_ex = __pyx_t_2;
+      /*try:*/ {
 
-      /* "pyrfc/_cyrfc.pyx":1791
+        /* "pyrfc/_cyrfc.pyx":1791
  *             return handler(<uintptr_t>rfcHandle, unit_identifier).value
  *         except Exception as ex:
  *             _server_log("Error in bgRFC handler onCheck:", ex)             # <<<<<<<<<<<<<<
  *             return RCStatus.RFC_EXTERNAL_FAILURE.value
  * 
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_server_log); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1791, __pyx_L6_except_error)
-      __Pyx_GOTREF(__pyx_t_10);
-      __pyx_t_13 = NULL;
-      __pyx_t_11 = 0;
-      if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_10))) {
-        __pyx_t_13 = PyMethod_GET_SELF(__pyx_t_10);
-        if (likely(__pyx_t_13)) {
-          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_10);
-          __Pyx_INCREF(__pyx_t_13);
-          __Pyx_INCREF(function);
-          __Pyx_DECREF_SET(__pyx_t_10, function);
-          __pyx_t_11 = 1;
+        __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_server_log); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1791, __pyx_L15_error)
+        __Pyx_GOTREF(__pyx_t_10);
+        __pyx_t_13 = NULL;
+        __pyx_t_11 = 0;
+        if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_10))) {
+          __pyx_t_13 = PyMethod_GET_SELF(__pyx_t_10);
+          if (likely(__pyx_t_13)) {
+            PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_10);
+            __Pyx_INCREF(__pyx_t_13);
+            __Pyx_INCREF(function);
+            __Pyx_DECREF_SET(__pyx_t_10, function);
+            __pyx_t_11 = 1;
+          }
         }
-      }
-      #if CYTHON_FAST_PYCALL
-      if (PyFunction_Check(__pyx_t_10)) {
-        PyObject *__pyx_temp[3] = {__pyx_t_13, __pyx_kp_s_Error_in_bgRFC_handler_onCheck, __pyx_v_ex};
-        __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_10, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1791, __pyx_L6_except_error)
-        __Pyx_XDECREF(__pyx_t_13); __pyx_t_13 = 0;
-        __Pyx_GOTREF(__pyx_t_1);
-      } else
-      #endif
-      #if CYTHON_FAST_PYCCALL
-      if (__Pyx_PyFastCFunction_Check(__pyx_t_10)) {
-        PyObject *__pyx_temp[3] = {__pyx_t_13, __pyx_kp_s_Error_in_bgRFC_handler_onCheck, __pyx_v_ex};
-        __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_10, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1791, __pyx_L6_except_error)
-        __Pyx_XDECREF(__pyx_t_13); __pyx_t_13 = 0;
-        __Pyx_GOTREF(__pyx_t_1);
-      } else
-      #endif
-      {
-        __pyx_t_14 = PyTuple_New(2+__pyx_t_11); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 1791, __pyx_L6_except_error)
-        __Pyx_GOTREF(__pyx_t_14);
-        if (__pyx_t_13) {
-          __Pyx_GIVEREF(__pyx_t_13); PyTuple_SET_ITEM(__pyx_t_14, 0, __pyx_t_13); __pyx_t_13 = NULL;
-        }
-        __Pyx_INCREF(__pyx_kp_s_Error_in_bgRFC_handler_onCheck);
-        __Pyx_GIVEREF(__pyx_kp_s_Error_in_bgRFC_handler_onCheck);
-        PyTuple_SET_ITEM(__pyx_t_14, 0+__pyx_t_11, __pyx_kp_s_Error_in_bgRFC_handler_onCheck);
-        __Pyx_INCREF(__pyx_v_ex);
-        __Pyx_GIVEREF(__pyx_v_ex);
-        PyTuple_SET_ITEM(__pyx_t_14, 1+__pyx_t_11, __pyx_v_ex);
-        __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_10, __pyx_t_14, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1791, __pyx_L6_except_error)
-        __Pyx_GOTREF(__pyx_t_1);
-        __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
-      }
-      __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+        #if CYTHON_FAST_PYCALL
+        if (PyFunction_Check(__pyx_t_10)) {
+          PyObject *__pyx_temp[3] = {__pyx_t_13, __pyx_kp_u_Error_in_bgRFC_handler_onCheck, __pyx_v_ex};
+          __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_10, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1791, __pyx_L15_error)
+          __Pyx_XDECREF(__pyx_t_13); __pyx_t_13 = 0;
+          __Pyx_GOTREF(__pyx_t_1);
+        } else
+        #endif
+        #if CYTHON_FAST_PYCCALL
+        if (__Pyx_PyFastCFunction_Check(__pyx_t_10)) {
+          PyObject *__pyx_temp[3] = {__pyx_t_13, __pyx_kp_u_Error_in_bgRFC_handler_onCheck, __pyx_v_ex};
+          __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_10, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1791, __pyx_L15_error)
+          __Pyx_XDECREF(__pyx_t_13); __pyx_t_13 = 0;
+          __Pyx_GOTREF(__pyx_t_1);
+        } else
+        #endif
+        {
+          __pyx_t_14 = PyTuple_New(2+__pyx_t_11); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 1791, __pyx_L15_error)
+          __Pyx_GOTREF(__pyx_t_14);
+          if (__pyx_t_13) {
+            __Pyx_GIVEREF(__pyx_t_13); PyTuple_SET_ITEM(__pyx_t_14, 0, __pyx_t_13); __pyx_t_13 = NULL;
+          }
+          __Pyx_INCREF(__pyx_kp_u_Error_in_bgRFC_handler_onCheck);
+          __Pyx_GIVEREF(__pyx_kp_u_Error_in_bgRFC_handler_onCheck);
+          PyTuple_SET_ITEM(__pyx_t_14, 0+__pyx_t_11, __pyx_kp_u_Error_in_bgRFC_handler_onCheck);
+          __Pyx_INCREF(__pyx_v_ex);
+          __Pyx_GIVEREF(__pyx_v_ex);
+          PyTuple_SET_ITEM(__pyx_t_14, 1+__pyx_t_11, __pyx_v_ex);
+          __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_10, __pyx_t_14, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1791, __pyx_L15_error)
+          __Pyx_GOTREF(__pyx_t_1);
+          __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
+        }
+        __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+        __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-      /* "pyrfc/_cyrfc.pyx":1792
+        /* "pyrfc/_cyrfc.pyx":1792
  *         except Exception as ex:
  *             _server_log("Error in bgRFC handler onCheck:", ex)
  *             return RCStatus.RFC_EXTERNAL_FAILURE.value             # <<<<<<<<<<<<<<
  * 
  *     @staticmethod
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_RCStatus); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1792, __pyx_L6_except_error)
-      __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_RFC_EXTERNAL_FAILURE); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1792, __pyx_L6_except_error)
-      __Pyx_GOTREF(__pyx_t_10);
-      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_10, __pyx_n_s_value); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1792, __pyx_L6_except_error)
-      __Pyx_GOTREF(__pyx_t_1);
-      __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-      __pyx_t_5 = ((RFC_RC)__Pyx_PyInt_As_RFC_RC(__pyx_t_1)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1792, __pyx_L6_except_error)
-      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __pyx_r = __pyx_t_5;
-      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-      __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-      __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-      goto __pyx_L7_except_return;
+        __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_RCStatus); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1792, __pyx_L15_error)
+        __Pyx_GOTREF(__pyx_t_1);
+        __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_RFC_EXTERNAL_FAILURE); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1792, __pyx_L15_error)
+        __Pyx_GOTREF(__pyx_t_10);
+        __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+        __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_10, __pyx_n_s_value); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1792, __pyx_L15_error)
+        __Pyx_GOTREF(__pyx_t_1);
+        __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+        __pyx_t_5 = ((RFC_RC)__Pyx_PyInt_As_RFC_RC(__pyx_t_1)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1792, __pyx_L15_error)
+        __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+        __pyx_r = __pyx_t_5;
+        __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+        __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+        __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+        goto __pyx_L14_return;
+      }
+
+      /* "pyrfc/_cyrfc.pyx":1790
+ *             unit_identifier = wrapUnitIdentifier(identifier[0])
+ *             return handler(<uintptr_t>rfcHandle, unit_identifier).value
+ *         except Exception as ex:             # <<<<<<<<<<<<<<
+ *             _server_log("Error in bgRFC handler onCheck:", ex)
+ *             return RCStatus.RFC_EXTERNAL_FAILURE.value
+ */
+      /*finally:*/ {
+        __pyx_L15_error:;
+        /*exception exit:*/{
+          __Pyx_PyThreadState_declare
+          __Pyx_PyThreadState_assign
+          __pyx_t_17 = 0; __pyx_t_18 = 0; __pyx_t_19 = 0; __pyx_t_20 = 0; __pyx_t_21 = 0; __pyx_t_22 = 0;
+          __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
+          __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
+          __Pyx_XDECREF(__pyx_t_13); __pyx_t_13 = 0;
+          __Pyx_XDECREF(__pyx_t_14); __pyx_t_14 = 0;
+          if (PY_MAJOR_VERSION >= 3) __Pyx_ExceptionSwap(&__pyx_t_20, &__pyx_t_21, &__pyx_t_22);
+          if ((PY_MAJOR_VERSION < 3) || unlikely(__Pyx_GetException(&__pyx_t_17, &__pyx_t_18, &__pyx_t_19) < 0)) __Pyx_ErrFetch(&__pyx_t_17, &__pyx_t_18, &__pyx_t_19);
+          __Pyx_XGOTREF(__pyx_t_17);
+          __Pyx_XGOTREF(__pyx_t_18);
+          __Pyx_XGOTREF(__pyx_t_19);
+          __Pyx_XGOTREF(__pyx_t_20);
+          __Pyx_XGOTREF(__pyx_t_21);
+          __Pyx_XGOTREF(__pyx_t_22);
+          __pyx_t_11 = __pyx_lineno; __pyx_t_15 = __pyx_clineno; __pyx_t_16 = __pyx_filename;
+          {
+            __Pyx_DECREF(__pyx_v_ex);
+            __pyx_v_ex = NULL;
+          }
+          if (PY_MAJOR_VERSION >= 3) {
+            __Pyx_XGIVEREF(__pyx_t_20);
+            __Pyx_XGIVEREF(__pyx_t_21);
+            __Pyx_XGIVEREF(__pyx_t_22);
+            __Pyx_ExceptionReset(__pyx_t_20, __pyx_t_21, __pyx_t_22);
+          }
+          __Pyx_XGIVEREF(__pyx_t_17);
+          __Pyx_XGIVEREF(__pyx_t_18);
+          __Pyx_XGIVEREF(__pyx_t_19);
+          __Pyx_ErrRestore(__pyx_t_17, __pyx_t_18, __pyx_t_19);
+          __pyx_t_17 = 0; __pyx_t_18 = 0; __pyx_t_19 = 0; __pyx_t_20 = 0; __pyx_t_21 = 0; __pyx_t_22 = 0;
+          __pyx_lineno = __pyx_t_11; __pyx_clineno = __pyx_t_15; __pyx_filename = __pyx_t_16;
+          goto __pyx_L6_except_error;
+        }
+        __pyx_L14_return: {
+          __pyx_t_5 = __pyx_r;
+          __Pyx_DECREF(__pyx_v_ex);
+          __pyx_v_ex = NULL;
+          __pyx_r = __pyx_t_5;
+          goto __pyx_L7_except_return;
+        }
+      }
     }
     goto __pyx_L6_except_error;
     __pyx_L6_except_error:;
 
     /* "pyrfc/_cyrfc.pyx":1787
  *         if handler is None:
  *             return RCStatus.OK.value
@@ -22661,14 +23041,22 @@
   PyObject *__pyx_t_8 = NULL;
   PyObject *__pyx_t_9 = NULL;
   PyObject *__pyx_t_10 = NULL;
   int __pyx_t_11;
   PyObject *__pyx_t_12 = NULL;
   PyObject *__pyx_t_13 = NULL;
   PyObject *__pyx_t_14 = NULL;
+  int __pyx_t_15;
+  char const *__pyx_t_16;
+  PyObject *__pyx_t_17 = NULL;
+  PyObject *__pyx_t_18 = NULL;
+  PyObject *__pyx_t_19 = NULL;
+  PyObject *__pyx_t_20 = NULL;
+  PyObject *__pyx_t_21 = NULL;
+  PyObject *__pyx_t_22 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
   #endif
   __Pyx_RefNannySetupContext("__onCommitFunction", 0);
@@ -22678,15 +23066,15 @@
  *     cdef RFC_RC __onCommitFunction(RFC_CONNECTION_HANDLE rfcHandle, const RFC_UNIT_IDENTIFIER *identifier) with gil:
  *         handler = Server.__bgRfcFunction["commit"]             # <<<<<<<<<<<<<<
  *         if handler is None:
  *             return RCStatus.OK.value
  */
   __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_5pyrfc_6_cyrfc_Server), __pyx_n_s_bgRfcFunction); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1796, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_Dict_GetItem(__pyx_t_1, __pyx_n_s_commit); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1796, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Dict_GetItem(__pyx_t_1, __pyx_n_u_commit); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1796, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_handler = __pyx_t_2;
   __pyx_t_2 = 0;
 
   /* "pyrfc/_cyrfc.pyx":1797
  *     cdef RFC_RC __onCommitFunction(RFC_CONNECTION_HANDLE rfcHandle, const RFC_UNIT_IDENTIFIER *identifier) with gil:
@@ -22848,93 +23236,148 @@
       __Pyx_AddTraceback("pyrfc._cyrfc.Server.__onCommitFunction", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_9, &__pyx_t_2, &__pyx_t_12) < 0) __PYX_ERR(0, 1802, __pyx_L6_except_error)
       __Pyx_GOTREF(__pyx_t_9);
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_GOTREF(__pyx_t_12);
       __Pyx_INCREF(__pyx_t_2);
       __pyx_v_ex = __pyx_t_2;
+      /*try:*/ {
 
-      /* "pyrfc/_cyrfc.pyx":1803
+        /* "pyrfc/_cyrfc.pyx":1803
  *             return handler(<uintptr_t>rfcHandle, unit_identifier).value
  *         except Exception as ex:
  *             _server_log("Error in bgRFC handler onCommit:", ex)             # <<<<<<<<<<<<<<
  *             return RCStatus.RFC_EXTERNAL_FAILURE.value
  * 
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_server_log); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1803, __pyx_L6_except_error)
-      __Pyx_GOTREF(__pyx_t_10);
-      __pyx_t_13 = NULL;
-      __pyx_t_11 = 0;
-      if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_10))) {
-        __pyx_t_13 = PyMethod_GET_SELF(__pyx_t_10);
-        if (likely(__pyx_t_13)) {
-          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_10);
-          __Pyx_INCREF(__pyx_t_13);
-          __Pyx_INCREF(function);
-          __Pyx_DECREF_SET(__pyx_t_10, function);
-          __pyx_t_11 = 1;
+        __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_server_log); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1803, __pyx_L15_error)
+        __Pyx_GOTREF(__pyx_t_10);
+        __pyx_t_13 = NULL;
+        __pyx_t_11 = 0;
+        if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_10))) {
+          __pyx_t_13 = PyMethod_GET_SELF(__pyx_t_10);
+          if (likely(__pyx_t_13)) {
+            PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_10);
+            __Pyx_INCREF(__pyx_t_13);
+            __Pyx_INCREF(function);
+            __Pyx_DECREF_SET(__pyx_t_10, function);
+            __pyx_t_11 = 1;
+          }
         }
-      }
-      #if CYTHON_FAST_PYCALL
-      if (PyFunction_Check(__pyx_t_10)) {
-        PyObject *__pyx_temp[3] = {__pyx_t_13, __pyx_kp_s_Error_in_bgRFC_handler_onCommit, __pyx_v_ex};
-        __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_10, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1803, __pyx_L6_except_error)
-        __Pyx_XDECREF(__pyx_t_13); __pyx_t_13 = 0;
-        __Pyx_GOTREF(__pyx_t_1);
-      } else
-      #endif
-      #if CYTHON_FAST_PYCCALL
-      if (__Pyx_PyFastCFunction_Check(__pyx_t_10)) {
-        PyObject *__pyx_temp[3] = {__pyx_t_13, __pyx_kp_s_Error_in_bgRFC_handler_onCommit, __pyx_v_ex};
-        __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_10, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1803, __pyx_L6_except_error)
-        __Pyx_XDECREF(__pyx_t_13); __pyx_t_13 = 0;
-        __Pyx_GOTREF(__pyx_t_1);
-      } else
-      #endif
-      {
-        __pyx_t_14 = PyTuple_New(2+__pyx_t_11); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 1803, __pyx_L6_except_error)
-        __Pyx_GOTREF(__pyx_t_14);
-        if (__pyx_t_13) {
-          __Pyx_GIVEREF(__pyx_t_13); PyTuple_SET_ITEM(__pyx_t_14, 0, __pyx_t_13); __pyx_t_13 = NULL;
-        }
-        __Pyx_INCREF(__pyx_kp_s_Error_in_bgRFC_handler_onCommit);
-        __Pyx_GIVEREF(__pyx_kp_s_Error_in_bgRFC_handler_onCommit);
-        PyTuple_SET_ITEM(__pyx_t_14, 0+__pyx_t_11, __pyx_kp_s_Error_in_bgRFC_handler_onCommit);
-        __Pyx_INCREF(__pyx_v_ex);
-        __Pyx_GIVEREF(__pyx_v_ex);
-        PyTuple_SET_ITEM(__pyx_t_14, 1+__pyx_t_11, __pyx_v_ex);
-        __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_10, __pyx_t_14, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1803, __pyx_L6_except_error)
-        __Pyx_GOTREF(__pyx_t_1);
-        __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
-      }
-      __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+        #if CYTHON_FAST_PYCALL
+        if (PyFunction_Check(__pyx_t_10)) {
+          PyObject *__pyx_temp[3] = {__pyx_t_13, __pyx_kp_u_Error_in_bgRFC_handler_onCommit, __pyx_v_ex};
+          __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_10, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1803, __pyx_L15_error)
+          __Pyx_XDECREF(__pyx_t_13); __pyx_t_13 = 0;
+          __Pyx_GOTREF(__pyx_t_1);
+        } else
+        #endif
+        #if CYTHON_FAST_PYCCALL
+        if (__Pyx_PyFastCFunction_Check(__pyx_t_10)) {
+          PyObject *__pyx_temp[3] = {__pyx_t_13, __pyx_kp_u_Error_in_bgRFC_handler_onCommit, __pyx_v_ex};
+          __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_10, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1803, __pyx_L15_error)
+          __Pyx_XDECREF(__pyx_t_13); __pyx_t_13 = 0;
+          __Pyx_GOTREF(__pyx_t_1);
+        } else
+        #endif
+        {
+          __pyx_t_14 = PyTuple_New(2+__pyx_t_11); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 1803, __pyx_L15_error)
+          __Pyx_GOTREF(__pyx_t_14);
+          if (__pyx_t_13) {
+            __Pyx_GIVEREF(__pyx_t_13); PyTuple_SET_ITEM(__pyx_t_14, 0, __pyx_t_13); __pyx_t_13 = NULL;
+          }
+          __Pyx_INCREF(__pyx_kp_u_Error_in_bgRFC_handler_onCommit);
+          __Pyx_GIVEREF(__pyx_kp_u_Error_in_bgRFC_handler_onCommit);
+          PyTuple_SET_ITEM(__pyx_t_14, 0+__pyx_t_11, __pyx_kp_u_Error_in_bgRFC_handler_onCommit);
+          __Pyx_INCREF(__pyx_v_ex);
+          __Pyx_GIVEREF(__pyx_v_ex);
+          PyTuple_SET_ITEM(__pyx_t_14, 1+__pyx_t_11, __pyx_v_ex);
+          __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_10, __pyx_t_14, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1803, __pyx_L15_error)
+          __Pyx_GOTREF(__pyx_t_1);
+          __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
+        }
+        __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+        __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-      /* "pyrfc/_cyrfc.pyx":1804
+        /* "pyrfc/_cyrfc.pyx":1804
  *         except Exception as ex:
  *             _server_log("Error in bgRFC handler onCommit:", ex)
  *             return RCStatus.RFC_EXTERNAL_FAILURE.value             # <<<<<<<<<<<<<<
  * 
  *     @staticmethod
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_RCStatus); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1804, __pyx_L6_except_error)
-      __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_RFC_EXTERNAL_FAILURE); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1804, __pyx_L6_except_error)
-      __Pyx_GOTREF(__pyx_t_10);
-      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_10, __pyx_n_s_value); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1804, __pyx_L6_except_error)
-      __Pyx_GOTREF(__pyx_t_1);
-      __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-      __pyx_t_5 = ((RFC_RC)__Pyx_PyInt_As_RFC_RC(__pyx_t_1)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1804, __pyx_L6_except_error)
-      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __pyx_r = __pyx_t_5;
-      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-      __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-      __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-      goto __pyx_L7_except_return;
+        __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_RCStatus); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1804, __pyx_L15_error)
+        __Pyx_GOTREF(__pyx_t_1);
+        __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_RFC_EXTERNAL_FAILURE); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1804, __pyx_L15_error)
+        __Pyx_GOTREF(__pyx_t_10);
+        __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+        __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_10, __pyx_n_s_value); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1804, __pyx_L15_error)
+        __Pyx_GOTREF(__pyx_t_1);
+        __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+        __pyx_t_5 = ((RFC_RC)__Pyx_PyInt_As_RFC_RC(__pyx_t_1)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1804, __pyx_L15_error)
+        __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+        __pyx_r = __pyx_t_5;
+        __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+        __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+        __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+        goto __pyx_L14_return;
+      }
+
+      /* "pyrfc/_cyrfc.pyx":1802
+ *             unit_identifier = wrapUnitIdentifier(identifier[0])
+ *             return handler(<uintptr_t>rfcHandle, unit_identifier).value
+ *         except Exception as ex:             # <<<<<<<<<<<<<<
+ *             _server_log("Error in bgRFC handler onCommit:", ex)
+ *             return RCStatus.RFC_EXTERNAL_FAILURE.value
+ */
+      /*finally:*/ {
+        __pyx_L15_error:;
+        /*exception exit:*/{
+          __Pyx_PyThreadState_declare
+          __Pyx_PyThreadState_assign
+          __pyx_t_17 = 0; __pyx_t_18 = 0; __pyx_t_19 = 0; __pyx_t_20 = 0; __pyx_t_21 = 0; __pyx_t_22 = 0;
+          __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
+          __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
+          __Pyx_XDECREF(__pyx_t_13); __pyx_t_13 = 0;
+          __Pyx_XDECREF(__pyx_t_14); __pyx_t_14 = 0;
+          if (PY_MAJOR_VERSION >= 3) __Pyx_ExceptionSwap(&__pyx_t_20, &__pyx_t_21, &__pyx_t_22);
+          if ((PY_MAJOR_VERSION < 3) || unlikely(__Pyx_GetException(&__pyx_t_17, &__pyx_t_18, &__pyx_t_19) < 0)) __Pyx_ErrFetch(&__pyx_t_17, &__pyx_t_18, &__pyx_t_19);
+          __Pyx_XGOTREF(__pyx_t_17);
+          __Pyx_XGOTREF(__pyx_t_18);
+          __Pyx_XGOTREF(__pyx_t_19);
+          __Pyx_XGOTREF(__pyx_t_20);
+          __Pyx_XGOTREF(__pyx_t_21);
+          __Pyx_XGOTREF(__pyx_t_22);
+          __pyx_t_11 = __pyx_lineno; __pyx_t_15 = __pyx_clineno; __pyx_t_16 = __pyx_filename;
+          {
+            __Pyx_DECREF(__pyx_v_ex);
+            __pyx_v_ex = NULL;
+          }
+          if (PY_MAJOR_VERSION >= 3) {
+            __Pyx_XGIVEREF(__pyx_t_20);
+            __Pyx_XGIVEREF(__pyx_t_21);
+            __Pyx_XGIVEREF(__pyx_t_22);
+            __Pyx_ExceptionReset(__pyx_t_20, __pyx_t_21, __pyx_t_22);
+          }
+          __Pyx_XGIVEREF(__pyx_t_17);
+          __Pyx_XGIVEREF(__pyx_t_18);
+          __Pyx_XGIVEREF(__pyx_t_19);
+          __Pyx_ErrRestore(__pyx_t_17, __pyx_t_18, __pyx_t_19);
+          __pyx_t_17 = 0; __pyx_t_18 = 0; __pyx_t_19 = 0; __pyx_t_20 = 0; __pyx_t_21 = 0; __pyx_t_22 = 0;
+          __pyx_lineno = __pyx_t_11; __pyx_clineno = __pyx_t_15; __pyx_filename = __pyx_t_16;
+          goto __pyx_L6_except_error;
+        }
+        __pyx_L14_return: {
+          __pyx_t_5 = __pyx_r;
+          __Pyx_DECREF(__pyx_v_ex);
+          __pyx_v_ex = NULL;
+          __pyx_r = __pyx_t_5;
+          goto __pyx_L7_except_return;
+        }
+      }
     }
     goto __pyx_L6_except_error;
     __pyx_L6_except_error:;
 
     /* "pyrfc/_cyrfc.pyx":1799
  *         if handler is None:
  *             return RCStatus.OK.value
@@ -23015,14 +23458,22 @@
   PyObject *__pyx_t_8 = NULL;
   PyObject *__pyx_t_9 = NULL;
   PyObject *__pyx_t_10 = NULL;
   int __pyx_t_11;
   PyObject *__pyx_t_12 = NULL;
   PyObject *__pyx_t_13 = NULL;
   PyObject *__pyx_t_14 = NULL;
+  int __pyx_t_15;
+  char const *__pyx_t_16;
+  PyObject *__pyx_t_17 = NULL;
+  PyObject *__pyx_t_18 = NULL;
+  PyObject *__pyx_t_19 = NULL;
+  PyObject *__pyx_t_20 = NULL;
+  PyObject *__pyx_t_21 = NULL;
+  PyObject *__pyx_t_22 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
   #endif
   __Pyx_RefNannySetupContext("__onRollbackFunction", 0);
@@ -23032,15 +23483,15 @@
  *     cdef RFC_RC __onRollbackFunction(RFC_CONNECTION_HANDLE rfcHandle, const RFC_UNIT_IDENTIFIER *identifier) with gil:
  *         handler = Server.__bgRfcFunction["rollback"]             # <<<<<<<<<<<<<<
  *         if handler is None:
  *             return RCStatus.OK.value
  */
   __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_5pyrfc_6_cyrfc_Server), __pyx_n_s_bgRfcFunction); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1808, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_Dict_GetItem(__pyx_t_1, __pyx_n_s_rollback); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1808, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Dict_GetItem(__pyx_t_1, __pyx_n_u_rollback); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1808, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_handler = __pyx_t_2;
   __pyx_t_2 = 0;
 
   /* "pyrfc/_cyrfc.pyx":1809
  *     cdef RFC_RC __onRollbackFunction(RFC_CONNECTION_HANDLE rfcHandle, const RFC_UNIT_IDENTIFIER *identifier) with gil:
@@ -23202,93 +23653,148 @@
       __Pyx_AddTraceback("pyrfc._cyrfc.Server.__onRollbackFunction", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_9, &__pyx_t_2, &__pyx_t_12) < 0) __PYX_ERR(0, 1814, __pyx_L6_except_error)
       __Pyx_GOTREF(__pyx_t_9);
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_GOTREF(__pyx_t_12);
       __Pyx_INCREF(__pyx_t_2);
       __pyx_v_ex = __pyx_t_2;
+      /*try:*/ {
 
-      /* "pyrfc/_cyrfc.pyx":1815
+        /* "pyrfc/_cyrfc.pyx":1815
  *             return handler(<uintptr_t>rfcHandle, unit_identifier).value
  *         except Exception as ex:
  *             _server_log("Error in bgRFC handler onRollback:", ex)             # <<<<<<<<<<<<<<
  *             return RCStatus.RFC_EXTERNAL_FAILURE.value
  * 
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_server_log); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1815, __pyx_L6_except_error)
-      __Pyx_GOTREF(__pyx_t_10);
-      __pyx_t_13 = NULL;
-      __pyx_t_11 = 0;
-      if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_10))) {
-        __pyx_t_13 = PyMethod_GET_SELF(__pyx_t_10);
-        if (likely(__pyx_t_13)) {
-          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_10);
-          __Pyx_INCREF(__pyx_t_13);
-          __Pyx_INCREF(function);
-          __Pyx_DECREF_SET(__pyx_t_10, function);
-          __pyx_t_11 = 1;
+        __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_server_log); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1815, __pyx_L15_error)
+        __Pyx_GOTREF(__pyx_t_10);
+        __pyx_t_13 = NULL;
+        __pyx_t_11 = 0;
+        if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_10))) {
+          __pyx_t_13 = PyMethod_GET_SELF(__pyx_t_10);
+          if (likely(__pyx_t_13)) {
+            PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_10);
+            __Pyx_INCREF(__pyx_t_13);
+            __Pyx_INCREF(function);
+            __Pyx_DECREF_SET(__pyx_t_10, function);
+            __pyx_t_11 = 1;
+          }
         }
-      }
-      #if CYTHON_FAST_PYCALL
-      if (PyFunction_Check(__pyx_t_10)) {
-        PyObject *__pyx_temp[3] = {__pyx_t_13, __pyx_kp_s_Error_in_bgRFC_handler_onRollbac, __pyx_v_ex};
-        __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_10, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1815, __pyx_L6_except_error)
-        __Pyx_XDECREF(__pyx_t_13); __pyx_t_13 = 0;
-        __Pyx_GOTREF(__pyx_t_1);
-      } else
-      #endif
-      #if CYTHON_FAST_PYCCALL
-      if (__Pyx_PyFastCFunction_Check(__pyx_t_10)) {
-        PyObject *__pyx_temp[3] = {__pyx_t_13, __pyx_kp_s_Error_in_bgRFC_handler_onRollbac, __pyx_v_ex};
-        __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_10, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1815, __pyx_L6_except_error)
-        __Pyx_XDECREF(__pyx_t_13); __pyx_t_13 = 0;
-        __Pyx_GOTREF(__pyx_t_1);
-      } else
-      #endif
-      {
-        __pyx_t_14 = PyTuple_New(2+__pyx_t_11); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 1815, __pyx_L6_except_error)
-        __Pyx_GOTREF(__pyx_t_14);
-        if (__pyx_t_13) {
-          __Pyx_GIVEREF(__pyx_t_13); PyTuple_SET_ITEM(__pyx_t_14, 0, __pyx_t_13); __pyx_t_13 = NULL;
-        }
-        __Pyx_INCREF(__pyx_kp_s_Error_in_bgRFC_handler_onRollbac);
-        __Pyx_GIVEREF(__pyx_kp_s_Error_in_bgRFC_handler_onRollbac);
-        PyTuple_SET_ITEM(__pyx_t_14, 0+__pyx_t_11, __pyx_kp_s_Error_in_bgRFC_handler_onRollbac);
-        __Pyx_INCREF(__pyx_v_ex);
-        __Pyx_GIVEREF(__pyx_v_ex);
-        PyTuple_SET_ITEM(__pyx_t_14, 1+__pyx_t_11, __pyx_v_ex);
-        __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_10, __pyx_t_14, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1815, __pyx_L6_except_error)
-        __Pyx_GOTREF(__pyx_t_1);
-        __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
-      }
-      __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+        #if CYTHON_FAST_PYCALL
+        if (PyFunction_Check(__pyx_t_10)) {
+          PyObject *__pyx_temp[3] = {__pyx_t_13, __pyx_kp_u_Error_in_bgRFC_handler_onRollbac, __pyx_v_ex};
+          __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_10, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1815, __pyx_L15_error)
+          __Pyx_XDECREF(__pyx_t_13); __pyx_t_13 = 0;
+          __Pyx_GOTREF(__pyx_t_1);
+        } else
+        #endif
+        #if CYTHON_FAST_PYCCALL
+        if (__Pyx_PyFastCFunction_Check(__pyx_t_10)) {
+          PyObject *__pyx_temp[3] = {__pyx_t_13, __pyx_kp_u_Error_in_bgRFC_handler_onRollbac, __pyx_v_ex};
+          __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_10, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1815, __pyx_L15_error)
+          __Pyx_XDECREF(__pyx_t_13); __pyx_t_13 = 0;
+          __Pyx_GOTREF(__pyx_t_1);
+        } else
+        #endif
+        {
+          __pyx_t_14 = PyTuple_New(2+__pyx_t_11); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 1815, __pyx_L15_error)
+          __Pyx_GOTREF(__pyx_t_14);
+          if (__pyx_t_13) {
+            __Pyx_GIVEREF(__pyx_t_13); PyTuple_SET_ITEM(__pyx_t_14, 0, __pyx_t_13); __pyx_t_13 = NULL;
+          }
+          __Pyx_INCREF(__pyx_kp_u_Error_in_bgRFC_handler_onRollbac);
+          __Pyx_GIVEREF(__pyx_kp_u_Error_in_bgRFC_handler_onRollbac);
+          PyTuple_SET_ITEM(__pyx_t_14, 0+__pyx_t_11, __pyx_kp_u_Error_in_bgRFC_handler_onRollbac);
+          __Pyx_INCREF(__pyx_v_ex);
+          __Pyx_GIVEREF(__pyx_v_ex);
+          PyTuple_SET_ITEM(__pyx_t_14, 1+__pyx_t_11, __pyx_v_ex);
+          __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_10, __pyx_t_14, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1815, __pyx_L15_error)
+          __Pyx_GOTREF(__pyx_t_1);
+          __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
+        }
+        __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+        __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-      /* "pyrfc/_cyrfc.pyx":1816
+        /* "pyrfc/_cyrfc.pyx":1816
  *         except Exception as ex:
  *             _server_log("Error in bgRFC handler onRollback:", ex)
  *             return RCStatus.RFC_EXTERNAL_FAILURE.value             # <<<<<<<<<<<<<<
  * 
  *     @staticmethod
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_RCStatus); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1816, __pyx_L6_except_error)
-      __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_RFC_EXTERNAL_FAILURE); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1816, __pyx_L6_except_error)
-      __Pyx_GOTREF(__pyx_t_10);
-      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_10, __pyx_n_s_value); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1816, __pyx_L6_except_error)
-      __Pyx_GOTREF(__pyx_t_1);
-      __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-      __pyx_t_5 = ((RFC_RC)__Pyx_PyInt_As_RFC_RC(__pyx_t_1)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1816, __pyx_L6_except_error)
-      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __pyx_r = __pyx_t_5;
-      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-      __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-      __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-      goto __pyx_L7_except_return;
+        __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_RCStatus); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1816, __pyx_L15_error)
+        __Pyx_GOTREF(__pyx_t_1);
+        __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_RFC_EXTERNAL_FAILURE); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1816, __pyx_L15_error)
+        __Pyx_GOTREF(__pyx_t_10);
+        __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+        __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_10, __pyx_n_s_value); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1816, __pyx_L15_error)
+        __Pyx_GOTREF(__pyx_t_1);
+        __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+        __pyx_t_5 = ((RFC_RC)__Pyx_PyInt_As_RFC_RC(__pyx_t_1)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1816, __pyx_L15_error)
+        __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+        __pyx_r = __pyx_t_5;
+        __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+        __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+        __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+        goto __pyx_L14_return;
+      }
+
+      /* "pyrfc/_cyrfc.pyx":1814
+ *             unit_identifier = wrapUnitIdentifier(identifier[0])
+ *             return handler(<uintptr_t>rfcHandle, unit_identifier).value
+ *         except Exception as ex:             # <<<<<<<<<<<<<<
+ *             _server_log("Error in bgRFC handler onRollback:", ex)
+ *             return RCStatus.RFC_EXTERNAL_FAILURE.value
+ */
+      /*finally:*/ {
+        __pyx_L15_error:;
+        /*exception exit:*/{
+          __Pyx_PyThreadState_declare
+          __Pyx_PyThreadState_assign
+          __pyx_t_17 = 0; __pyx_t_18 = 0; __pyx_t_19 = 0; __pyx_t_20 = 0; __pyx_t_21 = 0; __pyx_t_22 = 0;
+          __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
+          __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
+          __Pyx_XDECREF(__pyx_t_13); __pyx_t_13 = 0;
+          __Pyx_XDECREF(__pyx_t_14); __pyx_t_14 = 0;
+          if (PY_MAJOR_VERSION >= 3) __Pyx_ExceptionSwap(&__pyx_t_20, &__pyx_t_21, &__pyx_t_22);
+          if ((PY_MAJOR_VERSION < 3) || unlikely(__Pyx_GetException(&__pyx_t_17, &__pyx_t_18, &__pyx_t_19) < 0)) __Pyx_ErrFetch(&__pyx_t_17, &__pyx_t_18, &__pyx_t_19);
+          __Pyx_XGOTREF(__pyx_t_17);
+          __Pyx_XGOTREF(__pyx_t_18);
+          __Pyx_XGOTREF(__pyx_t_19);
+          __Pyx_XGOTREF(__pyx_t_20);
+          __Pyx_XGOTREF(__pyx_t_21);
+          __Pyx_XGOTREF(__pyx_t_22);
+          __pyx_t_11 = __pyx_lineno; __pyx_t_15 = __pyx_clineno; __pyx_t_16 = __pyx_filename;
+          {
+            __Pyx_DECREF(__pyx_v_ex);
+            __pyx_v_ex = NULL;
+          }
+          if (PY_MAJOR_VERSION >= 3) {
+            __Pyx_XGIVEREF(__pyx_t_20);
+            __Pyx_XGIVEREF(__pyx_t_21);
+            __Pyx_XGIVEREF(__pyx_t_22);
+            __Pyx_ExceptionReset(__pyx_t_20, __pyx_t_21, __pyx_t_22);
+          }
+          __Pyx_XGIVEREF(__pyx_t_17);
+          __Pyx_XGIVEREF(__pyx_t_18);
+          __Pyx_XGIVEREF(__pyx_t_19);
+          __Pyx_ErrRestore(__pyx_t_17, __pyx_t_18, __pyx_t_19);
+          __pyx_t_17 = 0; __pyx_t_18 = 0; __pyx_t_19 = 0; __pyx_t_20 = 0; __pyx_t_21 = 0; __pyx_t_22 = 0;
+          __pyx_lineno = __pyx_t_11; __pyx_clineno = __pyx_t_15; __pyx_filename = __pyx_t_16;
+          goto __pyx_L6_except_error;
+        }
+        __pyx_L14_return: {
+          __pyx_t_5 = __pyx_r;
+          __Pyx_DECREF(__pyx_v_ex);
+          __pyx_v_ex = NULL;
+          __pyx_r = __pyx_t_5;
+          goto __pyx_L7_except_return;
+        }
+      }
     }
     goto __pyx_L6_except_error;
     __pyx_L6_except_error:;
 
     /* "pyrfc/_cyrfc.pyx":1811
  *         if handler is None:
  *             return RCStatus.OK.value
@@ -23369,14 +23875,22 @@
   PyObject *__pyx_t_8 = NULL;
   PyObject *__pyx_t_9 = NULL;
   PyObject *__pyx_t_10 = NULL;
   int __pyx_t_11;
   PyObject *__pyx_t_12 = NULL;
   PyObject *__pyx_t_13 = NULL;
   PyObject *__pyx_t_14 = NULL;
+  int __pyx_t_15;
+  char const *__pyx_t_16;
+  PyObject *__pyx_t_17 = NULL;
+  PyObject *__pyx_t_18 = NULL;
+  PyObject *__pyx_t_19 = NULL;
+  PyObject *__pyx_t_20 = NULL;
+  PyObject *__pyx_t_21 = NULL;
+  PyObject *__pyx_t_22 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
   #endif
   __Pyx_RefNannySetupContext("__onConfirmFunction", 0);
@@ -23386,15 +23900,15 @@
  *     cdef RFC_RC __onConfirmFunction(RFC_CONNECTION_HANDLE rfcHandle, const RFC_UNIT_IDENTIFIER *identifier) with gil:
  *         handler = Server.__bgRfcFunction["confirm"]             # <<<<<<<<<<<<<<
  *         if handler is None:
  *             return RCStatus.OK.value
  */
   __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_5pyrfc_6_cyrfc_Server), __pyx_n_s_bgRfcFunction); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1820, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_Dict_GetItem(__pyx_t_1, __pyx_n_s_confirm); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1820, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Dict_GetItem(__pyx_t_1, __pyx_n_u_confirm); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1820, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_handler = __pyx_t_2;
   __pyx_t_2 = 0;
 
   /* "pyrfc/_cyrfc.pyx":1821
  *     cdef RFC_RC __onConfirmFunction(RFC_CONNECTION_HANDLE rfcHandle, const RFC_UNIT_IDENTIFIER *identifier) with gil:
@@ -23556,93 +24070,148 @@
       __Pyx_AddTraceback("pyrfc._cyrfc.Server.__onConfirmFunction", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_9, &__pyx_t_2, &__pyx_t_12) < 0) __PYX_ERR(0, 1826, __pyx_L6_except_error)
       __Pyx_GOTREF(__pyx_t_9);
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_GOTREF(__pyx_t_12);
       __Pyx_INCREF(__pyx_t_2);
       __pyx_v_ex = __pyx_t_2;
+      /*try:*/ {
 
-      /* "pyrfc/_cyrfc.pyx":1827
+        /* "pyrfc/_cyrfc.pyx":1827
  *             return handler(<uintptr_t>rfcHandle, unit_identifier).value
  *         except Exception as ex:
  *             _server_log("Error in bgRFC handler onConfirm:", ex)             # <<<<<<<<<<<<<<
  *             return RCStatus.RFC_EXTERNAL_FAILURE.value
  * 
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_server_log); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1827, __pyx_L6_except_error)
-      __Pyx_GOTREF(__pyx_t_10);
-      __pyx_t_13 = NULL;
-      __pyx_t_11 = 0;
-      if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_10))) {
-        __pyx_t_13 = PyMethod_GET_SELF(__pyx_t_10);
-        if (likely(__pyx_t_13)) {
-          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_10);
-          __Pyx_INCREF(__pyx_t_13);
-          __Pyx_INCREF(function);
-          __Pyx_DECREF_SET(__pyx_t_10, function);
-          __pyx_t_11 = 1;
+        __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_server_log); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1827, __pyx_L15_error)
+        __Pyx_GOTREF(__pyx_t_10);
+        __pyx_t_13 = NULL;
+        __pyx_t_11 = 0;
+        if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_10))) {
+          __pyx_t_13 = PyMethod_GET_SELF(__pyx_t_10);
+          if (likely(__pyx_t_13)) {
+            PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_10);
+            __Pyx_INCREF(__pyx_t_13);
+            __Pyx_INCREF(function);
+            __Pyx_DECREF_SET(__pyx_t_10, function);
+            __pyx_t_11 = 1;
+          }
         }
-      }
-      #if CYTHON_FAST_PYCALL
-      if (PyFunction_Check(__pyx_t_10)) {
-        PyObject *__pyx_temp[3] = {__pyx_t_13, __pyx_kp_s_Error_in_bgRFC_handler_onConfirm, __pyx_v_ex};
-        __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_10, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1827, __pyx_L6_except_error)
-        __Pyx_XDECREF(__pyx_t_13); __pyx_t_13 = 0;
-        __Pyx_GOTREF(__pyx_t_1);
-      } else
-      #endif
-      #if CYTHON_FAST_PYCCALL
-      if (__Pyx_PyFastCFunction_Check(__pyx_t_10)) {
-        PyObject *__pyx_temp[3] = {__pyx_t_13, __pyx_kp_s_Error_in_bgRFC_handler_onConfirm, __pyx_v_ex};
-        __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_10, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1827, __pyx_L6_except_error)
-        __Pyx_XDECREF(__pyx_t_13); __pyx_t_13 = 0;
-        __Pyx_GOTREF(__pyx_t_1);
-      } else
-      #endif
-      {
-        __pyx_t_14 = PyTuple_New(2+__pyx_t_11); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 1827, __pyx_L6_except_error)
-        __Pyx_GOTREF(__pyx_t_14);
-        if (__pyx_t_13) {
-          __Pyx_GIVEREF(__pyx_t_13); PyTuple_SET_ITEM(__pyx_t_14, 0, __pyx_t_13); __pyx_t_13 = NULL;
-        }
-        __Pyx_INCREF(__pyx_kp_s_Error_in_bgRFC_handler_onConfirm);
-        __Pyx_GIVEREF(__pyx_kp_s_Error_in_bgRFC_handler_onConfirm);
-        PyTuple_SET_ITEM(__pyx_t_14, 0+__pyx_t_11, __pyx_kp_s_Error_in_bgRFC_handler_onConfirm);
-        __Pyx_INCREF(__pyx_v_ex);
-        __Pyx_GIVEREF(__pyx_v_ex);
-        PyTuple_SET_ITEM(__pyx_t_14, 1+__pyx_t_11, __pyx_v_ex);
-        __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_10, __pyx_t_14, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1827, __pyx_L6_except_error)
-        __Pyx_GOTREF(__pyx_t_1);
-        __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
-      }
-      __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+        #if CYTHON_FAST_PYCALL
+        if (PyFunction_Check(__pyx_t_10)) {
+          PyObject *__pyx_temp[3] = {__pyx_t_13, __pyx_kp_u_Error_in_bgRFC_handler_onConfirm, __pyx_v_ex};
+          __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_10, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1827, __pyx_L15_error)
+          __Pyx_XDECREF(__pyx_t_13); __pyx_t_13 = 0;
+          __Pyx_GOTREF(__pyx_t_1);
+        } else
+        #endif
+        #if CYTHON_FAST_PYCCALL
+        if (__Pyx_PyFastCFunction_Check(__pyx_t_10)) {
+          PyObject *__pyx_temp[3] = {__pyx_t_13, __pyx_kp_u_Error_in_bgRFC_handler_onConfirm, __pyx_v_ex};
+          __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_10, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1827, __pyx_L15_error)
+          __Pyx_XDECREF(__pyx_t_13); __pyx_t_13 = 0;
+          __Pyx_GOTREF(__pyx_t_1);
+        } else
+        #endif
+        {
+          __pyx_t_14 = PyTuple_New(2+__pyx_t_11); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 1827, __pyx_L15_error)
+          __Pyx_GOTREF(__pyx_t_14);
+          if (__pyx_t_13) {
+            __Pyx_GIVEREF(__pyx_t_13); PyTuple_SET_ITEM(__pyx_t_14, 0, __pyx_t_13); __pyx_t_13 = NULL;
+          }
+          __Pyx_INCREF(__pyx_kp_u_Error_in_bgRFC_handler_onConfirm);
+          __Pyx_GIVEREF(__pyx_kp_u_Error_in_bgRFC_handler_onConfirm);
+          PyTuple_SET_ITEM(__pyx_t_14, 0+__pyx_t_11, __pyx_kp_u_Error_in_bgRFC_handler_onConfirm);
+          __Pyx_INCREF(__pyx_v_ex);
+          __Pyx_GIVEREF(__pyx_v_ex);
+          PyTuple_SET_ITEM(__pyx_t_14, 1+__pyx_t_11, __pyx_v_ex);
+          __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_10, __pyx_t_14, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1827, __pyx_L15_error)
+          __Pyx_GOTREF(__pyx_t_1);
+          __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
+        }
+        __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+        __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-      /* "pyrfc/_cyrfc.pyx":1828
+        /* "pyrfc/_cyrfc.pyx":1828
  *         except Exception as ex:
  *             _server_log("Error in bgRFC handler onConfirm:", ex)
  *             return RCStatus.RFC_EXTERNAL_FAILURE.value             # <<<<<<<<<<<<<<
  * 
  *     @staticmethod
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_RCStatus); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1828, __pyx_L6_except_error)
-      __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_RFC_EXTERNAL_FAILURE); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1828, __pyx_L6_except_error)
-      __Pyx_GOTREF(__pyx_t_10);
-      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_10, __pyx_n_s_value); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1828, __pyx_L6_except_error)
-      __Pyx_GOTREF(__pyx_t_1);
-      __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-      __pyx_t_5 = ((RFC_RC)__Pyx_PyInt_As_RFC_RC(__pyx_t_1)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1828, __pyx_L6_except_error)
-      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __pyx_r = __pyx_t_5;
-      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-      __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-      __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-      goto __pyx_L7_except_return;
+        __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_RCStatus); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1828, __pyx_L15_error)
+        __Pyx_GOTREF(__pyx_t_1);
+        __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_RFC_EXTERNAL_FAILURE); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1828, __pyx_L15_error)
+        __Pyx_GOTREF(__pyx_t_10);
+        __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+        __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_10, __pyx_n_s_value); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1828, __pyx_L15_error)
+        __Pyx_GOTREF(__pyx_t_1);
+        __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+        __pyx_t_5 = ((RFC_RC)__Pyx_PyInt_As_RFC_RC(__pyx_t_1)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1828, __pyx_L15_error)
+        __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+        __pyx_r = __pyx_t_5;
+        __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+        __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+        __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+        goto __pyx_L14_return;
+      }
+
+      /* "pyrfc/_cyrfc.pyx":1826
+ *             unit_identifier = wrapUnitIdentifier(identifier[0])
+ *             return handler(<uintptr_t>rfcHandle, unit_identifier).value
+ *         except Exception as ex:             # <<<<<<<<<<<<<<
+ *             _server_log("Error in bgRFC handler onConfirm:", ex)
+ *             return RCStatus.RFC_EXTERNAL_FAILURE.value
+ */
+      /*finally:*/ {
+        __pyx_L15_error:;
+        /*exception exit:*/{
+          __Pyx_PyThreadState_declare
+          __Pyx_PyThreadState_assign
+          __pyx_t_17 = 0; __pyx_t_18 = 0; __pyx_t_19 = 0; __pyx_t_20 = 0; __pyx_t_21 = 0; __pyx_t_22 = 0;
+          __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
+          __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
+          __Pyx_XDECREF(__pyx_t_13); __pyx_t_13 = 0;
+          __Pyx_XDECREF(__pyx_t_14); __pyx_t_14 = 0;
+          if (PY_MAJOR_VERSION >= 3) __Pyx_ExceptionSwap(&__pyx_t_20, &__pyx_t_21, &__pyx_t_22);
+          if ((PY_MAJOR_VERSION < 3) || unlikely(__Pyx_GetException(&__pyx_t_17, &__pyx_t_18, &__pyx_t_19) < 0)) __Pyx_ErrFetch(&__pyx_t_17, &__pyx_t_18, &__pyx_t_19);
+          __Pyx_XGOTREF(__pyx_t_17);
+          __Pyx_XGOTREF(__pyx_t_18);
+          __Pyx_XGOTREF(__pyx_t_19);
+          __Pyx_XGOTREF(__pyx_t_20);
+          __Pyx_XGOTREF(__pyx_t_21);
+          __Pyx_XGOTREF(__pyx_t_22);
+          __pyx_t_11 = __pyx_lineno; __pyx_t_15 = __pyx_clineno; __pyx_t_16 = __pyx_filename;
+          {
+            __Pyx_DECREF(__pyx_v_ex);
+            __pyx_v_ex = NULL;
+          }
+          if (PY_MAJOR_VERSION >= 3) {
+            __Pyx_XGIVEREF(__pyx_t_20);
+            __Pyx_XGIVEREF(__pyx_t_21);
+            __Pyx_XGIVEREF(__pyx_t_22);
+            __Pyx_ExceptionReset(__pyx_t_20, __pyx_t_21, __pyx_t_22);
+          }
+          __Pyx_XGIVEREF(__pyx_t_17);
+          __Pyx_XGIVEREF(__pyx_t_18);
+          __Pyx_XGIVEREF(__pyx_t_19);
+          __Pyx_ErrRestore(__pyx_t_17, __pyx_t_18, __pyx_t_19);
+          __pyx_t_17 = 0; __pyx_t_18 = 0; __pyx_t_19 = 0; __pyx_t_20 = 0; __pyx_t_21 = 0; __pyx_t_22 = 0;
+          __pyx_lineno = __pyx_t_11; __pyx_clineno = __pyx_t_15; __pyx_filename = __pyx_t_16;
+          goto __pyx_L6_except_error;
+        }
+        __pyx_L14_return: {
+          __pyx_t_5 = __pyx_r;
+          __Pyx_DECREF(__pyx_v_ex);
+          __pyx_v_ex = NULL;
+          __pyx_r = __pyx_t_5;
+          goto __pyx_L7_except_return;
+        }
+      }
     }
     goto __pyx_L6_except_error;
     __pyx_L6_except_error:;
 
     /* "pyrfc/_cyrfc.pyx":1823
  *         if handler is None:
  *             return RCStatus.OK.value
@@ -23726,14 +24295,22 @@
   PyObject *__pyx_t_10 = NULL;
   int __pyx_t_11;
   PyObject *__pyx_t_12 = NULL;
   Py_ssize_t __pyx_t_13;
   Py_UCS4 __pyx_t_14;
   PyObject *__pyx_t_15 = NULL;
   PyObject *__pyx_t_16 = NULL;
+  int __pyx_t_17;
+  char const *__pyx_t_18;
+  PyObject *__pyx_t_19 = NULL;
+  PyObject *__pyx_t_20 = NULL;
+  PyObject *__pyx_t_21 = NULL;
+  PyObject *__pyx_t_22 = NULL;
+  PyObject *__pyx_t_23 = NULL;
+  PyObject *__pyx_t_24 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
   #endif
   __Pyx_RefNannySetupContext("__onGetStateFunction", 0);
@@ -23743,15 +24320,15 @@
  *             ) with gil:
  *         handler = Server.__bgRfcFunction["getState"]             # <<<<<<<<<<<<<<
  *         if handler is None:
  *             _server_log("bgRFC handler onGetState is not registered for server connection handle '{<uintptr_t>rfcHandle}'")
  */
   __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_5pyrfc_6_cyrfc_Server), __pyx_n_s_bgRfcFunction); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1836, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_Dict_GetItem(__pyx_t_1, __pyx_n_s_getState); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1836, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Dict_GetItem(__pyx_t_1, __pyx_n_u_getState); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1836, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_handler = __pyx_t_2;
   __pyx_t_2 = 0;
 
   /* "pyrfc/_cyrfc.pyx":1837
  *             ) with gil:
@@ -23779,15 +24356,15 @@
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
         __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_1, function);
       }
     }
-    __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_5, __pyx_kp_s_bgRFC_handler_onGetState_is_not) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_kp_s_bgRFC_handler_onGetState_is_not);
+    __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_5, __pyx_kp_u_bgRFC_handler_onGetState_is_not) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_kp_u_bgRFC_handler_onGetState_is_not);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1838, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
     /* "pyrfc/_cyrfc.pyx":1839
@@ -24089,15 +24666,15 @@
         __Pyx_GOTREF(__pyx_t_2);
         __pyx_t_13 = 0;
         __pyx_t_14 = 127;
         __Pyx_INCREF(__pyx_kp_u_TID);
         __pyx_t_13 += 4;
         __Pyx_GIVEREF(__pyx_kp_u_TID);
         PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_kp_u_TID);
-        __pyx_t_5 = __Pyx_PyObject_Dict_GetItem(__pyx_v_unit_identifier, __pyx_n_s_id); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1853, __pyx_L4_error)
+        __pyx_t_5 = __Pyx_PyObject_Dict_GetItem(__pyx_v_unit_identifier, __pyx_n_u_id); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1853, __pyx_L4_error)
         __Pyx_GOTREF(__pyx_t_5);
         __pyx_t_12 = __Pyx_PyObject_FormatSimple(__pyx_t_5, __pyx_empty_unicode); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 1853, __pyx_L4_error)
         __Pyx_GOTREF(__pyx_t_12);
         __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
         __pyx_t_14 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_12) > __pyx_t_14) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_12) : __pyx_t_14;
         __pyx_t_13 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_12);
         __Pyx_GIVEREF(__pyx_t_12);
@@ -24177,93 +24754,148 @@
       __Pyx_AddTraceback("pyrfc._cyrfc.Server.__onGetStateFunction", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_2, &__pyx_t_12, &__pyx_t_5) < 0) __PYX_ERR(0, 1855, __pyx_L6_except_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_GOTREF(__pyx_t_12);
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_INCREF(__pyx_t_12);
       __pyx_v_ex = __pyx_t_12;
+      /*try:*/ {
 
-      /* "pyrfc/_cyrfc.pyx":1856
+        /* "pyrfc/_cyrfc.pyx":1856
  *             return RCStatus.OK.value
  *         except Exception as ex:
  *             _server_log("Error in bgRFC handler onGetState:\n", ex)             # <<<<<<<<<<<<<<
  *             return RCStatus.RFC_EXTERNAL_FAILURE.value
  * 
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_server_log); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1856, __pyx_L6_except_error)
-      __Pyx_GOTREF(__pyx_t_10);
-      __pyx_t_15 = NULL;
-      __pyx_t_11 = 0;
-      if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_10))) {
-        __pyx_t_15 = PyMethod_GET_SELF(__pyx_t_10);
-        if (likely(__pyx_t_15)) {
-          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_10);
-          __Pyx_INCREF(__pyx_t_15);
-          __Pyx_INCREF(function);
-          __Pyx_DECREF_SET(__pyx_t_10, function);
-          __pyx_t_11 = 1;
+        __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_server_log); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1856, __pyx_L18_error)
+        __Pyx_GOTREF(__pyx_t_10);
+        __pyx_t_15 = NULL;
+        __pyx_t_11 = 0;
+        if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_10))) {
+          __pyx_t_15 = PyMethod_GET_SELF(__pyx_t_10);
+          if (likely(__pyx_t_15)) {
+            PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_10);
+            __Pyx_INCREF(__pyx_t_15);
+            __Pyx_INCREF(function);
+            __Pyx_DECREF_SET(__pyx_t_10, function);
+            __pyx_t_11 = 1;
+          }
         }
-      }
-      #if CYTHON_FAST_PYCALL
-      if (PyFunction_Check(__pyx_t_10)) {
-        PyObject *__pyx_temp[3] = {__pyx_t_15, __pyx_kp_s_Error_in_bgRFC_handler_onGetStat, __pyx_v_ex};
-        __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_10, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1856, __pyx_L6_except_error)
-        __Pyx_XDECREF(__pyx_t_15); __pyx_t_15 = 0;
-        __Pyx_GOTREF(__pyx_t_1);
-      } else
-      #endif
-      #if CYTHON_FAST_PYCCALL
-      if (__Pyx_PyFastCFunction_Check(__pyx_t_10)) {
-        PyObject *__pyx_temp[3] = {__pyx_t_15, __pyx_kp_s_Error_in_bgRFC_handler_onGetStat, __pyx_v_ex};
-        __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_10, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1856, __pyx_L6_except_error)
-        __Pyx_XDECREF(__pyx_t_15); __pyx_t_15 = 0;
-        __Pyx_GOTREF(__pyx_t_1);
-      } else
-      #endif
-      {
-        __pyx_t_16 = PyTuple_New(2+__pyx_t_11); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 1856, __pyx_L6_except_error)
-        __Pyx_GOTREF(__pyx_t_16);
-        if (__pyx_t_15) {
-          __Pyx_GIVEREF(__pyx_t_15); PyTuple_SET_ITEM(__pyx_t_16, 0, __pyx_t_15); __pyx_t_15 = NULL;
-        }
-        __Pyx_INCREF(__pyx_kp_s_Error_in_bgRFC_handler_onGetStat);
-        __Pyx_GIVEREF(__pyx_kp_s_Error_in_bgRFC_handler_onGetStat);
-        PyTuple_SET_ITEM(__pyx_t_16, 0+__pyx_t_11, __pyx_kp_s_Error_in_bgRFC_handler_onGetStat);
-        __Pyx_INCREF(__pyx_v_ex);
-        __Pyx_GIVEREF(__pyx_v_ex);
-        PyTuple_SET_ITEM(__pyx_t_16, 1+__pyx_t_11, __pyx_v_ex);
-        __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_10, __pyx_t_16, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1856, __pyx_L6_except_error)
-        __Pyx_GOTREF(__pyx_t_1);
-        __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
-      }
-      __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+        #if CYTHON_FAST_PYCALL
+        if (PyFunction_Check(__pyx_t_10)) {
+          PyObject *__pyx_temp[3] = {__pyx_t_15, __pyx_kp_u_Error_in_bgRFC_handler_onGetStat, __pyx_v_ex};
+          __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_10, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1856, __pyx_L18_error)
+          __Pyx_XDECREF(__pyx_t_15); __pyx_t_15 = 0;
+          __Pyx_GOTREF(__pyx_t_1);
+        } else
+        #endif
+        #if CYTHON_FAST_PYCCALL
+        if (__Pyx_PyFastCFunction_Check(__pyx_t_10)) {
+          PyObject *__pyx_temp[3] = {__pyx_t_15, __pyx_kp_u_Error_in_bgRFC_handler_onGetStat, __pyx_v_ex};
+          __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_10, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1856, __pyx_L18_error)
+          __Pyx_XDECREF(__pyx_t_15); __pyx_t_15 = 0;
+          __Pyx_GOTREF(__pyx_t_1);
+        } else
+        #endif
+        {
+          __pyx_t_16 = PyTuple_New(2+__pyx_t_11); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 1856, __pyx_L18_error)
+          __Pyx_GOTREF(__pyx_t_16);
+          if (__pyx_t_15) {
+            __Pyx_GIVEREF(__pyx_t_15); PyTuple_SET_ITEM(__pyx_t_16, 0, __pyx_t_15); __pyx_t_15 = NULL;
+          }
+          __Pyx_INCREF(__pyx_kp_u_Error_in_bgRFC_handler_onGetStat);
+          __Pyx_GIVEREF(__pyx_kp_u_Error_in_bgRFC_handler_onGetStat);
+          PyTuple_SET_ITEM(__pyx_t_16, 0+__pyx_t_11, __pyx_kp_u_Error_in_bgRFC_handler_onGetStat);
+          __Pyx_INCREF(__pyx_v_ex);
+          __Pyx_GIVEREF(__pyx_v_ex);
+          PyTuple_SET_ITEM(__pyx_t_16, 1+__pyx_t_11, __pyx_v_ex);
+          __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_10, __pyx_t_16, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1856, __pyx_L18_error)
+          __Pyx_GOTREF(__pyx_t_1);
+          __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
+        }
+        __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+        __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-      /* "pyrfc/_cyrfc.pyx":1857
+        /* "pyrfc/_cyrfc.pyx":1857
  *         except Exception as ex:
  *             _server_log("Error in bgRFC handler onGetState:\n", ex)
  *             return RCStatus.RFC_EXTERNAL_FAILURE.value             # <<<<<<<<<<<<<<
  * 
  *     def bgrfc_init(self, sysId, bgRfcFunction):
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_RCStatus); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1857, __pyx_L6_except_error)
-      __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_RFC_EXTERNAL_FAILURE); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1857, __pyx_L6_except_error)
-      __Pyx_GOTREF(__pyx_t_10);
-      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_10, __pyx_n_s_value); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1857, __pyx_L6_except_error)
-      __Pyx_GOTREF(__pyx_t_1);
-      __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-      __pyx_t_6 = ((RFC_RC)__Pyx_PyInt_As_RFC_RC(__pyx_t_1)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1857, __pyx_L6_except_error)
-      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __pyx_r = __pyx_t_6;
-      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-      goto __pyx_L7_except_return;
+        __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_RCStatus); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1857, __pyx_L18_error)
+        __Pyx_GOTREF(__pyx_t_1);
+        __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_RFC_EXTERNAL_FAILURE); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1857, __pyx_L18_error)
+        __Pyx_GOTREF(__pyx_t_10);
+        __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+        __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_10, __pyx_n_s_value); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1857, __pyx_L18_error)
+        __Pyx_GOTREF(__pyx_t_1);
+        __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+        __pyx_t_6 = ((RFC_RC)__Pyx_PyInt_As_RFC_RC(__pyx_t_1)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1857, __pyx_L18_error)
+        __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+        __pyx_r = __pyx_t_6;
+        __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+        __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+        __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+        goto __pyx_L17_return;
+      }
+
+      /* "pyrfc/_cyrfc.pyx":1855
+ *                 raise Exception(f"TID {unit_identifier['id']} invalid state '{state}'")
+ *             return RCStatus.OK.value
+ *         except Exception as ex:             # <<<<<<<<<<<<<<
+ *             _server_log("Error in bgRFC handler onGetState:\n", ex)
+ *             return RCStatus.RFC_EXTERNAL_FAILURE.value
+ */
+      /*finally:*/ {
+        __pyx_L18_error:;
+        /*exception exit:*/{
+          __Pyx_PyThreadState_declare
+          __Pyx_PyThreadState_assign
+          __pyx_t_19 = 0; __pyx_t_20 = 0; __pyx_t_21 = 0; __pyx_t_22 = 0; __pyx_t_23 = 0; __pyx_t_24 = 0;
+          __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
+          __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
+          __Pyx_XDECREF(__pyx_t_15); __pyx_t_15 = 0;
+          __Pyx_XDECREF(__pyx_t_16); __pyx_t_16 = 0;
+          if (PY_MAJOR_VERSION >= 3) __Pyx_ExceptionSwap(&__pyx_t_22, &__pyx_t_23, &__pyx_t_24);
+          if ((PY_MAJOR_VERSION < 3) || unlikely(__Pyx_GetException(&__pyx_t_19, &__pyx_t_20, &__pyx_t_21) < 0)) __Pyx_ErrFetch(&__pyx_t_19, &__pyx_t_20, &__pyx_t_21);
+          __Pyx_XGOTREF(__pyx_t_19);
+          __Pyx_XGOTREF(__pyx_t_20);
+          __Pyx_XGOTREF(__pyx_t_21);
+          __Pyx_XGOTREF(__pyx_t_22);
+          __Pyx_XGOTREF(__pyx_t_23);
+          __Pyx_XGOTREF(__pyx_t_24);
+          __pyx_t_11 = __pyx_lineno; __pyx_t_17 = __pyx_clineno; __pyx_t_18 = __pyx_filename;
+          {
+            __Pyx_DECREF(__pyx_v_ex);
+            __pyx_v_ex = NULL;
+          }
+          if (PY_MAJOR_VERSION >= 3) {
+            __Pyx_XGIVEREF(__pyx_t_22);
+            __Pyx_XGIVEREF(__pyx_t_23);
+            __Pyx_XGIVEREF(__pyx_t_24);
+            __Pyx_ExceptionReset(__pyx_t_22, __pyx_t_23, __pyx_t_24);
+          }
+          __Pyx_XGIVEREF(__pyx_t_19);
+          __Pyx_XGIVEREF(__pyx_t_20);
+          __Pyx_XGIVEREF(__pyx_t_21);
+          __Pyx_ErrRestore(__pyx_t_19, __pyx_t_20, __pyx_t_21);
+          __pyx_t_19 = 0; __pyx_t_20 = 0; __pyx_t_21 = 0; __pyx_t_22 = 0; __pyx_t_23 = 0; __pyx_t_24 = 0;
+          __pyx_lineno = __pyx_t_11; __pyx_clineno = __pyx_t_17; __pyx_filename = __pyx_t_18;
+          goto __pyx_L6_except_error;
+        }
+        __pyx_L17_return: {
+          __pyx_t_6 = __pyx_r;
+          __Pyx_DECREF(__pyx_v_ex);
+          __pyx_v_ex = NULL;
+          __pyx_r = __pyx_t_6;
+          goto __pyx_L7_except_return;
+        }
+      }
     }
     goto __pyx_L6_except_error;
     __pyx_L6_except_error:;
 
     /* "pyrfc/_cyrfc.pyx":1840
  *             _server_log("bgRFC handler onGetState is not registered for server connection handle '{<uintptr_t>rfcHandle}'")
  *             return RCStatus.RFC_EXTERNAL_FAILURE.value
@@ -25099,34 +25731,34 @@
  *             "callback": callback,
  *             "server": self
  */
   __pyx_t_1 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1939, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_6 = __Pyx_PyInt_FromSize_t(((uintptr_t)__pyx_v_func_desc_handle)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1939, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_func_desc_handle, __pyx_t_6) < 0) __PYX_ERR(0, 1939, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_func_desc_handle, __pyx_t_6) < 0) __PYX_ERR(0, 1939, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
   /* "pyrfc/_cyrfc.pyx":1940
  *         server_functions[func_name] = {
  *             "func_desc_handle": <uintptr_t>func_desc_handle,
  *             "callback": callback,             # <<<<<<<<<<<<<<
  *             "server": self
  *         }
  */
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_callback, __pyx_v_callback) < 0) __PYX_ERR(0, 1939, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_callback, __pyx_v_callback) < 0) __PYX_ERR(0, 1939, __pyx_L1_error)
 
   /* "pyrfc/_cyrfc.pyx":1941
  *             "func_desc_handle": <uintptr_t>func_desc_handle,
  *             "callback": callback,
  *             "server": self             # <<<<<<<<<<<<<<
  *         }
  * 
  */
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_server, ((PyObject *)__pyx_v_self)) < 0) __PYX_ERR(0, 1939, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_server, ((PyObject *)__pyx_v_self)) < 0) __PYX_ERR(0, 1939, __pyx_L1_error)
 
   /* "pyrfc/_cyrfc.pyx":1938
  *             raise wrapError(&errorInfo)
  * 
  *         server_functions[func_name] = {             # <<<<<<<<<<<<<<
  *             "func_desc_handle": <uintptr_t>func_desc_handle,
  *             "callback": callback,
@@ -25156,37 +25788,37 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_6, function);
       __pyx_t_9 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_6)) {
-    PyObject *__pyx_temp[3] = {__pyx_t_7, __pyx_kp_s_Server_function_installed, __pyx_v_func_name};
+    PyObject *__pyx_temp[3] = {__pyx_t_7, __pyx_kp_u_Server_function_installed, __pyx_v_func_name};
     __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1944, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_GOTREF(__pyx_t_1);
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_6)) {
-    PyObject *__pyx_temp[3] = {__pyx_t_7, __pyx_kp_s_Server_function_installed, __pyx_v_func_name};
+    PyObject *__pyx_temp[3] = {__pyx_t_7, __pyx_kp_u_Server_function_installed, __pyx_v_func_name};
     __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1944, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_GOTREF(__pyx_t_1);
   } else
   #endif
   {
     __pyx_t_10 = PyTuple_New(2+__pyx_t_9); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1944, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
     if (__pyx_t_7) {
       __Pyx_GIVEREF(__pyx_t_7); PyTuple_SET_ITEM(__pyx_t_10, 0, __pyx_t_7); __pyx_t_7 = NULL;
     }
-    __Pyx_INCREF(__pyx_kp_s_Server_function_installed);
-    __Pyx_GIVEREF(__pyx_kp_s_Server_function_installed);
-    PyTuple_SET_ITEM(__pyx_t_10, 0+__pyx_t_9, __pyx_kp_s_Server_function_installed);
+    __Pyx_INCREF(__pyx_kp_u_Server_function_installed);
+    __Pyx_GIVEREF(__pyx_kp_u_Server_function_installed);
+    PyTuple_SET_ITEM(__pyx_t_10, 0+__pyx_t_9, __pyx_kp_u_Server_function_installed);
     __Pyx_INCREF(__pyx_v_func_name);
     __Pyx_GIVEREF(__pyx_v_func_name);
     PyTuple_SET_ITEM(__pyx_t_10, 1+__pyx_t_9, __pyx_v_func_name);
     __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_10, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1944, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
   }
@@ -25217,39 +25849,39 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_6, function);
       __pyx_t_9 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_6)) {
-    PyObject *__pyx_temp[3] = {__pyx_t_10, __pyx_kp_s_Server_function_installed, __pyx_t_7};
+    PyObject *__pyx_temp[3] = {__pyx_t_10, __pyx_kp_u_Server_function_installed, __pyx_t_7};
     __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1945, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_6)) {
-    PyObject *__pyx_temp[3] = {__pyx_t_10, __pyx_kp_s_Server_function_installed, __pyx_t_7};
+    PyObject *__pyx_temp[3] = {__pyx_t_10, __pyx_kp_u_Server_function_installed, __pyx_t_7};
     __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1945, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   } else
   #endif
   {
     __pyx_t_11 = PyTuple_New(2+__pyx_t_9); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 1945, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_11);
     if (__pyx_t_10) {
       __Pyx_GIVEREF(__pyx_t_10); PyTuple_SET_ITEM(__pyx_t_11, 0, __pyx_t_10); __pyx_t_10 = NULL;
     }
-    __Pyx_INCREF(__pyx_kp_s_Server_function_installed);
-    __Pyx_GIVEREF(__pyx_kp_s_Server_function_installed);
-    PyTuple_SET_ITEM(__pyx_t_11, 0+__pyx_t_9, __pyx_kp_s_Server_function_installed);
+    __Pyx_INCREF(__pyx_kp_u_Server_function_installed);
+    __Pyx_GIVEREF(__pyx_kp_u_Server_function_installed);
+    PyTuple_SET_ITEM(__pyx_t_11, 0+__pyx_t_9, __pyx_kp_u_Server_function_installed);
     __Pyx_GIVEREF(__pyx_t_7);
     PyTuple_SET_ITEM(__pyx_t_11, 1+__pyx_t_9, __pyx_t_7);
     __pyx_t_7 = 0;
     __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_11, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1945, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
   }
@@ -25446,39 +26078,39 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_4, function);
       __pyx_t_7 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_4)) {
-    PyObject *__pyx_temp[3] = {__pyx_t_6, __pyx_n_s_Server, __pyx_t_5};
+    PyObject *__pyx_temp[3] = {__pyx_t_6, __pyx_n_u_Server, __pyx_t_5};
     __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1963, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_4)) {
-    PyObject *__pyx_temp[3] = {__pyx_t_6, __pyx_n_s_Server, __pyx_t_5};
+    PyObject *__pyx_temp[3] = {__pyx_t_6, __pyx_n_u_Server, __pyx_t_5};
     __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1963, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   } else
   #endif
   {
     __pyx_t_8 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1963, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     if (__pyx_t_6) {
       __Pyx_GIVEREF(__pyx_t_6); PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_6); __pyx_t_6 = NULL;
     }
-    __Pyx_INCREF(__pyx_n_s_Server);
-    __Pyx_GIVEREF(__pyx_n_s_Server);
-    PyTuple_SET_ITEM(__pyx_t_8, 0+__pyx_t_7, __pyx_n_s_Server);
+    __Pyx_INCREF(__pyx_n_u_Server);
+    __Pyx_GIVEREF(__pyx_n_u_Server);
+    PyTuple_SET_ITEM(__pyx_t_8, 0+__pyx_t_7, __pyx_n_u_Server);
     __Pyx_GIVEREF(__pyx_t_5);
     PyTuple_SET_ITEM(__pyx_t_8, 1+__pyx_t_7, __pyx_t_5);
     __pyx_t_5 = 0;
     __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_8, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1963, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   }
@@ -25957,27 +26589,27 @@
   __pyx_t_3 = __Pyx_PyDict_NewPresized(6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2015, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4.__pyx_n = 2;
   __pyx_t_4.uclen = __pyx_int_neg_1;
   __pyx_t_4.rstrip = Py_True;
   __pyx_t_5 = __pyx_f_5pyrfc_6_cyrfc_wrapString(__pyx_v_attributes.serverName, &__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 2015, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_serverName, __pyx_t_5) < 0) __PYX_ERR(0, 2015, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_serverName, __pyx_t_5) < 0) __PYX_ERR(0, 2015, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "pyrfc/_cyrfc.pyx":2017
  *             'serverName': wrapString(attributes.serverName, -1, True)
  *             # This RFC server's type. Will be one of RFC_MULTI_COUNT_REGISTERED_SERVER or RFC_TCP_SOCKET_SERVER
  *             , 'protocolType': "multi count" if attributes.type == RFC_MULTI_COUNT_REGISTERED_SERVER             # <<<<<<<<<<<<<<
  *             else socket.gethostname()  # Own host name
  *             # The current number of active registrations (in case of a Registered Server)
  */
   if (((__pyx_v_attributes.type == RFC_MULTI_COUNT_REGISTERED_SERVER) != 0)) {
-    __Pyx_INCREF(__pyx_kp_s_multi_count);
-    __pyx_t_5 = __pyx_kp_s_multi_count;
+    __Pyx_INCREF(__pyx_kp_u_multi_count);
+    __pyx_t_5 = __pyx_kp_u_multi_count;
   } else {
 
     /* "pyrfc/_cyrfc.pyx":2018
  *             # This RFC server's type. Will be one of RFC_MULTI_COUNT_REGISTERED_SERVER or RFC_TCP_SOCKET_SERVER
  *             , 'protocolType': "multi count" if attributes.type == RFC_MULTI_COUNT_REGISTERED_SERVER
  *             else socket.gethostname()  # Own host name             # <<<<<<<<<<<<<<
  *             # The current number of active registrations (in case of a Registered Server)
@@ -26002,60 +26634,60 @@
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 2018, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     __pyx_t_5 = __pyx_t_6;
     __pyx_t_6 = 0;
   }
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_protocolType, __pyx_t_5) < 0) __PYX_ERR(0, 2015, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_protocolType, __pyx_t_5) < 0) __PYX_ERR(0, 2015, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "pyrfc/_cyrfc.pyx":2021
  *             # The current number of active registrations (in case of a Registered Server)
  *             # or the maximum number of parallel connections the server will accept (in case of a TCP Socket Server)
  *             , 'registrationCount': attributes.registrationCount             # <<<<<<<<<<<<<<
  *             # Used in state information in order to indicate the current state of an RFC Server.
  *             , 'state': rfcServerState
  */
   __pyx_t_5 = __Pyx_PyInt_From_unsigned_int(__pyx_v_attributes.registrationCount); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 2021, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_registrationCount, __pyx_t_5) < 0) __PYX_ERR(0, 2015, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_registrationCount, __pyx_t_5) < 0) __PYX_ERR(0, 2015, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "pyrfc/_cyrfc.pyx":2023
  *             , 'registrationCount': attributes.registrationCount
  *             # Used in state information in order to indicate the current state of an RFC Server.
  *             , 'state': rfcServerState             # <<<<<<<<<<<<<<
  *             # The number of requests currently being processed.
  *             , 'currentBusyCount': attributes.currentBusyCount
  */
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_state, __pyx_v_rfcServerState) < 0) __PYX_ERR(0, 2015, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_state, __pyx_v_rfcServerState) < 0) __PYX_ERR(0, 2015, __pyx_L1_error)
 
   /* "pyrfc/_cyrfc.pyx":2025
  *             , 'state': rfcServerState
  *             # The number of requests currently being processed.
  *             , 'currentBusyCount': attributes.currentBusyCount             # <<<<<<<<<<<<<<
  *             # The maximum number of requests the server has been processing in parallel since it has been created
  *             , 'peakBusyCount': attributes.peakBusyCount
  */
   __pyx_t_5 = __Pyx_PyInt_From_unsigned_int(__pyx_v_attributes.currentBusyCount); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 2025, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_currentBusyCount, __pyx_t_5) < 0) __PYX_ERR(0, 2015, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_currentBusyCount, __pyx_t_5) < 0) __PYX_ERR(0, 2015, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "pyrfc/_cyrfc.pyx":2027
  *             , 'currentBusyCount': attributes.currentBusyCount
  *             # The maximum number of requests the server has been processing in parallel since it has been created
  *             , 'peakBusyCount': attributes.peakBusyCount             # <<<<<<<<<<<<<<
  *         }
  * 
  */
   __pyx_t_5 = __Pyx_PyInt_From_unsigned_int(__pyx_v_attributes.peakBusyCount); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 2027, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_peakBusyCount, __pyx_t_5) < 0) __PYX_ERR(0, 2015, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_peakBusyCount, __pyx_t_5) < 0) __PYX_ERR(0, 2015, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_r = __pyx_t_3;
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
   /* "pyrfc/_cyrfc.pyx":1990
  *         self._close()
@@ -26110,18 +26742,17 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   Py_ssize_t __pyx_t_5;
-  PyObject *(*__pyx_t_6)(PyObject *);
-  PyObject *__pyx_t_7 = NULL;
-  PyObject *__pyx_t_8 = NULL;
-  PyObject *(*__pyx_t_9)(PyObject *);
+  Py_ssize_t __pyx_t_6;
+  int __pyx_t_7;
+  int __pyx_t_8;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_close", 0);
 
   /* "pyrfc/_cyrfc.pyx":2036
  *         """
@@ -26183,138 +26814,51 @@
   /* "pyrfc/_cyrfc.pyx":2041
  *         after_remove = {}
  *         global server_functions
  *         for func_name, func_data in server_functions.items():             # <<<<<<<<<<<<<<
  *             if func_data["server"] != self:
  *                 after_remove[func_name] = func_data
  */
+  __pyx_t_5 = 0;
   __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_server_functions); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2041, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_items); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 2041, __pyx_L1_error)
+  if (unlikely(__pyx_t_3 == Py_None)) {
+    PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "items");
+    __PYX_ERR(0, 2041, __pyx_L1_error)
+  }
+  __pyx_t_4 = __Pyx_dict_iterator(__pyx_t_3, 0, __pyx_n_s_items, (&__pyx_t_6), (&__pyx_t_7)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 2041, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = NULL;
-  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
-    __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_4);
-    if (likely(__pyx_t_3)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
-      __Pyx_INCREF(__pyx_t_3);
-      __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_4, function);
-    }
-  }
-  __pyx_t_2 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_4);
-  __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2041, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (likely(PyList_CheckExact(__pyx_t_2)) || PyTuple_CheckExact(__pyx_t_2)) {
-    __pyx_t_4 = __pyx_t_2; __Pyx_INCREF(__pyx_t_4); __pyx_t_5 = 0;
-    __pyx_t_6 = NULL;
-  } else {
-    __pyx_t_5 = -1; __pyx_t_4 = PyObject_GetIter(__pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 2041, __pyx_L1_error)
+  __Pyx_XDECREF(__pyx_t_2);
+  __pyx_t_2 = __pyx_t_4;
+  __pyx_t_4 = 0;
+  while (1) {
+    __pyx_t_8 = __Pyx_dict_iter_next(__pyx_t_2, __pyx_t_6, &__pyx_t_5, &__pyx_t_4, &__pyx_t_3, NULL, __pyx_t_7);
+    if (unlikely(__pyx_t_8 == 0)) break;
+    if (unlikely(__pyx_t_8 == -1)) __PYX_ERR(0, 2041, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_6 = Py_TYPE(__pyx_t_4)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 2041, __pyx_L1_error)
-  }
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  for (;;) {
-    if (likely(!__pyx_t_6)) {
-      if (likely(PyList_CheckExact(__pyx_t_4))) {
-        if (__pyx_t_5 >= PyList_GET_SIZE(__pyx_t_4)) break;
-        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_2 = PyList_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_2); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(0, 2041, __pyx_L1_error)
-        #else
-        __pyx_t_2 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2041, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_2);
-        #endif
-      } else {
-        if (__pyx_t_5 >= PyTuple_GET_SIZE(__pyx_t_4)) break;
-        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_2); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(0, 2041, __pyx_L1_error)
-        #else
-        __pyx_t_2 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2041, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_2);
-        #endif
-      }
-    } else {
-      __pyx_t_2 = __pyx_t_6(__pyx_t_4);
-      if (unlikely(!__pyx_t_2)) {
-        PyObject* exc_type = PyErr_Occurred();
-        if (exc_type) {
-          if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 2041, __pyx_L1_error)
-        }
-        break;
-      }
-      __Pyx_GOTREF(__pyx_t_2);
-    }
-    if ((likely(PyTuple_CheckExact(__pyx_t_2))) || (PyList_CheckExact(__pyx_t_2))) {
-      PyObject* sequence = __pyx_t_2;
-      Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
-      if (unlikely(size != 2)) {
-        if (size > 2) __Pyx_RaiseTooManyValuesError(2);
-        else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-        __PYX_ERR(0, 2041, __pyx_L1_error)
-      }
-      #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-      if (likely(PyTuple_CheckExact(sequence))) {
-        __pyx_t_3 = PyTuple_GET_ITEM(sequence, 0); 
-        __pyx_t_7 = PyTuple_GET_ITEM(sequence, 1); 
-      } else {
-        __pyx_t_3 = PyList_GET_ITEM(sequence, 0); 
-        __pyx_t_7 = PyList_GET_ITEM(sequence, 1); 
-      }
-      __Pyx_INCREF(__pyx_t_3);
-      __Pyx_INCREF(__pyx_t_7);
-      #else
-      __pyx_t_3 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2041, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_7 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 2041, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_7);
-      #endif
-      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    } else {
-      Py_ssize_t index = -1;
-      __pyx_t_8 = PyObject_GetIter(__pyx_t_2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 2041, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_8);
-      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-      __pyx_t_9 = Py_TYPE(__pyx_t_8)->tp_iternext;
-      index = 0; __pyx_t_3 = __pyx_t_9(__pyx_t_8); if (unlikely(!__pyx_t_3)) goto __pyx_L6_unpacking_failed;
-      __Pyx_GOTREF(__pyx_t_3);
-      index = 1; __pyx_t_7 = __pyx_t_9(__pyx_t_8); if (unlikely(!__pyx_t_7)) goto __pyx_L6_unpacking_failed;
-      __Pyx_GOTREF(__pyx_t_7);
-      if (__Pyx_IternextUnpackEndCheck(__pyx_t_9(__pyx_t_8), 2) < 0) __PYX_ERR(0, 2041, __pyx_L1_error)
-      __pyx_t_9 = NULL;
-      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      goto __pyx_L7_unpacking_done;
-      __pyx_L6_unpacking_failed:;
-      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __pyx_t_9 = NULL;
-      if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-      __PYX_ERR(0, 2041, __pyx_L1_error)
-      __pyx_L7_unpacking_done:;
-    }
-    __Pyx_XDECREF_SET(__pyx_v_func_name, __pyx_t_3);
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_XDECREF_SET(__pyx_v_func_name, __pyx_t_4);
+    __pyx_t_4 = 0;
+    __Pyx_XDECREF_SET(__pyx_v_func_data, __pyx_t_3);
     __pyx_t_3 = 0;
-    __Pyx_XDECREF_SET(__pyx_v_func_data, __pyx_t_7);
-    __pyx_t_7 = 0;
 
     /* "pyrfc/_cyrfc.pyx":2042
  *         global server_functions
  *         for func_name, func_data in server_functions.items():
  *             if func_data["server"] != self:             # <<<<<<<<<<<<<<
  *                 after_remove[func_name] = func_data
  *         server_functions = after_remove
  */
-    __pyx_t_2 = __Pyx_PyObject_Dict_GetItem(__pyx_v_func_data, __pyx_n_s_server); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2042, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_7 = PyObject_RichCompare(__pyx_t_2, ((PyObject *)__pyx_v_self), Py_NE); __Pyx_XGOTREF(__pyx_t_7); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 2042, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_7); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 2042, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+    __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_v_func_data, __pyx_n_u_server); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2042, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __pyx_t_4 = PyObject_RichCompare(__pyx_t_3, ((PyObject *)__pyx_v_self), Py_NE); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 2042, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 2042, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     if (__pyx_t_1) {
 
       /* "pyrfc/_cyrfc.pyx":2043
  *         for func_name, func_data in server_functions.items():
  *             if func_data["server"] != self:
  *                 after_remove[func_name] = func_data             # <<<<<<<<<<<<<<
  *         server_functions = after_remove
@@ -26326,24 +26870,16 @@
  *         global server_functions
  *         for func_name, func_data in server_functions.items():
  *             if func_data["server"] != self:             # <<<<<<<<<<<<<<
  *                 after_remove[func_name] = func_data
  *         server_functions = after_remove
  */
     }
-
-    /* "pyrfc/_cyrfc.pyx":2041
- *         after_remove = {}
- *         global server_functions
- *         for func_name, func_data in server_functions.items():             # <<<<<<<<<<<<<<
- *             if func_data["server"] != self:
- *                 after_remove[func_name] = func_data
- */
   }
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "pyrfc/_cyrfc.pyx":2044
  *             if func_data["server"] != self:
  *                 after_remove[func_name] = func_data
  *         server_functions = after_remove             # <<<<<<<<<<<<<<
  * 
  *     cdef _error(self, RFC_ERROR_INFO* errorInfo):
@@ -26361,16 +26897,14 @@
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_XDECREF(__pyx_t_7);
-  __Pyx_XDECREF(__pyx_t_8);
   __Pyx_AddTraceback("pyrfc._cyrfc.Server._close", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_after_remove);
   __Pyx_XDECREF(__pyx_v_func_name);
   __Pyx_XDECREF(__pyx_v_func_data);
   __Pyx_XGIVEREF(__pyx_r);
@@ -26620,15 +27154,15 @@
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__33, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 2, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__34, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(1, 2, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
@@ -26676,15 +27210,15 @@
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__34, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__35, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(1, 4, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
@@ -26923,28 +27457,28 @@
     /* "pyrfc/_cyrfc.pyx":2088
  *     for field_desc in type_desc.fields:
  *         # Set name
  *         sapuc = fillString(field_desc['name'])             # <<<<<<<<<<<<<<
  *         strncpyU(fieldDesc.name, sapuc, len(field_desc['name']) + 1)
  *         free(sapuc)
  */
-    __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_field_desc, __pyx_n_s_name); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2088, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_field_desc, __pyx_n_u_name); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2088, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_2 = __pyx_f_5pyrfc_6_cyrfc_fillString(__pyx_t_1); if (unlikely(__pyx_t_2 == ((SAP_UC *)NULL))) __PYX_ERR(0, 2088, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_v_sapuc = __pyx_t_2;
 
     /* "pyrfc/_cyrfc.pyx":2089
  *         # Set name
  *         sapuc = fillString(field_desc['name'])
  *         strncpyU(fieldDesc.name, sapuc, len(field_desc['name']) + 1)             # <<<<<<<<<<<<<<
  *         free(sapuc)
  *         fieldDesc.type = RfcFieldType[field_desc['field_type']].value
  */
-    __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_field_desc, __pyx_n_s_name); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2089, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_field_desc, __pyx_n_u_name); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2089, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_9 = PyObject_Length(__pyx_t_1); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1))) __PYX_ERR(0, 2089, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     strncpyU(__pyx_v_fieldDesc.name, __pyx_v_sapuc, (__pyx_t_9 + 1));
 
     /* "pyrfc/_cyrfc.pyx":2090
  *         sapuc = fillString(field_desc['name'])
@@ -26960,15 +27494,15 @@
  *         free(sapuc)
  *         fieldDesc.type = RfcFieldType[field_desc['field_type']].value             # <<<<<<<<<<<<<<
  *         fieldDesc.nucLength = field_desc['nuc_length']
  *         fieldDesc.nucOffset = field_desc['nuc_offset']
  */
     __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_RfcFieldType); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2091, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_10 = __Pyx_PyObject_Dict_GetItem(__pyx_v_field_desc, __pyx_n_s_field_type); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 2091, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyObject_Dict_GetItem(__pyx_v_field_desc, __pyx_n_u_field_type); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 2091, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
     __pyx_t_11 = __Pyx_PyObject_GetItem(__pyx_t_1, __pyx_t_10); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 2091, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_11);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
     __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_11, __pyx_n_s_value); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 2091, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
@@ -26980,94 +27514,94 @@
     /* "pyrfc/_cyrfc.pyx":2092
  *         free(sapuc)
  *         fieldDesc.type = RfcFieldType[field_desc['field_type']].value
  *         fieldDesc.nucLength = field_desc['nuc_length']             # <<<<<<<<<<<<<<
  *         fieldDesc.nucOffset = field_desc['nuc_offset']
  *         fieldDesc.ucLength = field_desc['uc_length']
  */
-    __pyx_t_10 = __Pyx_PyObject_Dict_GetItem(__pyx_v_field_desc, __pyx_n_s_nuc_length); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 2092, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyObject_Dict_GetItem(__pyx_v_field_desc, __pyx_n_u_nuc_length); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 2092, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
     __pyx_t_5 = __Pyx_PyInt_As_unsigned_int(__pyx_t_10); if (unlikely((__pyx_t_5 == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(0, 2092, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
     __pyx_v_fieldDesc.nucLength = __pyx_t_5;
 
     /* "pyrfc/_cyrfc.pyx":2093
  *         fieldDesc.type = RfcFieldType[field_desc['field_type']].value
  *         fieldDesc.nucLength = field_desc['nuc_length']
  *         fieldDesc.nucOffset = field_desc['nuc_offset']             # <<<<<<<<<<<<<<
  *         fieldDesc.ucLength = field_desc['uc_length']
  *         fieldDesc.ucOffset = field_desc['uc_offset']
  */
-    __pyx_t_10 = __Pyx_PyObject_Dict_GetItem(__pyx_v_field_desc, __pyx_n_s_nuc_offset); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 2093, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyObject_Dict_GetItem(__pyx_v_field_desc, __pyx_n_u_nuc_offset); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 2093, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
     __pyx_t_5 = __Pyx_PyInt_As_unsigned_int(__pyx_t_10); if (unlikely((__pyx_t_5 == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(0, 2093, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
     __pyx_v_fieldDesc.nucOffset = __pyx_t_5;
 
     /* "pyrfc/_cyrfc.pyx":2094
  *         fieldDesc.nucLength = field_desc['nuc_length']
  *         fieldDesc.nucOffset = field_desc['nuc_offset']
  *         fieldDesc.ucLength = field_desc['uc_length']             # <<<<<<<<<<<<<<
  *         fieldDesc.ucOffset = field_desc['uc_offset']
  *         fieldDesc.decimals = field_desc['decimals']
  */
-    __pyx_t_10 = __Pyx_PyObject_Dict_GetItem(__pyx_v_field_desc, __pyx_n_s_uc_length); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 2094, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyObject_Dict_GetItem(__pyx_v_field_desc, __pyx_n_u_uc_length); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 2094, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
     __pyx_t_5 = __Pyx_PyInt_As_unsigned_int(__pyx_t_10); if (unlikely((__pyx_t_5 == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(0, 2094, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
     __pyx_v_fieldDesc.ucLength = __pyx_t_5;
 
     /* "pyrfc/_cyrfc.pyx":2095
  *         fieldDesc.nucOffset = field_desc['nuc_offset']
  *         fieldDesc.ucLength = field_desc['uc_length']
  *         fieldDesc.ucOffset = field_desc['uc_offset']             # <<<<<<<<<<<<<<
  *         fieldDesc.decimals = field_desc['decimals']
  *         if field_desc['type_description'] is not None:
  */
-    __pyx_t_10 = __Pyx_PyObject_Dict_GetItem(__pyx_v_field_desc, __pyx_n_s_uc_offset); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 2095, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyObject_Dict_GetItem(__pyx_v_field_desc, __pyx_n_u_uc_offset); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 2095, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
     __pyx_t_5 = __Pyx_PyInt_As_unsigned_int(__pyx_t_10); if (unlikely((__pyx_t_5 == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(0, 2095, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
     __pyx_v_fieldDesc.ucOffset = __pyx_t_5;
 
     /* "pyrfc/_cyrfc.pyx":2096
  *         fieldDesc.ucLength = field_desc['uc_length']
  *         fieldDesc.ucOffset = field_desc['uc_offset']
  *         fieldDesc.decimals = field_desc['decimals']             # <<<<<<<<<<<<<<
  *         if field_desc['type_description'] is not None:
  *             fieldDesc.typeDescHandle = fillTypeDescription(field_desc['type_description'])
  */
-    __pyx_t_10 = __Pyx_PyObject_Dict_GetItem(__pyx_v_field_desc, __pyx_n_s_decimals); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 2096, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyObject_Dict_GetItem(__pyx_v_field_desc, __pyx_n_u_decimals); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 2096, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
     __pyx_t_5 = __Pyx_PyInt_As_unsigned_int(__pyx_t_10); if (unlikely((__pyx_t_5 == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(0, 2096, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
     __pyx_v_fieldDesc.decimals = __pyx_t_5;
 
     /* "pyrfc/_cyrfc.pyx":2097
  *         fieldDesc.ucOffset = field_desc['uc_offset']
  *         fieldDesc.decimals = field_desc['decimals']
  *         if field_desc['type_description'] is not None:             # <<<<<<<<<<<<<<
  *             fieldDesc.typeDescHandle = fillTypeDescription(field_desc['type_description'])
  *         else:
  */
-    __pyx_t_10 = __Pyx_PyObject_Dict_GetItem(__pyx_v_field_desc, __pyx_n_s_type_description); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 2097, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyObject_Dict_GetItem(__pyx_v_field_desc, __pyx_n_u_type_description); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 2097, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
     __pyx_t_3 = (__pyx_t_10 != Py_None);
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
     __pyx_t_13 = (__pyx_t_3 != 0);
     if (__pyx_t_13) {
 
       /* "pyrfc/_cyrfc.pyx":2098
  *         fieldDesc.decimals = field_desc['decimals']
  *         if field_desc['type_description'] is not None:
  *             fieldDesc.typeDescHandle = fillTypeDescription(field_desc['type_description'])             # <<<<<<<<<<<<<<
  *         else:
  *             fieldDesc.typeDescHandle = NULL
  */
-      __pyx_t_10 = __Pyx_PyObject_Dict_GetItem(__pyx_v_field_desc, __pyx_n_s_type_description); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 2098, __pyx_L1_error)
+      __pyx_t_10 = __Pyx_PyObject_Dict_GetItem(__pyx_v_field_desc, __pyx_n_u_type_description); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 2098, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
       __pyx_v_fieldDesc.typeDescHandle = __pyx_f_5pyrfc_6_cyrfc_fillTypeDescription(__pyx_t_10);
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
 
       /* "pyrfc/_cyrfc.pyx":2097
  *         fieldDesc.ucOffset = field_desc['uc_offset']
  *         fieldDesc.decimals = field_desc['decimals']
@@ -27344,28 +27878,28 @@
     /* "pyrfc/_cyrfc.pyx":2127
  * 
  *     for param_desc in func_desc.parameters:
  *         sapuc = fillString(param_desc['name'])             # <<<<<<<<<<<<<<
  *         strncpyU(paramDesc.name, sapuc, len(param_desc['name']) + 1)
  *         free(sapuc)
  */
-    __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_param_desc, __pyx_n_s_name); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2127, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_param_desc, __pyx_n_u_name); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2127, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_2 = __pyx_f_5pyrfc_6_cyrfc_fillString(__pyx_t_1); if (unlikely(__pyx_t_2 == ((SAP_UC *)NULL))) __PYX_ERR(0, 2127, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_v_sapuc = __pyx_t_2;
 
     /* "pyrfc/_cyrfc.pyx":2128
  *     for param_desc in func_desc.parameters:
  *         sapuc = fillString(param_desc['name'])
  *         strncpyU(paramDesc.name, sapuc, len(param_desc['name']) + 1)             # <<<<<<<<<<<<<<
  *         free(sapuc)
  *         paramDesc.type = RfcFieldType[param_desc['parameter_type']].value
  */
-    __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_param_desc, __pyx_n_s_name); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2128, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_param_desc, __pyx_n_u_name); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2128, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_7 = PyObject_Length(__pyx_t_1); if (unlikely(__pyx_t_7 == ((Py_ssize_t)-1))) __PYX_ERR(0, 2128, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     strncpyU(__pyx_v_paramDesc.name, __pyx_v_sapuc, (__pyx_t_7 + 1));
 
     /* "pyrfc/_cyrfc.pyx":2129
  *         sapuc = fillString(param_desc['name'])
@@ -27381,15 +27915,15 @@
  *         free(sapuc)
  *         paramDesc.type = RfcFieldType[param_desc['parameter_type']].value             # <<<<<<<<<<<<<<
  *         paramDesc.direction = RfcParameterDirection[param_desc['direction']].value
  *         paramDesc.nucLength = param_desc['nuc_length']
  */
     __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_RfcFieldType); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2130, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_8 = __Pyx_PyObject_Dict_GetItem(__pyx_v_param_desc, __pyx_n_s_parameter_type); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 2130, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_Dict_GetItem(__pyx_v_param_desc, __pyx_n_u_parameter_type); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 2130, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __pyx_t_9 = __Pyx_PyObject_GetItem(__pyx_t_1, __pyx_t_8); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 2130, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_value); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 2130, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
@@ -27403,15 +27937,15 @@
  *         paramDesc.type = RfcFieldType[param_desc['parameter_type']].value
  *         paramDesc.direction = RfcParameterDirection[param_desc['direction']].value             # <<<<<<<<<<<<<<
  *         paramDesc.nucLength = param_desc['nuc_length']
  *         paramDesc.ucLength = param_desc['uc_length']
  */
     __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_RfcParameterDirection); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 2131, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
-    __pyx_t_9 = __Pyx_PyObject_Dict_GetItem(__pyx_v_param_desc, __pyx_n_s_direction); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 2131, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyObject_Dict_GetItem(__pyx_v_param_desc, __pyx_n_u_direction); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 2131, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
     __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_t_8, __pyx_t_9); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2131, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
     __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_value); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 2131, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
@@ -27423,67 +27957,67 @@
     /* "pyrfc/_cyrfc.pyx":2132
  *         paramDesc.type = RfcFieldType[param_desc['parameter_type']].value
  *         paramDesc.direction = RfcParameterDirection[param_desc['direction']].value
  *         paramDesc.nucLength = param_desc['nuc_length']             # <<<<<<<<<<<<<<
  *         paramDesc.ucLength = param_desc['uc_length']
  *         paramDesc.decimals = param_desc['decimals']
  */
-    __pyx_t_9 = __Pyx_PyObject_Dict_GetItem(__pyx_v_param_desc, __pyx_n_s_nuc_length); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 2132, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyObject_Dict_GetItem(__pyx_v_param_desc, __pyx_n_u_nuc_length); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 2132, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
     __pyx_t_12 = __Pyx_PyInt_As_unsigned_int(__pyx_t_9); if (unlikely((__pyx_t_12 == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(0, 2132, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
     __pyx_v_paramDesc.nucLength = __pyx_t_12;
 
     /* "pyrfc/_cyrfc.pyx":2133
  *         paramDesc.direction = RfcParameterDirection[param_desc['direction']].value
  *         paramDesc.nucLength = param_desc['nuc_length']
  *         paramDesc.ucLength = param_desc['uc_length']             # <<<<<<<<<<<<<<
  *         paramDesc.decimals = param_desc['decimals']
  *         # defaultValue
  */
-    __pyx_t_9 = __Pyx_PyObject_Dict_GetItem(__pyx_v_param_desc, __pyx_n_s_uc_length); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 2133, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyObject_Dict_GetItem(__pyx_v_param_desc, __pyx_n_u_uc_length); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 2133, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
     __pyx_t_12 = __Pyx_PyInt_As_unsigned_int(__pyx_t_9); if (unlikely((__pyx_t_12 == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(0, 2133, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
     __pyx_v_paramDesc.ucLength = __pyx_t_12;
 
     /* "pyrfc/_cyrfc.pyx":2134
  *         paramDesc.nucLength = param_desc['nuc_length']
  *         paramDesc.ucLength = param_desc['uc_length']
  *         paramDesc.decimals = param_desc['decimals']             # <<<<<<<<<<<<<<
  *         # defaultValue
  *         sapuc = fillString(param_desc['default_value'])
  */
-    __pyx_t_9 = __Pyx_PyObject_Dict_GetItem(__pyx_v_param_desc, __pyx_n_s_decimals); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 2134, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyObject_Dict_GetItem(__pyx_v_param_desc, __pyx_n_u_decimals); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 2134, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
     __pyx_t_12 = __Pyx_PyInt_As_unsigned_int(__pyx_t_9); if (unlikely((__pyx_t_12 == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(0, 2134, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
     __pyx_v_paramDesc.decimals = __pyx_t_12;
 
     /* "pyrfc/_cyrfc.pyx":2136
  *         paramDesc.decimals = param_desc['decimals']
  *         # defaultValue
  *         sapuc = fillString(param_desc['default_value'])             # <<<<<<<<<<<<<<
  *         strncpyU(paramDesc.defaultValue, sapuc, len(param_desc['default_value']) + 1)
  *         free(sapuc)
  */
-    __pyx_t_9 = __Pyx_PyObject_Dict_GetItem(__pyx_v_param_desc, __pyx_n_s_default_value); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 2136, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyObject_Dict_GetItem(__pyx_v_param_desc, __pyx_n_u_default_value); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 2136, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
     __pyx_t_2 = __pyx_f_5pyrfc_6_cyrfc_fillString(__pyx_t_9); if (unlikely(__pyx_t_2 == ((SAP_UC *)NULL))) __PYX_ERR(0, 2136, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
     __pyx_v_sapuc = __pyx_t_2;
 
     /* "pyrfc/_cyrfc.pyx":2137
  *         # defaultValue
  *         sapuc = fillString(param_desc['default_value'])
  *         strncpyU(paramDesc.defaultValue, sapuc, len(param_desc['default_value']) + 1)             # <<<<<<<<<<<<<<
  *         free(sapuc)
  *         # parameterText
  */
-    __pyx_t_9 = __Pyx_PyObject_Dict_GetItem(__pyx_v_param_desc, __pyx_n_s_default_value); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 2137, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyObject_Dict_GetItem(__pyx_v_param_desc, __pyx_n_u_default_value); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 2137, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
     __pyx_t_7 = PyObject_Length(__pyx_t_9); if (unlikely(__pyx_t_7 == ((Py_ssize_t)-1))) __PYX_ERR(0, 2137, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
     strncpyU(__pyx_v_paramDesc.defaultValue, __pyx_v_sapuc, (__pyx_t_7 + 1));
 
     /* "pyrfc/_cyrfc.pyx":2138
  *         sapuc = fillString(param_desc['default_value'])
@@ -27497,28 +28031,28 @@
     /* "pyrfc/_cyrfc.pyx":2140
  *         free(sapuc)
  *         # parameterText
  *         sapuc = fillString(param_desc['parameter_text'])             # <<<<<<<<<<<<<<
  *         strncpyU(paramDesc.parameterText, sapuc, len(param_desc['parameter_text']) + 1)
  *         free(sapuc)
  */
-    __pyx_t_9 = __Pyx_PyObject_Dict_GetItem(__pyx_v_param_desc, __pyx_n_s_parameter_text); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 2140, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyObject_Dict_GetItem(__pyx_v_param_desc, __pyx_n_u_parameter_text); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 2140, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
     __pyx_t_2 = __pyx_f_5pyrfc_6_cyrfc_fillString(__pyx_t_9); if (unlikely(__pyx_t_2 == ((SAP_UC *)NULL))) __PYX_ERR(0, 2140, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
     __pyx_v_sapuc = __pyx_t_2;
 
     /* "pyrfc/_cyrfc.pyx":2141
  *         # parameterText
  *         sapuc = fillString(param_desc['parameter_text'])
  *         strncpyU(paramDesc.parameterText, sapuc, len(param_desc['parameter_text']) + 1)             # <<<<<<<<<<<<<<
  *         free(sapuc)
  *         paramDesc.optional = <bint> param_desc['optional']
  */
-    __pyx_t_9 = __Pyx_PyObject_Dict_GetItem(__pyx_v_param_desc, __pyx_n_s_parameter_text); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 2141, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyObject_Dict_GetItem(__pyx_v_param_desc, __pyx_n_u_parameter_text); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 2141, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
     __pyx_t_7 = PyObject_Length(__pyx_t_9); if (unlikely(__pyx_t_7 == ((Py_ssize_t)-1))) __PYX_ERR(0, 2141, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
     strncpyU(__pyx_v_paramDesc.parameterText, __pyx_v_sapuc, (__pyx_t_7 + 1));
 
     /* "pyrfc/_cyrfc.pyx":2142
  *         sapuc = fillString(param_desc['parameter_text'])
@@ -27532,42 +28066,42 @@
     /* "pyrfc/_cyrfc.pyx":2143
  *         strncpyU(paramDesc.parameterText, sapuc, len(param_desc['parameter_text']) + 1)
  *         free(sapuc)
  *         paramDesc.optional = <bint> param_desc['optional']             # <<<<<<<<<<<<<<
  *         if param_desc['type_description'] is not None:
  *             paramDesc.typeDescHandle = fillTypeDescription(param_desc['type_description'])
  */
-    __pyx_t_9 = __Pyx_PyObject_Dict_GetItem(__pyx_v_param_desc, __pyx_n_s_optional); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 2143, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyObject_Dict_GetItem(__pyx_v_param_desc, __pyx_n_u_optional); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 2143, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
     __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_9); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 2143, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
     __pyx_v_paramDesc.optional = __pyx_t_3;
 
     /* "pyrfc/_cyrfc.pyx":2144
  *         free(sapuc)
  *         paramDesc.optional = <bint> param_desc['optional']
  *         if param_desc['type_description'] is not None:             # <<<<<<<<<<<<<<
  *             paramDesc.typeDescHandle = fillTypeDescription(param_desc['type_description'])
  *         else:
  */
-    __pyx_t_9 = __Pyx_PyObject_Dict_GetItem(__pyx_v_param_desc, __pyx_n_s_type_description); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 2144, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyObject_Dict_GetItem(__pyx_v_param_desc, __pyx_n_u_type_description); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 2144, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
     __pyx_t_3 = (__pyx_t_9 != Py_None);
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
     __pyx_t_13 = (__pyx_t_3 != 0);
     if (__pyx_t_13) {
 
       /* "pyrfc/_cyrfc.pyx":2145
  *         paramDesc.optional = <bint> param_desc['optional']
  *         if param_desc['type_description'] is not None:
  *             paramDesc.typeDescHandle = fillTypeDescription(param_desc['type_description'])             # <<<<<<<<<<<<<<
  *         else:
  *             paramDesc.typeDescHandle = NULL
  */
-      __pyx_t_9 = __Pyx_PyObject_Dict_GetItem(__pyx_v_param_desc, __pyx_n_s_type_description); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 2145, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyObject_Dict_GetItem(__pyx_v_param_desc, __pyx_n_u_type_description); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 2145, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
       __pyx_v_paramDesc.typeDescHandle = __pyx_f_5pyrfc_6_cyrfc_fillTypeDescription(__pyx_t_9);
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
 
       /* "pyrfc/_cyrfc.pyx":2144
  *         free(sapuc)
  *         paramDesc.optional = <bint> param_desc['optional']
@@ -27721,37 +28255,37 @@
   /* "pyrfc/_cyrfc.pyx":2159
  *     cdef RFC_UNIT_IDENTIFIER uIdentifier
  *     cdef SAP_UC* sapuc
  *     uIdentifier.unitType = fillString("Q" if unit['queued'] else "T")[0]             # <<<<<<<<<<<<<<
  *     if len(unit['id']) != RFC_UNITID_LN:
  *         raise RFCError(f"Invalid length of unit['id'] (should be {RFC_UNITID_LN}, but found {len(unit['id'])}).")
  */
-  __pyx_t_2 = __Pyx_PyObject_Dict_GetItem(__pyx_v_unit, __pyx_n_s_queued); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2159, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Dict_GetItem(__pyx_v_unit, __pyx_n_u_queued); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2159, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 2159, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (__pyx_t_3) {
-    __Pyx_INCREF(__pyx_n_s_Q);
-    __pyx_t_1 = __pyx_n_s_Q;
+    __Pyx_INCREF(__pyx_n_u_Q);
+    __pyx_t_1 = __pyx_n_u_Q;
   } else {
-    __Pyx_INCREF(__pyx_n_s_T);
-    __pyx_t_1 = __pyx_n_s_T;
+    __Pyx_INCREF(__pyx_n_u_T);
+    __pyx_t_1 = __pyx_n_u_T;
   }
   __pyx_t_4 = __pyx_f_5pyrfc_6_cyrfc_fillString(__pyx_t_1); if (unlikely(__pyx_t_4 == ((SAP_UC *)NULL))) __PYX_ERR(0, 2159, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_uIdentifier.unitType = (__pyx_t_4[0]);
 
   /* "pyrfc/_cyrfc.pyx":2160
  *     cdef SAP_UC* sapuc
  *     uIdentifier.unitType = fillString("Q" if unit['queued'] else "T")[0]
  *     if len(unit['id']) != RFC_UNITID_LN:             # <<<<<<<<<<<<<<
  *         raise RFCError(f"Invalid length of unit['id'] (should be {RFC_UNITID_LN}, but found {len(unit['id'])}).")
  *     sapuc = fillString(unit['id'])
  */
-  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_unit, __pyx_n_s_id); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2160, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_unit, __pyx_n_u_id); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2160, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_5 = PyObject_Length(__pyx_t_1); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 2160, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_3 = ((__pyx_t_5 != RFC_UNITID_LN) != 0);
   if (unlikely(__pyx_t_3)) {
 
     /* "pyrfc/_cyrfc.pyx":2161
@@ -27777,28 +28311,28 @@
     __Pyx_GIVEREF(__pyx_t_8);
     PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_t_8);
     __pyx_t_8 = 0;
     __Pyx_INCREF(__pyx_kp_u_but_found);
     __pyx_t_5 += 12;
     __Pyx_GIVEREF(__pyx_kp_u_but_found);
     PyTuple_SET_ITEM(__pyx_t_6, 2, __pyx_kp_u_but_found);
-    __pyx_t_8 = __Pyx_PyObject_Dict_GetItem(__pyx_v_unit, __pyx_n_s_id); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 2161, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_Dict_GetItem(__pyx_v_unit, __pyx_n_u_id); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 2161, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __pyx_t_9 = PyObject_Length(__pyx_t_8); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1))) __PYX_ERR(0, 2161, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     __pyx_t_8 = __Pyx_PyUnicode_From_Py_ssize_t(__pyx_t_9, 0, ' ', 'd'); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 2161, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __pyx_t_5 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_8);
     __Pyx_GIVEREF(__pyx_t_8);
     PyTuple_SET_ITEM(__pyx_t_6, 3, __pyx_t_8);
     __pyx_t_8 = 0;
-    __Pyx_INCREF(__pyx_kp_u__28);
+    __Pyx_INCREF(__pyx_kp_u__29);
     __pyx_t_5 += 2;
-    __Pyx_GIVEREF(__pyx_kp_u__28);
-    PyTuple_SET_ITEM(__pyx_t_6, 4, __pyx_kp_u__28);
+    __Pyx_GIVEREF(__pyx_kp_u__29);
+    PyTuple_SET_ITEM(__pyx_t_6, 4, __pyx_kp_u__29);
     __pyx_t_8 = __Pyx_PyUnicode_Join(__pyx_t_6, 5, __pyx_t_5, __pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 2161, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __pyx_t_6 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_6)) {
@@ -27830,15 +28364,15 @@
   /* "pyrfc/_cyrfc.pyx":2162
  *     if len(unit['id']) != RFC_UNITID_LN:
  *         raise RFCError(f"Invalid length of unit['id'] (should be {RFC_UNITID_LN}, but found {len(unit['id'])}).")
  *     sapuc = fillString(unit['id'])             # <<<<<<<<<<<<<<
  *     strncpyU(uIdentifier.unitID, sapuc, RFC_UNITID_LN + 1)
  *     free(sapuc)
  */
-  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_unit, __pyx_n_s_id); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2162, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_unit, __pyx_n_u_id); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2162, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_4 = __pyx_f_5pyrfc_6_cyrfc_fillString(__pyx_t_1); if (unlikely(__pyx_t_4 == ((SAP_UC *)NULL))) __PYX_ERR(0, 2162, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_sapuc = __pyx_t_4;
 
   /* "pyrfc/_cyrfc.pyx":2163
  *         raise RFCError(f"Invalid length of unit['id'] (should be {RFC_UNITID_LN}, but found {len(unit['id'])}).")
@@ -28176,23 +28710,23 @@
  *             if not isinstance(conn, Connection):
  *                 raise TypeError('Connection object required, received', conn, 'of type', type(conn))             # <<<<<<<<<<<<<<
  *             self.setOnConnection(conn)
  * 
  */
       __pyx_t_4 = PyTuple_New(4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 2191, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __Pyx_INCREF(__pyx_kp_s_Connection_object_required_recei);
-      __Pyx_GIVEREF(__pyx_kp_s_Connection_object_required_recei);
-      PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_kp_s_Connection_object_required_recei);
+      __Pyx_INCREF(__pyx_kp_u_Connection_object_required_recei);
+      __Pyx_GIVEREF(__pyx_kp_u_Connection_object_required_recei);
+      PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_kp_u_Connection_object_required_recei);
       __Pyx_INCREF(__pyx_v_conn);
       __Pyx_GIVEREF(__pyx_v_conn);
       PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_v_conn);
-      __Pyx_INCREF(__pyx_kp_s_of_type);
-      __Pyx_GIVEREF(__pyx_kp_s_of_type);
-      PyTuple_SET_ITEM(__pyx_t_4, 2, __pyx_kp_s_of_type);
+      __Pyx_INCREF(__pyx_kp_u_of_type);
+      __Pyx_GIVEREF(__pyx_kp_u_of_type);
+      PyTuple_SET_ITEM(__pyx_t_4, 2, __pyx_kp_u_of_type);
       __Pyx_INCREF(((PyObject *)Py_TYPE(__pyx_v_conn)));
       __Pyx_GIVEREF(((PyObject *)Py_TYPE(__pyx_v_conn)));
       PyTuple_SET_ITEM(__pyx_t_4, 3, ((PyObject *)Py_TYPE(__pyx_v_conn)));
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_t_4, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 2191, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
@@ -29485,15 +30019,15 @@
       if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_4);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
-    __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_kp_s_No_connections_assigned) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_kp_s_No_connections_assigned);
+    __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_kp_u_No_connections_assigned) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_kp_u_No_connections_assigned);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2330, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __PYX_ERR(0, 2330, __pyx_L1_error)
@@ -29553,15 +30087,15 @@
  *             raise wrapError(&errorInfo)
  *         _stats['numberOfCalls'] = numberOfCalls             # <<<<<<<<<<<<<<
  * 
  *         rc = RfcGetSentBytes (self._throughput_handle, &sentBytes, &errorInfo)
  */
   __pyx_t_1 = __Pyx_PyInt_From_SAP_ULLONG(__pyx_v_numberOfCalls); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2335, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (unlikely(PyDict_SetItem(__pyx_v__stats, __pyx_n_s_numberOfCalls, __pyx_t_1) < 0)) __PYX_ERR(0, 2335, __pyx_L1_error)
+  if (unlikely(PyDict_SetItem(__pyx_v__stats, __pyx_n_u_numberOfCalls, __pyx_t_1) < 0)) __PYX_ERR(0, 2335, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "pyrfc/_cyrfc.pyx":2337
  *         _stats['numberOfCalls'] = numberOfCalls
  * 
  *         rc = RfcGetSentBytes (self._throughput_handle, &sentBytes, &errorInfo)             # <<<<<<<<<<<<<<
  *         if rc != RFC_OK:
@@ -29606,15 +30140,15 @@
  *             raise wrapError(&errorInfo)
  *         _stats['sentBytes'] = sentBytes             # <<<<<<<<<<<<<<
  * 
  *         rc = RfcGetReceivedBytes (self._throughput_handle, &receivedBytes, &errorInfo)
  */
   __pyx_t_1 = __Pyx_PyInt_From_SAP_ULLONG(__pyx_v_sentBytes); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2340, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (unlikely(PyDict_SetItem(__pyx_v__stats, __pyx_n_s_sentBytes, __pyx_t_1) < 0)) __PYX_ERR(0, 2340, __pyx_L1_error)
+  if (unlikely(PyDict_SetItem(__pyx_v__stats, __pyx_n_u_sentBytes, __pyx_t_1) < 0)) __PYX_ERR(0, 2340, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "pyrfc/_cyrfc.pyx":2342
  *         _stats['sentBytes'] = sentBytes
  * 
  *         rc = RfcGetReceivedBytes (self._throughput_handle, &receivedBytes, &errorInfo)             # <<<<<<<<<<<<<<
  *         if rc != RFC_OK:
@@ -29659,15 +30193,15 @@
  *             raise wrapError(&errorInfo)
  *         _stats['receivedBytes'] = receivedBytes             # <<<<<<<<<<<<<<
  * 
  *         rc = RfcGetApplicationTime (self._throughput_handle, &applicationTime, &errorInfo)
  */
   __pyx_t_1 = __Pyx_PyInt_From_SAP_ULLONG(__pyx_v_receivedBytes); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2345, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (unlikely(PyDict_SetItem(__pyx_v__stats, __pyx_n_s_receivedBytes, __pyx_t_1) < 0)) __PYX_ERR(0, 2345, __pyx_L1_error)
+  if (unlikely(PyDict_SetItem(__pyx_v__stats, __pyx_n_u_receivedBytes, __pyx_t_1) < 0)) __PYX_ERR(0, 2345, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "pyrfc/_cyrfc.pyx":2347
  *         _stats['receivedBytes'] = receivedBytes
  * 
  *         rc = RfcGetApplicationTime (self._throughput_handle, &applicationTime, &errorInfo)             # <<<<<<<<<<<<<<
  *         if rc != RFC_OK:
@@ -29712,15 +30246,15 @@
  *             raise wrapError(&errorInfo)
  *         _stats['applicationTime'] = applicationTime             # <<<<<<<<<<<<<<
  * 
  *         rc = RfcGetTotalTime (self._throughput_handle, &totalTime, &errorInfo)
  */
   __pyx_t_1 = __Pyx_PyInt_From_SAP_ULLONG(__pyx_v_applicationTime); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2350, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (unlikely(PyDict_SetItem(__pyx_v__stats, __pyx_n_s_applicationTime, __pyx_t_1) < 0)) __PYX_ERR(0, 2350, __pyx_L1_error)
+  if (unlikely(PyDict_SetItem(__pyx_v__stats, __pyx_n_u_applicationTime, __pyx_t_1) < 0)) __PYX_ERR(0, 2350, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "pyrfc/_cyrfc.pyx":2352
  *         _stats['applicationTime'] = applicationTime
  * 
  *         rc = RfcGetTotalTime (self._throughput_handle, &totalTime, &errorInfo)             # <<<<<<<<<<<<<<
  *         if rc != RFC_OK:
@@ -29765,15 +30299,15 @@
  *             raise wrapError(&errorInfo)
  *         _stats['totalTime'] = totalTime             # <<<<<<<<<<<<<<
  * 
  *         rc = RfcGetSerializationTime (self._throughput_handle, &serializationTime, &errorInfo)
  */
   __pyx_t_1 = __Pyx_PyInt_From_SAP_ULLONG(__pyx_v_totalTime); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2355, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (unlikely(PyDict_SetItem(__pyx_v__stats, __pyx_n_s_totalTime, __pyx_t_1) < 0)) __PYX_ERR(0, 2355, __pyx_L1_error)
+  if (unlikely(PyDict_SetItem(__pyx_v__stats, __pyx_n_u_totalTime, __pyx_t_1) < 0)) __PYX_ERR(0, 2355, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "pyrfc/_cyrfc.pyx":2357
  *         _stats['totalTime'] = totalTime
  * 
  *         rc = RfcGetSerializationTime (self._throughput_handle, &serializationTime, &errorInfo)             # <<<<<<<<<<<<<<
  *         if rc != RFC_OK:
@@ -29818,15 +30352,15 @@
  *             raise wrapError(&errorInfo)
  *         _stats['serializationTime'] = serializationTime             # <<<<<<<<<<<<<<
  * 
  *         rc = RfcGetDeserializationTime (self._throughput_handle, &deserializationTime, &errorInfo)
  */
   __pyx_t_1 = __Pyx_PyInt_From_SAP_ULLONG(__pyx_v_serializationTime); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2360, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (unlikely(PyDict_SetItem(__pyx_v__stats, __pyx_n_s_serializationTime, __pyx_t_1) < 0)) __PYX_ERR(0, 2360, __pyx_L1_error)
+  if (unlikely(PyDict_SetItem(__pyx_v__stats, __pyx_n_u_serializationTime, __pyx_t_1) < 0)) __PYX_ERR(0, 2360, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "pyrfc/_cyrfc.pyx":2362
  *         _stats['serializationTime'] = serializationTime
  * 
  *         rc = RfcGetDeserializationTime (self._throughput_handle, &deserializationTime, &errorInfo)             # <<<<<<<<<<<<<<
  *         if rc != RFC_OK:
@@ -29871,15 +30405,15 @@
  *             raise wrapError(&errorInfo)
  *         _stats['deserializationTime'] = deserializationTime             # <<<<<<<<<<<<<<
  * 
  *         return _stats
  */
   __pyx_t_1 = __Pyx_PyInt_From_SAP_ULLONG(__pyx_v_deserializationTime); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2365, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (unlikely(PyDict_SetItem(__pyx_v__stats, __pyx_n_s_deserializationTime, __pyx_t_1) < 0)) __PYX_ERR(0, 2365, __pyx_L1_error)
+  if (unlikely(PyDict_SetItem(__pyx_v__stats, __pyx_n_u_deserializationTime, __pyx_t_1) < 0)) __PYX_ERR(0, 2365, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "pyrfc/_cyrfc.pyx":2367
  *         _stats['deserializationTime'] = deserializationTime
  * 
  *         return _stats             # <<<<<<<<<<<<<<
  * 
@@ -29942,15 +30476,15 @@
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("self._throughput_handle cannot be converted to a Python object for pickling")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("self._throughput_handle cannot be converted to a Python object for pickling")
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__35, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 2, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__36, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(1, 2, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
@@ -29998,15 +30532,15 @@
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":4
  *     raise TypeError("self._throughput_handle cannot be converted to a Python object for pickling")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("self._throughput_handle cannot be converted to a Python object for pickling")             # <<<<<<<<<<<<<<
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__36, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__37, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(1, 4, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
@@ -30436,15 +30970,15 @@
  *                 fillStructureField(typeDesc, lineHandle, name, value)
  *         else:
  *             fillStructureField(typeDesc, lineHandle, '', line)             # <<<<<<<<<<<<<<
  *         i += 1
  * 
  */
     /*else*/ {
-      __pyx_t_3 = __pyx_f_5pyrfc_6_cyrfc_fillStructureField(__pyx_v_typeDesc, __pyx_v_lineHandle, __pyx_kp_s__5, __pyx_v_line); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2410, __pyx_L1_error)
+      __pyx_t_3 = __pyx_f_5pyrfc_6_cyrfc_fillStructureField(__pyx_v_typeDesc, __pyx_v_lineHandle, __pyx_kp_u__5, __pyx_v_line); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2410, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     }
     __pyx_L6:;
 
     /* "pyrfc/_cyrfc.pyx":2411
  *         else:
@@ -30520,20 +31054,29 @@
   SAP_RAW *__pyx_t_13;
   SAP_UC *__pyx_t_14;
   PyObject *__pyx_t_15 = NULL;
   PyObject *__pyx_t_16 = NULL;
   PyObject *__pyx_t_17 = NULL;
   PyObject *__pyx_t_18 = NULL;
   PyObject *__pyx_t_19 = NULL;
-  int __pyx_t_20;
+  char const *__pyx_t_20;
   PyObject *__pyx_t_21 = NULL;
-  RFC_INT __pyx_t_22;
-  RFC_INT8 __pyx_t_23;
-  Py_UCS4 __pyx_t_24;
+  PyObject *__pyx_t_22 = NULL;
+  PyObject *__pyx_t_23 = NULL;
+  PyObject *__pyx_t_24 = NULL;
   PyObject *__pyx_t_25 = NULL;
+  PyObject *__pyx_t_26 = NULL;
+  int __pyx_t_27;
+  PyObject *__pyx_t_28 = NULL;
+  char const *__pyx_t_29;
+  RFC_INT __pyx_t_30;
+  RFC_INT8 __pyx_t_31;
+  Py_UCS4 __pyx_t_32;
+  PyObject *__pyx_t_33 = NULL;
+  char const *__pyx_t_34;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("fillVariable", 0);
   __Pyx_INCREF(__pyx_v_value);
 
   /* "pyrfc/_cyrfc.pyx":2422
@@ -30576,21 +31119,21 @@
           /* "pyrfc/_cyrfc.pyx":2425
  *         if typ == RFCTYPE_STRUCTURE:
  *             if type(value) is not dict:
  *                 raise TypeError('dictionary required for structure parameter, received', str(type(value)))             # <<<<<<<<<<<<<<
  *             rc = RfcGetStructure(container, cName, &struct, &errorInfo)
  *             if rc != RFC_OK:
  */
-          __pyx_t_6 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyString_Type)), ((PyObject *)Py_TYPE(__pyx_v_value))); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 2425, __pyx_L3_error)
+          __pyx_t_6 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyUnicode_Type)), ((PyObject *)Py_TYPE(__pyx_v_value))); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 2425, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_6);
           __pyx_t_7 = PyTuple_New(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 2425, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_7);
-          __Pyx_INCREF(__pyx_kp_s_dictionary_required_for_structur);
-          __Pyx_GIVEREF(__pyx_kp_s_dictionary_required_for_structur);
-          PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_kp_s_dictionary_required_for_structur);
+          __Pyx_INCREF(__pyx_kp_u_dictionary_required_for_structur);
+          __Pyx_GIVEREF(__pyx_kp_u_dictionary_required_for_structur);
+          PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_kp_u_dictionary_required_for_structur);
           __Pyx_GIVEREF(__pyx_t_6);
           PyTuple_SET_ITEM(__pyx_t_7, 1, __pyx_t_6);
           __pyx_t_6 = 0;
           __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_t_7, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 2425, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_6);
           __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
           __Pyx_Raise(__pyx_t_6, 0, 0, 0);
@@ -30712,21 +31255,21 @@
           /* "pyrfc/_cyrfc.pyx":2433
  *         elif typ == RFCTYPE_TABLE:
  *             if type(value) is not list:
  *                 raise TypeError('list required for table parameter, received', str(type(value)))             # <<<<<<<<<<<<<<
  *             rc = RfcGetTable(container, cName, &table, &errorInfo)
  *             if rc != RFC_OK:
  */
-          __pyx_t_6 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyString_Type)), ((PyObject *)Py_TYPE(__pyx_v_value))); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 2433, __pyx_L3_error)
+          __pyx_t_6 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyUnicode_Type)), ((PyObject *)Py_TYPE(__pyx_v_value))); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 2433, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_6);
           __pyx_t_11 = PyTuple_New(2); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 2433, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_11);
-          __Pyx_INCREF(__pyx_kp_s_list_required_for_table_paramete);
-          __Pyx_GIVEREF(__pyx_kp_s_list_required_for_table_paramete);
-          PyTuple_SET_ITEM(__pyx_t_11, 0, __pyx_kp_s_list_required_for_table_paramete);
+          __Pyx_INCREF(__pyx_kp_u_list_required_for_table_paramete);
+          __Pyx_GIVEREF(__pyx_kp_u_list_required_for_table_paramete);
+          PyTuple_SET_ITEM(__pyx_t_11, 0, __pyx_kp_u_list_required_for_table_paramete);
           __Pyx_GIVEREF(__pyx_t_6);
           PyTuple_SET_ITEM(__pyx_t_11, 1, __pyx_t_6);
           __pyx_t_6 = 0;
           __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_t_11, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 2433, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_6);
           __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
           __Pyx_Raise(__pyx_t_6, 0, 0, 0);
@@ -30885,36 +31428,36 @@
         /* "pyrfc/_cyrfc.pyx":2447
  *             free(bValue)
  *         elif typ == RFCTYPE_CHAR:
  *             if type(value) is not str:             # <<<<<<<<<<<<<<
  *                 raise TypeError('an string is required, received', value, 'of type', type(value))
  *             cValue = fillString(value)
  */
-        __pyx_t_4 = (((PyObject *)Py_TYPE(__pyx_v_value)) != ((PyObject *)(&PyString_Type)));
+        __pyx_t_4 = (((PyObject *)Py_TYPE(__pyx_v_value)) != ((PyObject *)(&PyUnicode_Type)));
         __pyx_t_5 = (__pyx_t_4 != 0);
         if (unlikely(__pyx_t_5)) {
 
           /* "pyrfc/_cyrfc.pyx":2448
  *         elif typ == RFCTYPE_CHAR:
  *             if type(value) is not str:
  *                 raise TypeError('an string is required, received', value, 'of type', type(value))             # <<<<<<<<<<<<<<
  *             cValue = fillString(value)
  *             rc = RfcSetChars(container, cName, cValue, strlenU(cValue), &errorInfo)
  */
           __pyx_t_6 = PyTuple_New(4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 2448, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_6);
-          __Pyx_INCREF(__pyx_kp_s_an_string_is_required_received);
-          __Pyx_GIVEREF(__pyx_kp_s_an_string_is_required_received);
-          PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_kp_s_an_string_is_required_received);
+          __Pyx_INCREF(__pyx_kp_u_an_string_is_required_received);
+          __Pyx_GIVEREF(__pyx_kp_u_an_string_is_required_received);
+          PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_kp_u_an_string_is_required_received);
           __Pyx_INCREF(__pyx_v_value);
           __Pyx_GIVEREF(__pyx_v_value);
           PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_v_value);
-          __Pyx_INCREF(__pyx_kp_s_of_type);
-          __Pyx_GIVEREF(__pyx_kp_s_of_type);
-          PyTuple_SET_ITEM(__pyx_t_6, 2, __pyx_kp_s_of_type);
+          __Pyx_INCREF(__pyx_kp_u_of_type);
+          __Pyx_GIVEREF(__pyx_kp_u_of_type);
+          PyTuple_SET_ITEM(__pyx_t_6, 2, __pyx_kp_u_of_type);
           __Pyx_INCREF(((PyObject *)Py_TYPE(__pyx_v_value)));
           __Pyx_GIVEREF(((PyObject *)Py_TYPE(__pyx_v_value)));
           PyTuple_SET_ITEM(__pyx_t_6, 3, ((PyObject *)Py_TYPE(__pyx_v_value)));
           __pyx_t_11 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_t_6, NULL); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 2448, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_11);
           __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
           __Pyx_Raise(__pyx_t_11, 0, 0, 0);
@@ -30971,36 +31514,36 @@
         /* "pyrfc/_cyrfc.pyx":2453
  *             free(cValue)
  *         elif typ == RFCTYPE_STRING:
  *             if type(value) is not str:             # <<<<<<<<<<<<<<
  *                 raise TypeError('an string is required, received', value, 'of type', type(value))
  *             cValue = fillString(value)
  */
-        __pyx_t_5 = (((PyObject *)Py_TYPE(__pyx_v_value)) != ((PyObject *)(&PyString_Type)));
+        __pyx_t_5 = (((PyObject *)Py_TYPE(__pyx_v_value)) != ((PyObject *)(&PyUnicode_Type)));
         __pyx_t_4 = (__pyx_t_5 != 0);
         if (unlikely(__pyx_t_4)) {
 
           /* "pyrfc/_cyrfc.pyx":2454
  *         elif typ == RFCTYPE_STRING:
  *             if type(value) is not str:
  *                 raise TypeError('an string is required, received', value, 'of type', type(value))             # <<<<<<<<<<<<<<
  *             cValue = fillString(value)
  *             rc = RfcSetString(container, cName, cValue, strlenU(cValue), &errorInfo)
  */
           __pyx_t_11 = PyTuple_New(4); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 2454, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_11);
-          __Pyx_INCREF(__pyx_kp_s_an_string_is_required_received);
-          __Pyx_GIVEREF(__pyx_kp_s_an_string_is_required_received);
-          PyTuple_SET_ITEM(__pyx_t_11, 0, __pyx_kp_s_an_string_is_required_received);
+          __Pyx_INCREF(__pyx_kp_u_an_string_is_required_received);
+          __Pyx_GIVEREF(__pyx_kp_u_an_string_is_required_received);
+          PyTuple_SET_ITEM(__pyx_t_11, 0, __pyx_kp_u_an_string_is_required_received);
           __Pyx_INCREF(__pyx_v_value);
           __Pyx_GIVEREF(__pyx_v_value);
           PyTuple_SET_ITEM(__pyx_t_11, 1, __pyx_v_value);
-          __Pyx_INCREF(__pyx_kp_s_of_type);
-          __Pyx_GIVEREF(__pyx_kp_s_of_type);
-          PyTuple_SET_ITEM(__pyx_t_11, 2, __pyx_kp_s_of_type);
+          __Pyx_INCREF(__pyx_kp_u_of_type);
+          __Pyx_GIVEREF(__pyx_kp_u_of_type);
+          PyTuple_SET_ITEM(__pyx_t_11, 2, __pyx_kp_u_of_type);
           __Pyx_INCREF(((PyObject *)Py_TYPE(__pyx_v_value)));
           __Pyx_GIVEREF(((PyObject *)Py_TYPE(__pyx_v_value)));
           PyTuple_SET_ITEM(__pyx_t_11, 3, ((PyObject *)Py_TYPE(__pyx_v_value)));
           __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_t_11, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 2454, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_6);
           __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
           __Pyx_Raise(__pyx_t_6, 0, 0, 0);
@@ -31177,42 +31720,88 @@
             __Pyx_AddTraceback("pyrfc._cyrfc.fillVariable", __pyx_clineno, __pyx_lineno, __pyx_filename);
             if (__Pyx_GetException(&__pyx_t_6, &__pyx_t_11, &__pyx_t_7) < 0) __PYX_ERR(0, 2466, __pyx_L19_except_error)
             __Pyx_GOTREF(__pyx_t_6);
             __Pyx_GOTREF(__pyx_t_11);
             __Pyx_GOTREF(__pyx_t_7);
             __Pyx_INCREF(__pyx_t_11);
             __pyx_v_ex = __pyx_t_11;
+            /*try:*/ {
 
-            /* "pyrfc/_cyrfc.pyx":2467
+              /* "pyrfc/_cyrfc.pyx":2467
  *                     raise
  *             except Exception as ex:
  *                 raise TypeError('a numeric string is required, received', value, 'of type', type(value))             # <<<<<<<<<<<<<<
  *         elif typ == RFCTYPE_BCD or typ == RFCTYPE_FLOAT or typ == RFCTYPE_DECF16 or typ == RFCTYPE_DECF34:
  *             # cast to string prevents rounding errors in NWRFC SDK
  */
-            __pyx_t_18 = PyTuple_New(4); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 2467, __pyx_L19_except_error)
-            __Pyx_GOTREF(__pyx_t_18);
-            __Pyx_INCREF(__pyx_kp_s_a_numeric_string_is_required_rec);
-            __Pyx_GIVEREF(__pyx_kp_s_a_numeric_string_is_required_rec);
-            PyTuple_SET_ITEM(__pyx_t_18, 0, __pyx_kp_s_a_numeric_string_is_required_rec);
-            __Pyx_INCREF(__pyx_v_value);
-            __Pyx_GIVEREF(__pyx_v_value);
-            PyTuple_SET_ITEM(__pyx_t_18, 1, __pyx_v_value);
-            __Pyx_INCREF(__pyx_kp_s_of_type);
-            __Pyx_GIVEREF(__pyx_kp_s_of_type);
-            PyTuple_SET_ITEM(__pyx_t_18, 2, __pyx_kp_s_of_type);
-            __Pyx_INCREF(((PyObject *)Py_TYPE(__pyx_v_value)));
-            __Pyx_GIVEREF(((PyObject *)Py_TYPE(__pyx_v_value)));
-            PyTuple_SET_ITEM(__pyx_t_18, 3, ((PyObject *)Py_TYPE(__pyx_v_value)));
-            __pyx_t_19 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_t_18, NULL); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 2467, __pyx_L19_except_error)
-            __Pyx_GOTREF(__pyx_t_19);
-            __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
-            __Pyx_Raise(__pyx_t_19, 0, 0, 0);
-            __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
-            __PYX_ERR(0, 2467, __pyx_L19_except_error)
+              __pyx_t_18 = PyTuple_New(4); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 2467, __pyx_L29_error)
+              __Pyx_GOTREF(__pyx_t_18);
+              __Pyx_INCREF(__pyx_kp_u_a_numeric_string_is_required_rec);
+              __Pyx_GIVEREF(__pyx_kp_u_a_numeric_string_is_required_rec);
+              PyTuple_SET_ITEM(__pyx_t_18, 0, __pyx_kp_u_a_numeric_string_is_required_rec);
+              __Pyx_INCREF(__pyx_v_value);
+              __Pyx_GIVEREF(__pyx_v_value);
+              PyTuple_SET_ITEM(__pyx_t_18, 1, __pyx_v_value);
+              __Pyx_INCREF(__pyx_kp_u_of_type);
+              __Pyx_GIVEREF(__pyx_kp_u_of_type);
+              PyTuple_SET_ITEM(__pyx_t_18, 2, __pyx_kp_u_of_type);
+              __Pyx_INCREF(((PyObject *)Py_TYPE(__pyx_v_value)));
+              __Pyx_GIVEREF(((PyObject *)Py_TYPE(__pyx_v_value)));
+              PyTuple_SET_ITEM(__pyx_t_18, 3, ((PyObject *)Py_TYPE(__pyx_v_value)));
+              __pyx_t_19 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_t_18, NULL); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 2467, __pyx_L29_error)
+              __Pyx_GOTREF(__pyx_t_19);
+              __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
+              __Pyx_Raise(__pyx_t_19, 0, 0, 0);
+              __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
+              __PYX_ERR(0, 2467, __pyx_L29_error)
+            }
+
+            /* "pyrfc/_cyrfc.pyx":2466
+ *                 else:
+ *                     raise
+ *             except Exception as ex:             # <<<<<<<<<<<<<<
+ *                 raise TypeError('a numeric string is required, received', value, 'of type', type(value))
+ *         elif typ == RFCTYPE_BCD or typ == RFCTYPE_FLOAT or typ == RFCTYPE_DECF16 or typ == RFCTYPE_DECF34:
+ */
+            /*finally:*/ {
+              __pyx_L29_error:;
+              /*exception exit:*/{
+                __Pyx_PyThreadState_declare
+                __Pyx_PyThreadState_assign
+                __pyx_t_21 = 0; __pyx_t_22 = 0; __pyx_t_23 = 0; __pyx_t_24 = 0; __pyx_t_25 = 0; __pyx_t_26 = 0;
+                __Pyx_XDECREF(__pyx_t_18); __pyx_t_18 = 0;
+                __Pyx_XDECREF(__pyx_t_19); __pyx_t_19 = 0;
+                if (PY_MAJOR_VERSION >= 3) __Pyx_ExceptionSwap(&__pyx_t_24, &__pyx_t_25, &__pyx_t_26);
+                if ((PY_MAJOR_VERSION < 3) || unlikely(__Pyx_GetException(&__pyx_t_21, &__pyx_t_22, &__pyx_t_23) < 0)) __Pyx_ErrFetch(&__pyx_t_21, &__pyx_t_22, &__pyx_t_23);
+                __Pyx_XGOTREF(__pyx_t_21);
+                __Pyx_XGOTREF(__pyx_t_22);
+                __Pyx_XGOTREF(__pyx_t_23);
+                __Pyx_XGOTREF(__pyx_t_24);
+                __Pyx_XGOTREF(__pyx_t_25);
+                __Pyx_XGOTREF(__pyx_t_26);
+                __pyx_t_10 = __pyx_lineno; __pyx_t_12 = __pyx_clineno; __pyx_t_20 = __pyx_filename;
+                {
+                  __Pyx_DECREF(__pyx_v_ex);
+                  __pyx_v_ex = NULL;
+                }
+                if (PY_MAJOR_VERSION >= 3) {
+                  __Pyx_XGIVEREF(__pyx_t_24);
+                  __Pyx_XGIVEREF(__pyx_t_25);
+                  __Pyx_XGIVEREF(__pyx_t_26);
+                  __Pyx_ExceptionReset(__pyx_t_24, __pyx_t_25, __pyx_t_26);
+                }
+                __Pyx_XGIVEREF(__pyx_t_21);
+                __Pyx_XGIVEREF(__pyx_t_22);
+                __Pyx_XGIVEREF(__pyx_t_23);
+                __Pyx_ErrRestore(__pyx_t_21, __pyx_t_22, __pyx_t_23);
+                __pyx_t_21 = 0; __pyx_t_22 = 0; __pyx_t_23 = 0; __pyx_t_24 = 0; __pyx_t_25 = 0; __pyx_t_26 = 0;
+                __pyx_lineno = __pyx_t_10; __pyx_clineno = __pyx_t_12; __pyx_filename = __pyx_t_20;
+                goto __pyx_L19_except_error;
+              }
+            }
           }
           goto __pyx_L19_except_error;
           __pyx_L19_except_error:;
 
           /* "pyrfc/_cyrfc.pyx":2459
  *             free(cValue)
  *         elif typ == RFCTYPE_NUM:
@@ -31269,143 +31858,143 @@
  *             # cast to string prevents rounding errors in NWRFC SDK
  *             try:
  *                 if type(value) is float or type(value) is Decimal:             # <<<<<<<<<<<<<<
  *                     svalue = str(value)
  *                 else:
  */
             __pyx_t_5 = (((PyObject *)Py_TYPE(__pyx_v_value)) == ((PyObject *)(&PyFloat_Type)));
-            __pyx_t_20 = (__pyx_t_5 != 0);
-            if (!__pyx_t_20) {
+            __pyx_t_27 = (__pyx_t_5 != 0);
+            if (!__pyx_t_27) {
             } else {
-              __pyx_t_4 = __pyx_t_20;
-              goto __pyx_L33_bool_binop_done;
+              __pyx_t_4 = __pyx_t_27;
+              goto __pyx_L42_bool_binop_done;
             }
-            __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_Decimal); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 2471, __pyx_L26_error)
+            __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_Decimal); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 2471, __pyx_L35_error)
             __Pyx_GOTREF(__pyx_t_7);
-            __pyx_t_20 = (((PyObject *)Py_TYPE(__pyx_v_value)) == __pyx_t_7);
+            __pyx_t_27 = (((PyObject *)Py_TYPE(__pyx_v_value)) == __pyx_t_7);
             __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-            __pyx_t_5 = (__pyx_t_20 != 0);
+            __pyx_t_5 = (__pyx_t_27 != 0);
             __pyx_t_4 = __pyx_t_5;
-            __pyx_L33_bool_binop_done:;
+            __pyx_L42_bool_binop_done:;
             if (__pyx_t_4) {
 
               /* "pyrfc/_cyrfc.pyx":2472
  *             try:
  *                 if type(value) is float or type(value) is Decimal:
  *                     svalue = str(value)             # <<<<<<<<<<<<<<
  *                 else:
  *                     # string passed from application should be locale correct, do nothing
  */
-              __pyx_t_7 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyString_Type)), __pyx_v_value); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 2472, __pyx_L26_error)
+              __pyx_t_7 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyUnicode_Type)), __pyx_v_value); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 2472, __pyx_L35_error)
               __Pyx_GOTREF(__pyx_t_7);
               __pyx_v_svalue = __pyx_t_7;
               __pyx_t_7 = 0;
 
               /* "pyrfc/_cyrfc.pyx":2471
  *             # cast to string prevents rounding errors in NWRFC SDK
  *             try:
  *                 if type(value) is float or type(value) is Decimal:             # <<<<<<<<<<<<<<
  *                     svalue = str(value)
  *                 else:
  */
-              goto __pyx_L32;
+              goto __pyx_L41;
             }
 
             /* "pyrfc/_cyrfc.pyx":2475
  *                 else:
  *                     # string passed from application should be locale correct, do nothing
  *                     svalue = value             # <<<<<<<<<<<<<<
  *                 # decimal separator must be "." for the Decimal parsing check
  *                 locale_radix = _LOCALE_RADIX  # localeconv()['decimal_point']
  */
             /*else*/ {
               __Pyx_INCREF(__pyx_v_value);
               __pyx_v_svalue = __pyx_v_value;
             }
-            __pyx_L32:;
+            __pyx_L41:;
 
             /* "pyrfc/_cyrfc.pyx":2477
  *                     svalue = value
  *                 # decimal separator must be "." for the Decimal parsing check
  *                 locale_radix = _LOCALE_RADIX  # localeconv()['decimal_point']             # <<<<<<<<<<<<<<
  *                 if locale_radix != ".":
  *                     Decimal('.'.join(svalue.rsplit(locale_radix, 1)))
  */
-            __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_LOCALE_RADIX); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 2477, __pyx_L26_error)
+            __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_LOCALE_RADIX); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 2477, __pyx_L35_error)
             __Pyx_GOTREF(__pyx_t_7);
             __pyx_v_locale_radix = __pyx_t_7;
             __pyx_t_7 = 0;
 
             /* "pyrfc/_cyrfc.pyx":2478
  *                 # decimal separator must be "." for the Decimal parsing check
  *                 locale_radix = _LOCALE_RADIX  # localeconv()['decimal_point']
  *                 if locale_radix != ".":             # <<<<<<<<<<<<<<
  *                     Decimal('.'.join(svalue.rsplit(locale_radix, 1)))
  *                 else:
  */
-            __pyx_t_4 = (__Pyx_PyString_Equals(__pyx_v_locale_radix, __pyx_kp_s__20, Py_NE)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 2478, __pyx_L26_error)
+            __pyx_t_4 = (__Pyx_PyUnicode_Equals(__pyx_v_locale_radix, __pyx_kp_u__21, Py_NE)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 2478, __pyx_L35_error)
             if (__pyx_t_4) {
 
               /* "pyrfc/_cyrfc.pyx":2479
  *                 locale_radix = _LOCALE_RADIX  # localeconv()['decimal_point']
  *                 if locale_radix != ".":
  *                     Decimal('.'.join(svalue.rsplit(locale_radix, 1)))             # <<<<<<<<<<<<<<
  *                 else:
  *                     Decimal(svalue)
  */
-              __Pyx_GetModuleGlobalName(__pyx_t_11, __pyx_n_s_Decimal); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 2479, __pyx_L26_error)
+              __Pyx_GetModuleGlobalName(__pyx_t_11, __pyx_n_s_Decimal); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 2479, __pyx_L35_error)
               __Pyx_GOTREF(__pyx_t_11);
-              __pyx_t_19 = __Pyx_PyObject_GetAttrStr(__pyx_v_svalue, __pyx_n_s_rsplit); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 2479, __pyx_L26_error)
+              __pyx_t_19 = __Pyx_PyObject_GetAttrStr(__pyx_v_svalue, __pyx_n_s_rsplit); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 2479, __pyx_L35_error)
               __Pyx_GOTREF(__pyx_t_19);
               __pyx_t_18 = NULL;
-              __pyx_t_10 = 0;
+              __pyx_t_12 = 0;
               if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_19))) {
                 __pyx_t_18 = PyMethod_GET_SELF(__pyx_t_19);
                 if (likely(__pyx_t_18)) {
                   PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_19);
                   __Pyx_INCREF(__pyx_t_18);
                   __Pyx_INCREF(function);
                   __Pyx_DECREF_SET(__pyx_t_19, function);
-                  __pyx_t_10 = 1;
+                  __pyx_t_12 = 1;
                 }
               }
               #if CYTHON_FAST_PYCALL
               if (PyFunction_Check(__pyx_t_19)) {
                 PyObject *__pyx_temp[3] = {__pyx_t_18, __pyx_v_locale_radix, __pyx_int_1};
-                __pyx_t_6 = __Pyx_PyFunction_FastCall(__pyx_t_19, __pyx_temp+1-__pyx_t_10, 2+__pyx_t_10); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 2479, __pyx_L26_error)
+                __pyx_t_6 = __Pyx_PyFunction_FastCall(__pyx_t_19, __pyx_temp+1-__pyx_t_12, 2+__pyx_t_12); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 2479, __pyx_L35_error)
                 __Pyx_XDECREF(__pyx_t_18); __pyx_t_18 = 0;
                 __Pyx_GOTREF(__pyx_t_6);
               } else
               #endif
               #if CYTHON_FAST_PYCCALL
               if (__Pyx_PyFastCFunction_Check(__pyx_t_19)) {
                 PyObject *__pyx_temp[3] = {__pyx_t_18, __pyx_v_locale_radix, __pyx_int_1};
-                __pyx_t_6 = __Pyx_PyCFunction_FastCall(__pyx_t_19, __pyx_temp+1-__pyx_t_10, 2+__pyx_t_10); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 2479, __pyx_L26_error)
+                __pyx_t_6 = __Pyx_PyCFunction_FastCall(__pyx_t_19, __pyx_temp+1-__pyx_t_12, 2+__pyx_t_12); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 2479, __pyx_L35_error)
                 __Pyx_XDECREF(__pyx_t_18); __pyx_t_18 = 0;
                 __Pyx_GOTREF(__pyx_t_6);
               } else
               #endif
               {
-                __pyx_t_21 = PyTuple_New(2+__pyx_t_10); if (unlikely(!__pyx_t_21)) __PYX_ERR(0, 2479, __pyx_L26_error)
-                __Pyx_GOTREF(__pyx_t_21);
+                __pyx_t_28 = PyTuple_New(2+__pyx_t_12); if (unlikely(!__pyx_t_28)) __PYX_ERR(0, 2479, __pyx_L35_error)
+                __Pyx_GOTREF(__pyx_t_28);
                 if (__pyx_t_18) {
-                  __Pyx_GIVEREF(__pyx_t_18); PyTuple_SET_ITEM(__pyx_t_21, 0, __pyx_t_18); __pyx_t_18 = NULL;
+                  __Pyx_GIVEREF(__pyx_t_18); PyTuple_SET_ITEM(__pyx_t_28, 0, __pyx_t_18); __pyx_t_18 = NULL;
                 }
                 __Pyx_INCREF(__pyx_v_locale_radix);
                 __Pyx_GIVEREF(__pyx_v_locale_radix);
-                PyTuple_SET_ITEM(__pyx_t_21, 0+__pyx_t_10, __pyx_v_locale_radix);
+                PyTuple_SET_ITEM(__pyx_t_28, 0+__pyx_t_12, __pyx_v_locale_radix);
                 __Pyx_INCREF(__pyx_int_1);
                 __Pyx_GIVEREF(__pyx_int_1);
-                PyTuple_SET_ITEM(__pyx_t_21, 1+__pyx_t_10, __pyx_int_1);
-                __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_19, __pyx_t_21, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 2479, __pyx_L26_error)
+                PyTuple_SET_ITEM(__pyx_t_28, 1+__pyx_t_12, __pyx_int_1);
+                __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_19, __pyx_t_28, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 2479, __pyx_L35_error)
                 __Pyx_GOTREF(__pyx_t_6);
-                __Pyx_DECREF(__pyx_t_21); __pyx_t_21 = 0;
+                __Pyx_DECREF(__pyx_t_28); __pyx_t_28 = 0;
               }
               __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
-              __pyx_t_19 = __Pyx_PyString_Join(__pyx_kp_s__20, __pyx_t_6); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 2479, __pyx_L26_error)
+              __pyx_t_19 = PyUnicode_Join(__pyx_kp_u__21, __pyx_t_6); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 2479, __pyx_L35_error)
               __Pyx_GOTREF(__pyx_t_19);
               __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
               __pyx_t_6 = NULL;
               if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_11))) {
                 __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_11);
                 if (likely(__pyx_t_6)) {
                   PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_11);
@@ -31413,149 +32002,196 @@
                   __Pyx_INCREF(function);
                   __Pyx_DECREF_SET(__pyx_t_11, function);
                 }
               }
               __pyx_t_7 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_11, __pyx_t_6, __pyx_t_19) : __Pyx_PyObject_CallOneArg(__pyx_t_11, __pyx_t_19);
               __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
               __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
-              if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 2479, __pyx_L26_error)
+              if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 2479, __pyx_L35_error)
               __Pyx_GOTREF(__pyx_t_7);
               __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
               __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
               /* "pyrfc/_cyrfc.pyx":2478
  *                 # decimal separator must be "." for the Decimal parsing check
  *                 locale_radix = _LOCALE_RADIX  # localeconv()['decimal_point']
  *                 if locale_radix != ".":             # <<<<<<<<<<<<<<
  *                     Decimal('.'.join(svalue.rsplit(locale_radix, 1)))
  *                 else:
  */
-              goto __pyx_L35;
+              goto __pyx_L44;
             }
 
             /* "pyrfc/_cyrfc.pyx":2481
  *                     Decimal('.'.join(svalue.rsplit(locale_radix, 1)))
  *                 else:
  *                     Decimal(svalue)             # <<<<<<<<<<<<<<
  *                 cValue = fillString(svalue)
  *             except Exception as ex:
  */
             /*else*/ {
-              __Pyx_GetModuleGlobalName(__pyx_t_11, __pyx_n_s_Decimal); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 2481, __pyx_L26_error)
+              __Pyx_GetModuleGlobalName(__pyx_t_11, __pyx_n_s_Decimal); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 2481, __pyx_L35_error)
               __Pyx_GOTREF(__pyx_t_11);
               __pyx_t_19 = NULL;
               if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_11))) {
                 __pyx_t_19 = PyMethod_GET_SELF(__pyx_t_11);
                 if (likely(__pyx_t_19)) {
                   PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_11);
                   __Pyx_INCREF(__pyx_t_19);
                   __Pyx_INCREF(function);
                   __Pyx_DECREF_SET(__pyx_t_11, function);
                 }
               }
               __pyx_t_7 = (__pyx_t_19) ? __Pyx_PyObject_Call2Args(__pyx_t_11, __pyx_t_19, __pyx_v_svalue) : __Pyx_PyObject_CallOneArg(__pyx_t_11, __pyx_v_svalue);
               __Pyx_XDECREF(__pyx_t_19); __pyx_t_19 = 0;
-              if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 2481, __pyx_L26_error)
+              if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 2481, __pyx_L35_error)
               __Pyx_GOTREF(__pyx_t_7);
               __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
               __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
             }
-            __pyx_L35:;
+            __pyx_L44:;
 
             /* "pyrfc/_cyrfc.pyx":2482
  *                 else:
  *                     Decimal(svalue)
  *                 cValue = fillString(svalue)             # <<<<<<<<<<<<<<
  *             except Exception as ex:
  *                 raise TypeError('a decimal value required, received', value, 'of type', type(value))
  */
-            __pyx_t_14 = __pyx_f_5pyrfc_6_cyrfc_fillString(__pyx_v_svalue); if (unlikely(__pyx_t_14 == ((SAP_UC *)NULL))) __PYX_ERR(0, 2482, __pyx_L26_error)
+            __pyx_t_14 = __pyx_f_5pyrfc_6_cyrfc_fillString(__pyx_v_svalue); if (unlikely(__pyx_t_14 == ((SAP_UC *)NULL))) __PYX_ERR(0, 2482, __pyx_L35_error)
             __pyx_v_cValue = __pyx_t_14;
 
             /* "pyrfc/_cyrfc.pyx":2470
  *         elif typ == RFCTYPE_BCD or typ == RFCTYPE_FLOAT or typ == RFCTYPE_DECF16 or typ == RFCTYPE_DECF34:
  *             # cast to string prevents rounding errors in NWRFC SDK
  *             try:             # <<<<<<<<<<<<<<
  *                 if type(value) is float or type(value) is Decimal:
  *                     svalue = str(value)
  */
           }
           __Pyx_XDECREF(__pyx_t_17); __pyx_t_17 = 0;
           __Pyx_XDECREF(__pyx_t_16); __pyx_t_16 = 0;
           __Pyx_XDECREF(__pyx_t_15); __pyx_t_15 = 0;
-          goto __pyx_L31_try_end;
-          __pyx_L26_error:;
+          goto __pyx_L40_try_end;
+          __pyx_L35_error:;
           __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
           __Pyx_XDECREF(__pyx_t_18); __pyx_t_18 = 0;
           __Pyx_XDECREF(__pyx_t_19); __pyx_t_19 = 0;
-          __Pyx_XDECREF(__pyx_t_21); __pyx_t_21 = 0;
+          __Pyx_XDECREF(__pyx_t_28); __pyx_t_28 = 0;
           __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
           __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
 
           /* "pyrfc/_cyrfc.pyx":2483
  *                     Decimal(svalue)
  *                 cValue = fillString(svalue)
  *             except Exception as ex:             # <<<<<<<<<<<<<<
  *                 raise TypeError('a decimal value required, received', value, 'of type', type(value))
  *             rc = RfcSetString(container, cName, cValue, strlenU(cValue), &errorInfo)
  */
-          __pyx_t_10 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
-          if (__pyx_t_10) {
+          __pyx_t_12 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
+          if (__pyx_t_12) {
             __Pyx_AddTraceback("pyrfc._cyrfc.fillVariable", __pyx_clineno, __pyx_lineno, __pyx_filename);
-            if (__Pyx_GetException(&__pyx_t_7, &__pyx_t_11, &__pyx_t_19) < 0) __PYX_ERR(0, 2483, __pyx_L28_except_error)
+            if (__Pyx_GetException(&__pyx_t_7, &__pyx_t_11, &__pyx_t_19) < 0) __PYX_ERR(0, 2483, __pyx_L37_except_error)
             __Pyx_GOTREF(__pyx_t_7);
             __Pyx_GOTREF(__pyx_t_11);
             __Pyx_GOTREF(__pyx_t_19);
             __Pyx_INCREF(__pyx_t_11);
             __pyx_v_ex = __pyx_t_11;
+            /*try:*/ {
 
-            /* "pyrfc/_cyrfc.pyx":2484
+              /* "pyrfc/_cyrfc.pyx":2484
  *                 cValue = fillString(svalue)
  *             except Exception as ex:
  *                 raise TypeError('a decimal value required, received', value, 'of type', type(value))             # <<<<<<<<<<<<<<
  *             rc = RfcSetString(container, cName, cValue, strlenU(cValue), &errorInfo)
  *             free(cValue)
  */
-            __pyx_t_6 = PyTuple_New(4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 2484, __pyx_L28_except_error)
-            __Pyx_GOTREF(__pyx_t_6);
-            __Pyx_INCREF(__pyx_kp_s_a_decimal_value_required_receive);
-            __Pyx_GIVEREF(__pyx_kp_s_a_decimal_value_required_receive);
-            PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_kp_s_a_decimal_value_required_receive);
-            __Pyx_INCREF(__pyx_v_value);
-            __Pyx_GIVEREF(__pyx_v_value);
-            PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_v_value);
-            __Pyx_INCREF(__pyx_kp_s_of_type);
-            __Pyx_GIVEREF(__pyx_kp_s_of_type);
-            PyTuple_SET_ITEM(__pyx_t_6, 2, __pyx_kp_s_of_type);
-            __Pyx_INCREF(((PyObject *)Py_TYPE(__pyx_v_value)));
-            __Pyx_GIVEREF(((PyObject *)Py_TYPE(__pyx_v_value)));
-            PyTuple_SET_ITEM(__pyx_t_6, 3, ((PyObject *)Py_TYPE(__pyx_v_value)));
-            __pyx_t_21 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_t_6, NULL); if (unlikely(!__pyx_t_21)) __PYX_ERR(0, 2484, __pyx_L28_except_error)
-            __Pyx_GOTREF(__pyx_t_21);
-            __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-            __Pyx_Raise(__pyx_t_21, 0, 0, 0);
-            __Pyx_DECREF(__pyx_t_21); __pyx_t_21 = 0;
-            __PYX_ERR(0, 2484, __pyx_L28_except_error)
+              __pyx_t_6 = PyTuple_New(4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 2484, __pyx_L50_error)
+              __Pyx_GOTREF(__pyx_t_6);
+              __Pyx_INCREF(__pyx_kp_u_a_decimal_value_required_receive);
+              __Pyx_GIVEREF(__pyx_kp_u_a_decimal_value_required_receive);
+              PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_kp_u_a_decimal_value_required_receive);
+              __Pyx_INCREF(__pyx_v_value);
+              __Pyx_GIVEREF(__pyx_v_value);
+              PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_v_value);
+              __Pyx_INCREF(__pyx_kp_u_of_type);
+              __Pyx_GIVEREF(__pyx_kp_u_of_type);
+              PyTuple_SET_ITEM(__pyx_t_6, 2, __pyx_kp_u_of_type);
+              __Pyx_INCREF(((PyObject *)Py_TYPE(__pyx_v_value)));
+              __Pyx_GIVEREF(((PyObject *)Py_TYPE(__pyx_v_value)));
+              PyTuple_SET_ITEM(__pyx_t_6, 3, ((PyObject *)Py_TYPE(__pyx_v_value)));
+              __pyx_t_28 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_t_6, NULL); if (unlikely(!__pyx_t_28)) __PYX_ERR(0, 2484, __pyx_L50_error)
+              __Pyx_GOTREF(__pyx_t_28);
+              __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+              __Pyx_Raise(__pyx_t_28, 0, 0, 0);
+              __Pyx_DECREF(__pyx_t_28); __pyx_t_28 = 0;
+              __PYX_ERR(0, 2484, __pyx_L50_error)
+            }
+
+            /* "pyrfc/_cyrfc.pyx":2483
+ *                     Decimal(svalue)
+ *                 cValue = fillString(svalue)
+ *             except Exception as ex:             # <<<<<<<<<<<<<<
+ *                 raise TypeError('a decimal value required, received', value, 'of type', type(value))
+ *             rc = RfcSetString(container, cName, cValue, strlenU(cValue), &errorInfo)
+ */
+            /*finally:*/ {
+              __pyx_L50_error:;
+              /*exception exit:*/{
+                __Pyx_PyThreadState_declare
+                __Pyx_PyThreadState_assign
+                __pyx_t_26 = 0; __pyx_t_25 = 0; __pyx_t_24 = 0; __pyx_t_23 = 0; __pyx_t_22 = 0; __pyx_t_21 = 0;
+                __Pyx_XDECREF(__pyx_t_18); __pyx_t_18 = 0;
+                __Pyx_XDECREF(__pyx_t_28); __pyx_t_28 = 0;
+                __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+                if (PY_MAJOR_VERSION >= 3) __Pyx_ExceptionSwap(&__pyx_t_23, &__pyx_t_22, &__pyx_t_21);
+                if ((PY_MAJOR_VERSION < 3) || unlikely(__Pyx_GetException(&__pyx_t_26, &__pyx_t_25, &__pyx_t_24) < 0)) __Pyx_ErrFetch(&__pyx_t_26, &__pyx_t_25, &__pyx_t_24);
+                __Pyx_XGOTREF(__pyx_t_26);
+                __Pyx_XGOTREF(__pyx_t_25);
+                __Pyx_XGOTREF(__pyx_t_24);
+                __Pyx_XGOTREF(__pyx_t_23);
+                __Pyx_XGOTREF(__pyx_t_22);
+                __Pyx_XGOTREF(__pyx_t_21);
+                __pyx_t_12 = __pyx_lineno; __pyx_t_10 = __pyx_clineno; __pyx_t_29 = __pyx_filename;
+                {
+                  __Pyx_DECREF(__pyx_v_ex);
+                  __pyx_v_ex = NULL;
+                }
+                if (PY_MAJOR_VERSION >= 3) {
+                  __Pyx_XGIVEREF(__pyx_t_23);
+                  __Pyx_XGIVEREF(__pyx_t_22);
+                  __Pyx_XGIVEREF(__pyx_t_21);
+                  __Pyx_ExceptionReset(__pyx_t_23, __pyx_t_22, __pyx_t_21);
+                }
+                __Pyx_XGIVEREF(__pyx_t_26);
+                __Pyx_XGIVEREF(__pyx_t_25);
+                __Pyx_XGIVEREF(__pyx_t_24);
+                __Pyx_ErrRestore(__pyx_t_26, __pyx_t_25, __pyx_t_24);
+                __pyx_t_26 = 0; __pyx_t_25 = 0; __pyx_t_24 = 0; __pyx_t_23 = 0; __pyx_t_22 = 0; __pyx_t_21 = 0;
+                __pyx_lineno = __pyx_t_12; __pyx_clineno = __pyx_t_10; __pyx_filename = __pyx_t_29;
+                goto __pyx_L37_except_error;
+              }
+            }
           }
-          goto __pyx_L28_except_error;
-          __pyx_L28_except_error:;
+          goto __pyx_L37_except_error;
+          __pyx_L37_except_error:;
 
           /* "pyrfc/_cyrfc.pyx":2470
  *         elif typ == RFCTYPE_BCD or typ == RFCTYPE_FLOAT or typ == RFCTYPE_DECF16 or typ == RFCTYPE_DECF34:
  *             # cast to string prevents rounding errors in NWRFC SDK
  *             try:             # <<<<<<<<<<<<<<
  *                 if type(value) is float or type(value) is Decimal:
  *                     svalue = str(value)
  */
           __Pyx_XGIVEREF(__pyx_t_17);
           __Pyx_XGIVEREF(__pyx_t_16);
           __Pyx_XGIVEREF(__pyx_t_15);
           __Pyx_ExceptionReset(__pyx_t_17, __pyx_t_16, __pyx_t_15);
           goto __pyx_L3_error;
-          __pyx_L31_try_end:;
+          __pyx_L40_try_end:;
         }
 
         /* "pyrfc/_cyrfc.pyx":2485
  *             except Exception as ex:
  *                 raise TypeError('a decimal value required, received', value, 'of type', type(value))
  *             rc = RfcSetString(container, cName, cValue, strlenU(cValue), &errorInfo)             # <<<<<<<<<<<<<<
  *             free(cValue)
@@ -31608,23 +32244,23 @@
  *             if type(value) is not int:
  *                 raise TypeError('an integer required, received', value, 'of type', type(value))             # <<<<<<<<<<<<<<
  *             rc = RfcSetInt(container, cName, value, &errorInfo)
  *         elif typ == RFCTYPE_INT8:
  */
           __pyx_t_19 = PyTuple_New(4); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 2489, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_19);
-          __Pyx_INCREF(__pyx_kp_s_an_integer_required_received);
-          __Pyx_GIVEREF(__pyx_kp_s_an_integer_required_received);
-          PyTuple_SET_ITEM(__pyx_t_19, 0, __pyx_kp_s_an_integer_required_received);
+          __Pyx_INCREF(__pyx_kp_u_an_integer_required_received);
+          __Pyx_GIVEREF(__pyx_kp_u_an_integer_required_received);
+          PyTuple_SET_ITEM(__pyx_t_19, 0, __pyx_kp_u_an_integer_required_received);
           __Pyx_INCREF(__pyx_v_value);
           __Pyx_GIVEREF(__pyx_v_value);
           PyTuple_SET_ITEM(__pyx_t_19, 1, __pyx_v_value);
-          __Pyx_INCREF(__pyx_kp_s_of_type);
-          __Pyx_GIVEREF(__pyx_kp_s_of_type);
-          PyTuple_SET_ITEM(__pyx_t_19, 2, __pyx_kp_s_of_type);
+          __Pyx_INCREF(__pyx_kp_u_of_type);
+          __Pyx_GIVEREF(__pyx_kp_u_of_type);
+          PyTuple_SET_ITEM(__pyx_t_19, 2, __pyx_kp_u_of_type);
           __Pyx_INCREF(((PyObject *)Py_TYPE(__pyx_v_value)));
           __Pyx_GIVEREF(((PyObject *)Py_TYPE(__pyx_v_value)));
           PyTuple_SET_ITEM(__pyx_t_19, 3, ((PyObject *)Py_TYPE(__pyx_v_value)));
           __pyx_t_11 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_t_19, NULL); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 2489, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_11);
           __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
           __Pyx_Raise(__pyx_t_11, 0, 0, 0);
@@ -31643,16 +32279,16 @@
         /* "pyrfc/_cyrfc.pyx":2490
  *             if type(value) is not int:
  *                 raise TypeError('an integer required, received', value, 'of type', type(value))
  *             rc = RfcSetInt(container, cName, value, &errorInfo)             # <<<<<<<<<<<<<<
  *         elif typ == RFCTYPE_INT8:
  *             if type(value) is not int:
  */
-        __pyx_t_22 = __Pyx_PyInt_As_RFC_INT(__pyx_v_value); if (unlikely((__pyx_t_22 == ((RFC_INT)-1)) && PyErr_Occurred())) __PYX_ERR(0, 2490, __pyx_L3_error)
-        __pyx_v_rc = RfcSetInt(__pyx_v_container, __pyx_v_cName, __pyx_t_22, (&__pyx_v_errorInfo));
+        __pyx_t_30 = __Pyx_PyInt_As_RFC_INT(__pyx_v_value); if (unlikely((__pyx_t_30 == ((RFC_INT)-1)) && PyErr_Occurred())) __PYX_ERR(0, 2490, __pyx_L3_error)
+        __pyx_v_rc = RfcSetInt(__pyx_v_container, __pyx_v_cName, __pyx_t_30, (&__pyx_v_errorInfo));
 
         /* "pyrfc/_cyrfc.pyx":2487
  *             rc = RfcSetString(container, cName, cValue, strlenU(cValue), &errorInfo)
  *             free(cValue)
  *         elif typ in (RFCTYPE_INT, RFCTYPE_INT1, RFCTYPE_INT2):             # <<<<<<<<<<<<<<
  *             if type(value) is not int:
  *                 raise TypeError('an integer required, received', value, 'of type', type(value))
@@ -31676,23 +32312,23 @@
  *             if type(value) is not int:
  *                 raise TypeError('an integer required, received', value, 'of type', type(value))             # <<<<<<<<<<<<<<
  *             rc = RfcSetInt8(container, cName, value, &errorInfo)
  *         elif typ == RFCTYPE_UTCLONG:
  */
           __pyx_t_11 = PyTuple_New(4); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 2493, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_11);
-          __Pyx_INCREF(__pyx_kp_s_an_integer_required_received);
-          __Pyx_GIVEREF(__pyx_kp_s_an_integer_required_received);
-          PyTuple_SET_ITEM(__pyx_t_11, 0, __pyx_kp_s_an_integer_required_received);
+          __Pyx_INCREF(__pyx_kp_u_an_integer_required_received);
+          __Pyx_GIVEREF(__pyx_kp_u_an_integer_required_received);
+          PyTuple_SET_ITEM(__pyx_t_11, 0, __pyx_kp_u_an_integer_required_received);
           __Pyx_INCREF(__pyx_v_value);
           __Pyx_GIVEREF(__pyx_v_value);
           PyTuple_SET_ITEM(__pyx_t_11, 1, __pyx_v_value);
-          __Pyx_INCREF(__pyx_kp_s_of_type);
-          __Pyx_GIVEREF(__pyx_kp_s_of_type);
-          PyTuple_SET_ITEM(__pyx_t_11, 2, __pyx_kp_s_of_type);
+          __Pyx_INCREF(__pyx_kp_u_of_type);
+          __Pyx_GIVEREF(__pyx_kp_u_of_type);
+          PyTuple_SET_ITEM(__pyx_t_11, 2, __pyx_kp_u_of_type);
           __Pyx_INCREF(((PyObject *)Py_TYPE(__pyx_v_value)));
           __Pyx_GIVEREF(((PyObject *)Py_TYPE(__pyx_v_value)));
           PyTuple_SET_ITEM(__pyx_t_11, 3, ((PyObject *)Py_TYPE(__pyx_v_value)));
           __pyx_t_19 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_t_11, NULL); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 2493, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_19);
           __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
           __Pyx_Raise(__pyx_t_19, 0, 0, 0);
@@ -31711,16 +32347,16 @@
         /* "pyrfc/_cyrfc.pyx":2494
  *             if type(value) is not int:
  *                 raise TypeError('an integer required, received', value, 'of type', type(value))
  *             rc = RfcSetInt8(container, cName, value, &errorInfo)             # <<<<<<<<<<<<<<
  *         elif typ == RFCTYPE_UTCLONG:
  *             if type(value) is not str:
  */
-        __pyx_t_23 = __Pyx_PyInt_As_RFC_INT8(__pyx_v_value); if (unlikely((__pyx_t_23 == ((RFC_INT8)-1)) && PyErr_Occurred())) __PYX_ERR(0, 2494, __pyx_L3_error)
-        __pyx_v_rc = RfcSetInt8(__pyx_v_container, __pyx_v_cName, __pyx_t_23, (&__pyx_v_errorInfo));
+        __pyx_t_31 = __Pyx_PyInt_As_RFC_INT8(__pyx_v_value); if (unlikely((__pyx_t_31 == ((RFC_INT8)-1)) && PyErr_Occurred())) __PYX_ERR(0, 2494, __pyx_L3_error)
+        __pyx_v_rc = RfcSetInt8(__pyx_v_container, __pyx_v_cName, __pyx_t_31, (&__pyx_v_errorInfo));
 
         /* "pyrfc/_cyrfc.pyx":2491
  *                 raise TypeError('an integer required, received', value, 'of type', type(value))
  *             rc = RfcSetInt(container, cName, value, &errorInfo)
  *         elif typ == RFCTYPE_INT8:             # <<<<<<<<<<<<<<
  *             if type(value) is not int:
  *                 raise TypeError('an integer required, received', value, 'of type', type(value))
@@ -31731,36 +32367,36 @@
         /* "pyrfc/_cyrfc.pyx":2496
  *             rc = RfcSetInt8(container, cName, value, &errorInfo)
  *         elif typ == RFCTYPE_UTCLONG:
  *             if type(value) is not str:             # <<<<<<<<<<<<<<
  *                 raise TypeError('an string is required, received', value, 'of type', type(value))
  *             cValue = fillString(value)
  */
-        __pyx_t_4 = (((PyObject *)Py_TYPE(__pyx_v_value)) != ((PyObject *)(&PyString_Type)));
+        __pyx_t_4 = (((PyObject *)Py_TYPE(__pyx_v_value)) != ((PyObject *)(&PyUnicode_Type)));
         __pyx_t_5 = (__pyx_t_4 != 0);
         if (unlikely(__pyx_t_5)) {
 
           /* "pyrfc/_cyrfc.pyx":2497
  *         elif typ == RFCTYPE_UTCLONG:
  *             if type(value) is not str:
  *                 raise TypeError('an string is required, received', value, 'of type', type(value))             # <<<<<<<<<<<<<<
  *             cValue = fillString(value)
  *             rc = RfcSetString(container, cName, cValue, strlenU(cValue), &errorInfo)
  */
           __pyx_t_19 = PyTuple_New(4); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 2497, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_19);
-          __Pyx_INCREF(__pyx_kp_s_an_string_is_required_received);
-          __Pyx_GIVEREF(__pyx_kp_s_an_string_is_required_received);
-          PyTuple_SET_ITEM(__pyx_t_19, 0, __pyx_kp_s_an_string_is_required_received);
+          __Pyx_INCREF(__pyx_kp_u_an_string_is_required_received);
+          __Pyx_GIVEREF(__pyx_kp_u_an_string_is_required_received);
+          PyTuple_SET_ITEM(__pyx_t_19, 0, __pyx_kp_u_an_string_is_required_received);
           __Pyx_INCREF(__pyx_v_value);
           __Pyx_GIVEREF(__pyx_v_value);
           PyTuple_SET_ITEM(__pyx_t_19, 1, __pyx_v_value);
-          __Pyx_INCREF(__pyx_kp_s_of_type);
-          __Pyx_GIVEREF(__pyx_kp_s_of_type);
-          PyTuple_SET_ITEM(__pyx_t_19, 2, __pyx_kp_s_of_type);
+          __Pyx_INCREF(__pyx_kp_u_of_type);
+          __Pyx_GIVEREF(__pyx_kp_u_of_type);
+          PyTuple_SET_ITEM(__pyx_t_19, 2, __pyx_kp_u_of_type);
           __Pyx_INCREF(((PyObject *)Py_TYPE(__pyx_v_value)));
           __Pyx_GIVEREF(((PyObject *)Py_TYPE(__pyx_v_value)));
           PyTuple_SET_ITEM(__pyx_t_19, 3, ((PyObject *)Py_TYPE(__pyx_v_value)));
           __pyx_t_11 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_t_19, NULL); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 2497, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_11);
           __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
           __Pyx_Raise(__pyx_t_11, 0, 0, 0);
@@ -31853,60 +32489,60 @@
  *                     cValue = fillString(f'{value.year:04}{value.month:02}{value.day:02}')             # <<<<<<<<<<<<<<
  *                 else:
  *                     try:
  */
             __pyx_t_11 = PyTuple_New(3); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 2505, __pyx_L3_error)
             __Pyx_GOTREF(__pyx_t_11);
             __pyx_t_9 = 0;
-            __pyx_t_24 = 127;
+            __pyx_t_32 = 127;
             __pyx_t_19 = __Pyx_PyObject_GetAttrStr(__pyx_v_value, __pyx_n_s_year); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 2505, __pyx_L3_error)
             __Pyx_GOTREF(__pyx_t_19);
             __pyx_t_7 = __Pyx_PyObject_Format(__pyx_t_19, __pyx_kp_u_04); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 2505, __pyx_L3_error)
             __Pyx_GOTREF(__pyx_t_7);
             __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
-            __pyx_t_24 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_7) > __pyx_t_24) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_7) : __pyx_t_24;
+            __pyx_t_32 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_7) > __pyx_t_32) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_7) : __pyx_t_32;
             __pyx_t_9 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_7);
             __Pyx_GIVEREF(__pyx_t_7);
             PyTuple_SET_ITEM(__pyx_t_11, 0, __pyx_t_7);
             __pyx_t_7 = 0;
             __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_value, __pyx_n_s_month); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 2505, __pyx_L3_error)
             __Pyx_GOTREF(__pyx_t_7);
             __pyx_t_19 = __Pyx_PyObject_Format(__pyx_t_7, __pyx_kp_u_02); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 2505, __pyx_L3_error)
             __Pyx_GOTREF(__pyx_t_19);
             __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-            __pyx_t_24 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_19) > __pyx_t_24) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_19) : __pyx_t_24;
+            __pyx_t_32 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_19) > __pyx_t_32) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_19) : __pyx_t_32;
             __pyx_t_9 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_19);
             __Pyx_GIVEREF(__pyx_t_19);
             PyTuple_SET_ITEM(__pyx_t_11, 1, __pyx_t_19);
             __pyx_t_19 = 0;
             __pyx_t_19 = __Pyx_PyObject_GetAttrStr(__pyx_v_value, __pyx_n_s_day); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 2505, __pyx_L3_error)
             __Pyx_GOTREF(__pyx_t_19);
             __pyx_t_7 = __Pyx_PyObject_Format(__pyx_t_19, __pyx_kp_u_02); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 2505, __pyx_L3_error)
             __Pyx_GOTREF(__pyx_t_7);
             __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
-            __pyx_t_24 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_7) > __pyx_t_24) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_7) : __pyx_t_24;
+            __pyx_t_32 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_7) > __pyx_t_32) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_7) : __pyx_t_32;
             __pyx_t_9 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_7);
             __Pyx_GIVEREF(__pyx_t_7);
             PyTuple_SET_ITEM(__pyx_t_11, 2, __pyx_t_7);
             __pyx_t_7 = 0;
-            __pyx_t_7 = __Pyx_PyUnicode_Join(__pyx_t_11, 3, __pyx_t_9, __pyx_t_24); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 2505, __pyx_L3_error)
+            __pyx_t_7 = __Pyx_PyUnicode_Join(__pyx_t_11, 3, __pyx_t_9, __pyx_t_32); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 2505, __pyx_L3_error)
             __Pyx_GOTREF(__pyx_t_7);
             __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
             __pyx_t_14 = __pyx_f_5pyrfc_6_cyrfc_fillString(__pyx_t_7); if (unlikely(__pyx_t_14 == ((SAP_UC *)NULL))) __PYX_ERR(0, 2505, __pyx_L3_error)
             __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
             __pyx_v_cValue = __pyx_t_14;
 
             /* "pyrfc/_cyrfc.pyx":2504
  *             if value:
  *                 format_ok = True
  *                 if type(value) is date:             # <<<<<<<<<<<<<<
  *                     cValue = fillString(f'{value.year:04}{value.month:02}{value.day:02}')
  *                 else:
  */
-            goto __pyx_L42;
+            goto __pyx_L60;
           }
 
           /* "pyrfc/_cyrfc.pyx":2507
  *                     cValue = fillString(f'{value.year:04}{value.month:02}{value.day:02}')
  *                 else:
  *                     try:             # <<<<<<<<<<<<<<
  *                         if len(value) != 8:
@@ -31925,15 +32561,15 @@
                 /* "pyrfc/_cyrfc.pyx":2508
  *                 else:
  *                     try:
  *                         if len(value) != 8:             # <<<<<<<<<<<<<<
  *                             format_ok = False
  *                         else:
  */
-                __pyx_t_9 = PyObject_Length(__pyx_v_value); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1))) __PYX_ERR(0, 2508, __pyx_L43_error)
+                __pyx_t_9 = PyObject_Length(__pyx_v_value); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1))) __PYX_ERR(0, 2508, __pyx_L61_error)
                 __pyx_t_4 = ((__pyx_t_9 != 8) != 0);
                 if (__pyx_t_4) {
 
                   /* "pyrfc/_cyrfc.pyx":2509
  *                     try:
  *                         if len(value) != 8:
  *                             format_ok = False             # <<<<<<<<<<<<<<
@@ -31945,69 +32581,69 @@
                   /* "pyrfc/_cyrfc.pyx":2508
  *                 else:
  *                     try:
  *                         if len(value) != 8:             # <<<<<<<<<<<<<<
  *                             format_ok = False
  *                         else:
  */
-                  goto __pyx_L49;
+                  goto __pyx_L67;
                 }
 
                 /* "pyrfc/_cyrfc.pyx":2511
  *                             format_ok = False
  *                         else:
  *                             if len(value.rstrip()) > 0:             # <<<<<<<<<<<<<<
  *                                 date(int(value[:4]), int(value[4:6]), int(value[6:8]))
  *                             cValue = fillString(value)
  */
                 /*else*/ {
-                  __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_v_value, __pyx_n_s_rstrip); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 2511, __pyx_L43_error)
+                  __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_v_value, __pyx_n_s_rstrip); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 2511, __pyx_L61_error)
                   __Pyx_GOTREF(__pyx_t_11);
                   __pyx_t_19 = NULL;
                   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_11))) {
                     __pyx_t_19 = PyMethod_GET_SELF(__pyx_t_11);
                     if (likely(__pyx_t_19)) {
                       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_11);
                       __Pyx_INCREF(__pyx_t_19);
                       __Pyx_INCREF(function);
                       __Pyx_DECREF_SET(__pyx_t_11, function);
                     }
                   }
                   __pyx_t_7 = (__pyx_t_19) ? __Pyx_PyObject_CallOneArg(__pyx_t_11, __pyx_t_19) : __Pyx_PyObject_CallNoArg(__pyx_t_11);
                   __Pyx_XDECREF(__pyx_t_19); __pyx_t_19 = 0;
-                  if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 2511, __pyx_L43_error)
+                  if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 2511, __pyx_L61_error)
                   __Pyx_GOTREF(__pyx_t_7);
                   __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-                  __pyx_t_9 = PyObject_Length(__pyx_t_7); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1))) __PYX_ERR(0, 2511, __pyx_L43_error)
+                  __pyx_t_9 = PyObject_Length(__pyx_t_7); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1))) __PYX_ERR(0, 2511, __pyx_L61_error)
                   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
                   __pyx_t_4 = ((__pyx_t_9 > 0) != 0);
                   if (__pyx_t_4) {
 
                     /* "pyrfc/_cyrfc.pyx":2512
  *                         else:
  *                             if len(value.rstrip()) > 0:
  *                                 date(int(value[:4]), int(value[4:6]), int(value[6:8]))             # <<<<<<<<<<<<<<
  *                             cValue = fillString(value)
  *                     except Exception as ex:
  */
-                    __Pyx_GetModuleGlobalName(__pyx_t_11, __pyx_n_s_date); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 2512, __pyx_L43_error)
+                    __Pyx_GetModuleGlobalName(__pyx_t_11, __pyx_n_s_date); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 2512, __pyx_L61_error)
                     __Pyx_GOTREF(__pyx_t_11);
-                    __pyx_t_19 = __Pyx_PyObject_GetSlice(__pyx_v_value, 0, 4, NULL, NULL, &__pyx_slice__37, 0, 1, 1); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 2512, __pyx_L43_error)
+                    __pyx_t_19 = __Pyx_PyObject_GetSlice(__pyx_v_value, 0, 4, NULL, NULL, &__pyx_slice__38, 0, 1, 1); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 2512, __pyx_L61_error)
                     __Pyx_GOTREF(__pyx_t_19);
-                    __pyx_t_21 = __Pyx_PyNumber_Int(__pyx_t_19); if (unlikely(!__pyx_t_21)) __PYX_ERR(0, 2512, __pyx_L43_error)
-                    __Pyx_GOTREF(__pyx_t_21);
+                    __pyx_t_28 = __Pyx_PyNumber_Int(__pyx_t_19); if (unlikely(!__pyx_t_28)) __PYX_ERR(0, 2512, __pyx_L61_error)
+                    __Pyx_GOTREF(__pyx_t_28);
                     __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
-                    __pyx_t_19 = __Pyx_PyObject_GetSlice(__pyx_v_value, 4, 6, NULL, NULL, &__pyx_slice__38, 1, 1, 1); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 2512, __pyx_L43_error)
+                    __pyx_t_19 = __Pyx_PyObject_GetSlice(__pyx_v_value, 4, 6, NULL, NULL, &__pyx_slice__39, 1, 1, 1); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 2512, __pyx_L61_error)
                     __Pyx_GOTREF(__pyx_t_19);
-                    __pyx_t_6 = __Pyx_PyNumber_Int(__pyx_t_19); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 2512, __pyx_L43_error)
+                    __pyx_t_6 = __Pyx_PyNumber_Int(__pyx_t_19); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 2512, __pyx_L61_error)
                     __Pyx_GOTREF(__pyx_t_6);
                     __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
-                    __pyx_t_19 = __Pyx_PyObject_GetSlice(__pyx_v_value, 6, 8, NULL, NULL, &__pyx_slice__39, 1, 1, 1); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 2512, __pyx_L43_error)
+                    __pyx_t_19 = __Pyx_PyObject_GetSlice(__pyx_v_value, 6, 8, NULL, NULL, &__pyx_slice__40, 1, 1, 1); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 2512, __pyx_L61_error)
                     __Pyx_GOTREF(__pyx_t_19);
-                    __pyx_t_18 = __Pyx_PyNumber_Int(__pyx_t_19); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 2512, __pyx_L43_error)
+                    __pyx_t_18 = __Pyx_PyNumber_Int(__pyx_t_19); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 2512, __pyx_L61_error)
                     __Pyx_GOTREF(__pyx_t_18);
                     __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
                     __pyx_t_19 = NULL;
                     __pyx_t_10 = 0;
                     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_11))) {
                       __pyx_t_19 = PyMethod_GET_SELF(__pyx_t_11);
                       if (likely(__pyx_t_19)) {
@@ -32016,52 +32652,52 @@
                         __Pyx_INCREF(function);
                         __Pyx_DECREF_SET(__pyx_t_11, function);
                         __pyx_t_10 = 1;
                       }
                     }
                     #if CYTHON_FAST_PYCALL
                     if (PyFunction_Check(__pyx_t_11)) {
-                      PyObject *__pyx_temp[4] = {__pyx_t_19, __pyx_t_21, __pyx_t_6, __pyx_t_18};
-                      __pyx_t_7 = __Pyx_PyFunction_FastCall(__pyx_t_11, __pyx_temp+1-__pyx_t_10, 3+__pyx_t_10); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 2512, __pyx_L43_error)
+                      PyObject *__pyx_temp[4] = {__pyx_t_19, __pyx_t_28, __pyx_t_6, __pyx_t_18};
+                      __pyx_t_7 = __Pyx_PyFunction_FastCall(__pyx_t_11, __pyx_temp+1-__pyx_t_10, 3+__pyx_t_10); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 2512, __pyx_L61_error)
                       __Pyx_XDECREF(__pyx_t_19); __pyx_t_19 = 0;
                       __Pyx_GOTREF(__pyx_t_7);
-                      __Pyx_DECREF(__pyx_t_21); __pyx_t_21 = 0;
+                      __Pyx_DECREF(__pyx_t_28); __pyx_t_28 = 0;
                       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
                       __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
                     } else
                     #endif
                     #if CYTHON_FAST_PYCCALL
                     if (__Pyx_PyFastCFunction_Check(__pyx_t_11)) {
-                      PyObject *__pyx_temp[4] = {__pyx_t_19, __pyx_t_21, __pyx_t_6, __pyx_t_18};
-                      __pyx_t_7 = __Pyx_PyCFunction_FastCall(__pyx_t_11, __pyx_temp+1-__pyx_t_10, 3+__pyx_t_10); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 2512, __pyx_L43_error)
+                      PyObject *__pyx_temp[4] = {__pyx_t_19, __pyx_t_28, __pyx_t_6, __pyx_t_18};
+                      __pyx_t_7 = __Pyx_PyCFunction_FastCall(__pyx_t_11, __pyx_temp+1-__pyx_t_10, 3+__pyx_t_10); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 2512, __pyx_L61_error)
                       __Pyx_XDECREF(__pyx_t_19); __pyx_t_19 = 0;
                       __Pyx_GOTREF(__pyx_t_7);
-                      __Pyx_DECREF(__pyx_t_21); __pyx_t_21 = 0;
+                      __Pyx_DECREF(__pyx_t_28); __pyx_t_28 = 0;
                       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
                       __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
                     } else
                     #endif
                     {
-                      __pyx_t_25 = PyTuple_New(3+__pyx_t_10); if (unlikely(!__pyx_t_25)) __PYX_ERR(0, 2512, __pyx_L43_error)
-                      __Pyx_GOTREF(__pyx_t_25);
+                      __pyx_t_33 = PyTuple_New(3+__pyx_t_10); if (unlikely(!__pyx_t_33)) __PYX_ERR(0, 2512, __pyx_L61_error)
+                      __Pyx_GOTREF(__pyx_t_33);
                       if (__pyx_t_19) {
-                        __Pyx_GIVEREF(__pyx_t_19); PyTuple_SET_ITEM(__pyx_t_25, 0, __pyx_t_19); __pyx_t_19 = NULL;
+                        __Pyx_GIVEREF(__pyx_t_19); PyTuple_SET_ITEM(__pyx_t_33, 0, __pyx_t_19); __pyx_t_19 = NULL;
                       }
-                      __Pyx_GIVEREF(__pyx_t_21);
-                      PyTuple_SET_ITEM(__pyx_t_25, 0+__pyx_t_10, __pyx_t_21);
+                      __Pyx_GIVEREF(__pyx_t_28);
+                      PyTuple_SET_ITEM(__pyx_t_33, 0+__pyx_t_10, __pyx_t_28);
                       __Pyx_GIVEREF(__pyx_t_6);
-                      PyTuple_SET_ITEM(__pyx_t_25, 1+__pyx_t_10, __pyx_t_6);
+                      PyTuple_SET_ITEM(__pyx_t_33, 1+__pyx_t_10, __pyx_t_6);
                       __Pyx_GIVEREF(__pyx_t_18);
-                      PyTuple_SET_ITEM(__pyx_t_25, 2+__pyx_t_10, __pyx_t_18);
-                      __pyx_t_21 = 0;
+                      PyTuple_SET_ITEM(__pyx_t_33, 2+__pyx_t_10, __pyx_t_18);
+                      __pyx_t_28 = 0;
                       __pyx_t_6 = 0;
                       __pyx_t_18 = 0;
-                      __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_11, __pyx_t_25, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 2512, __pyx_L43_error)
+                      __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_11, __pyx_t_33, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 2512, __pyx_L61_error)
                       __Pyx_GOTREF(__pyx_t_7);
-                      __Pyx_DECREF(__pyx_t_25); __pyx_t_25 = 0;
+                      __Pyx_DECREF(__pyx_t_33); __pyx_t_33 = 0;
                     }
                     __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
                     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
                     /* "pyrfc/_cyrfc.pyx":2511
  *                             format_ok = False
  *                         else:
@@ -32074,94 +32710,112 @@
                   /* "pyrfc/_cyrfc.pyx":2513
  *                             if len(value.rstrip()) > 0:
  *                                 date(int(value[:4]), int(value[4:6]), int(value[6:8]))
  *                             cValue = fillString(value)             # <<<<<<<<<<<<<<
  *                     except Exception as ex:
  *                         format_ok = False
  */
-                  __pyx_t_14 = __pyx_f_5pyrfc_6_cyrfc_fillString(__pyx_v_value); if (unlikely(__pyx_t_14 == ((SAP_UC *)NULL))) __PYX_ERR(0, 2513, __pyx_L43_error)
+                  __pyx_t_14 = __pyx_f_5pyrfc_6_cyrfc_fillString(__pyx_v_value); if (unlikely(__pyx_t_14 == ((SAP_UC *)NULL))) __PYX_ERR(0, 2513, __pyx_L61_error)
                   __pyx_v_cValue = __pyx_t_14;
                 }
-                __pyx_L49:;
+                __pyx_L67:;
 
                 /* "pyrfc/_cyrfc.pyx":2507
  *                     cValue = fillString(f'{value.year:04}{value.month:02}{value.day:02}')
  *                 else:
  *                     try:             # <<<<<<<<<<<<<<
  *                         if len(value) != 8:
  *                             format_ok = False
  */
               }
               __Pyx_XDECREF(__pyx_t_15); __pyx_t_15 = 0;
               __Pyx_XDECREF(__pyx_t_16); __pyx_t_16 = 0;
               __Pyx_XDECREF(__pyx_t_17); __pyx_t_17 = 0;
-              goto __pyx_L48_try_end;
-              __pyx_L43_error:;
+              goto __pyx_L66_try_end;
+              __pyx_L61_error:;
               __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
               __Pyx_XDECREF(__pyx_t_18); __pyx_t_18 = 0;
               __Pyx_XDECREF(__pyx_t_19); __pyx_t_19 = 0;
-              __Pyx_XDECREF(__pyx_t_21); __pyx_t_21 = 0;
-              __Pyx_XDECREF(__pyx_t_25); __pyx_t_25 = 0;
+              __Pyx_XDECREF(__pyx_t_28); __pyx_t_28 = 0;
+              __Pyx_XDECREF(__pyx_t_33); __pyx_t_33 = 0;
               __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
               __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
 
               /* "pyrfc/_cyrfc.pyx":2514
  *                                 date(int(value[:4]), int(value[4:6]), int(value[6:8]))
  *                             cValue = fillString(value)
  *                     except Exception as ex:             # <<<<<<<<<<<<<<
  *                         format_ok = False
  *                 if not format_ok:
  */
               __pyx_t_10 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
               if (__pyx_t_10) {
                 __Pyx_AddTraceback("pyrfc._cyrfc.fillVariable", __pyx_clineno, __pyx_lineno, __pyx_filename);
-                if (__Pyx_GetException(&__pyx_t_7, &__pyx_t_11, &__pyx_t_25) < 0) __PYX_ERR(0, 2514, __pyx_L45_except_error)
+                if (__Pyx_GetException(&__pyx_t_7, &__pyx_t_11, &__pyx_t_33) < 0) __PYX_ERR(0, 2514, __pyx_L63_except_error)
                 __Pyx_GOTREF(__pyx_t_7);
                 __Pyx_GOTREF(__pyx_t_11);
-                __Pyx_GOTREF(__pyx_t_25);
+                __Pyx_GOTREF(__pyx_t_33);
                 __Pyx_INCREF(__pyx_t_11);
                 __pyx_v_ex = __pyx_t_11;
+                /*try:*/ {
 
-                /* "pyrfc/_cyrfc.pyx":2515
+                  /* "pyrfc/_cyrfc.pyx":2515
  *                             cValue = fillString(value)
  *                     except Exception as ex:
  *                         format_ok = False             # <<<<<<<<<<<<<<
  *                 if not format_ok:
  *                     raise TypeError('date value required, received', value, 'of type', type(value))
  */
-                __pyx_v_format_ok = 0;
+                  __pyx_v_format_ok = 0;
+                }
+
+                /* "pyrfc/_cyrfc.pyx":2514
+ *                                 date(int(value[:4]), int(value[4:6]), int(value[6:8]))
+ *                             cValue = fillString(value)
+ *                     except Exception as ex:             # <<<<<<<<<<<<<<
+ *                         format_ok = False
+ *                 if not format_ok:
+ */
+                /*finally:*/ {
+                  /*normal exit:*/{
+                    __Pyx_DECREF(__pyx_v_ex);
+                    __pyx_v_ex = NULL;
+                    goto __pyx_L75;
+                  }
+                  __pyx_L75:;
+                }
                 __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
                 __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
-                __Pyx_XDECREF(__pyx_t_25); __pyx_t_25 = 0;
-                goto __pyx_L44_exception_handled;
+                __Pyx_XDECREF(__pyx_t_33); __pyx_t_33 = 0;
+                goto __pyx_L62_exception_handled;
               }
-              goto __pyx_L45_except_error;
-              __pyx_L45_except_error:;
+              goto __pyx_L63_except_error;
+              __pyx_L63_except_error:;
 
               /* "pyrfc/_cyrfc.pyx":2507
  *                     cValue = fillString(f'{value.year:04}{value.month:02}{value.day:02}')
  *                 else:
  *                     try:             # <<<<<<<<<<<<<<
  *                         if len(value) != 8:
  *                             format_ok = False
  */
               __Pyx_XGIVEREF(__pyx_t_15);
               __Pyx_XGIVEREF(__pyx_t_16);
               __Pyx_XGIVEREF(__pyx_t_17);
               __Pyx_ExceptionReset(__pyx_t_15, __pyx_t_16, __pyx_t_17);
               goto __pyx_L3_error;
-              __pyx_L44_exception_handled:;
+              __pyx_L62_exception_handled:;
               __Pyx_XGIVEREF(__pyx_t_15);
               __Pyx_XGIVEREF(__pyx_t_16);
               __Pyx_XGIVEREF(__pyx_t_17);
               __Pyx_ExceptionReset(__pyx_t_15, __pyx_t_16, __pyx_t_17);
-              __pyx_L48_try_end:;
+              __pyx_L66_try_end:;
             }
           }
-          __pyx_L42:;
+          __pyx_L60:;
 
           /* "pyrfc/_cyrfc.pyx":2516
  *                     except Exception as ex:
  *                         format_ok = False
  *                 if not format_ok:             # <<<<<<<<<<<<<<
  *                     raise TypeError('date value required, received', value, 'of type', type(value))
  *                 rc = RfcSetDate(container, cName, cValue, &errorInfo)
@@ -32172,31 +32826,31 @@
             /* "pyrfc/_cyrfc.pyx":2517
  *                         format_ok = False
  *                 if not format_ok:
  *                     raise TypeError('date value required, received', value, 'of type', type(value))             # <<<<<<<<<<<<<<
  *                 rc = RfcSetDate(container, cName, cValue, &errorInfo)
  *                 free(cValue)
  */
-            __pyx_t_25 = PyTuple_New(4); if (unlikely(!__pyx_t_25)) __PYX_ERR(0, 2517, __pyx_L3_error)
-            __Pyx_GOTREF(__pyx_t_25);
-            __Pyx_INCREF(__pyx_kp_s_date_value_required_received);
-            __Pyx_GIVEREF(__pyx_kp_s_date_value_required_received);
-            PyTuple_SET_ITEM(__pyx_t_25, 0, __pyx_kp_s_date_value_required_received);
+            __pyx_t_33 = PyTuple_New(4); if (unlikely(!__pyx_t_33)) __PYX_ERR(0, 2517, __pyx_L3_error)
+            __Pyx_GOTREF(__pyx_t_33);
+            __Pyx_INCREF(__pyx_kp_u_date_value_required_received);
+            __Pyx_GIVEREF(__pyx_kp_u_date_value_required_received);
+            PyTuple_SET_ITEM(__pyx_t_33, 0, __pyx_kp_u_date_value_required_received);
             __Pyx_INCREF(__pyx_v_value);
             __Pyx_GIVEREF(__pyx_v_value);
-            PyTuple_SET_ITEM(__pyx_t_25, 1, __pyx_v_value);
-            __Pyx_INCREF(__pyx_kp_s_of_type);
-            __Pyx_GIVEREF(__pyx_kp_s_of_type);
-            PyTuple_SET_ITEM(__pyx_t_25, 2, __pyx_kp_s_of_type);
+            PyTuple_SET_ITEM(__pyx_t_33, 1, __pyx_v_value);
+            __Pyx_INCREF(__pyx_kp_u_of_type);
+            __Pyx_GIVEREF(__pyx_kp_u_of_type);
+            PyTuple_SET_ITEM(__pyx_t_33, 2, __pyx_kp_u_of_type);
             __Pyx_INCREF(((PyObject *)Py_TYPE(__pyx_v_value)));
             __Pyx_GIVEREF(((PyObject *)Py_TYPE(__pyx_v_value)));
-            PyTuple_SET_ITEM(__pyx_t_25, 3, ((PyObject *)Py_TYPE(__pyx_v_value)));
-            __pyx_t_11 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_t_25, NULL); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 2517, __pyx_L3_error)
+            PyTuple_SET_ITEM(__pyx_t_33, 3, ((PyObject *)Py_TYPE(__pyx_v_value)));
+            __pyx_t_11 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_t_33, NULL); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 2517, __pyx_L3_error)
             __Pyx_GOTREF(__pyx_t_11);
-            __Pyx_DECREF(__pyx_t_25); __pyx_t_25 = 0;
+            __Pyx_DECREF(__pyx_t_33); __pyx_t_33 = 0;
             __Pyx_Raise(__pyx_t_11, 0, 0, 0);
             __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
             __PYX_ERR(0, 2517, __pyx_L3_error)
 
             /* "pyrfc/_cyrfc.pyx":2516
  *                     except Exception as ex:
  *                         format_ok = False
@@ -32227,28 +32881,28 @@
           /* "pyrfc/_cyrfc.pyx":2502
  *             free(cValue)
  *         elif typ == RFCTYPE_DATE:
  *             if value:             # <<<<<<<<<<<<<<
  *                 format_ok = True
  *                 if type(value) is date:
  */
-          goto __pyx_L41;
+          goto __pyx_L59;
         }
 
         /* "pyrfc/_cyrfc.pyx":2521
  *                 free(cValue)
  *             else:
  *                 rc = RFC_OK             # <<<<<<<<<<<<<<
  *         elif typ == RFCTYPE_TIME:
  *             if value:
  */
         /*else*/ {
           __pyx_v_rc = RFC_OK;
         }
-        __pyx_L41:;
+        __pyx_L59:;
 
         /* "pyrfc/_cyrfc.pyx":2501
  *             rc = RfcSetString(container, cName, cValue, strlenU(cValue), &errorInfo)
  *             free(cValue)
  *         elif typ == RFCTYPE_DATE:             # <<<<<<<<<<<<<<
  *             if value:
  *                 format_ok = True
@@ -32295,60 +32949,60 @@
  *                     cValue = fillString(f'{value.hour:02}{value.minute:02}{value.second:02}')             # <<<<<<<<<<<<<<
  *                 else:
  *                     try:
  */
             __pyx_t_11 = PyTuple_New(3); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 2526, __pyx_L3_error)
             __Pyx_GOTREF(__pyx_t_11);
             __pyx_t_9 = 0;
-            __pyx_t_24 = 127;
-            __pyx_t_25 = __Pyx_PyObject_GetAttrStr(__pyx_v_value, __pyx_n_s_hour); if (unlikely(!__pyx_t_25)) __PYX_ERR(0, 2526, __pyx_L3_error)
-            __Pyx_GOTREF(__pyx_t_25);
-            __pyx_t_7 = __Pyx_PyObject_Format(__pyx_t_25, __pyx_kp_u_02); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 2526, __pyx_L3_error)
+            __pyx_t_32 = 127;
+            __pyx_t_33 = __Pyx_PyObject_GetAttrStr(__pyx_v_value, __pyx_n_s_hour); if (unlikely(!__pyx_t_33)) __PYX_ERR(0, 2526, __pyx_L3_error)
+            __Pyx_GOTREF(__pyx_t_33);
+            __pyx_t_7 = __Pyx_PyObject_Format(__pyx_t_33, __pyx_kp_u_02); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 2526, __pyx_L3_error)
             __Pyx_GOTREF(__pyx_t_7);
-            __Pyx_DECREF(__pyx_t_25); __pyx_t_25 = 0;
-            __pyx_t_24 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_7) > __pyx_t_24) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_7) : __pyx_t_24;
+            __Pyx_DECREF(__pyx_t_33); __pyx_t_33 = 0;
+            __pyx_t_32 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_7) > __pyx_t_32) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_7) : __pyx_t_32;
             __pyx_t_9 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_7);
             __Pyx_GIVEREF(__pyx_t_7);
             PyTuple_SET_ITEM(__pyx_t_11, 0, __pyx_t_7);
             __pyx_t_7 = 0;
             __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_value, __pyx_n_s_minute); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 2526, __pyx_L3_error)
             __Pyx_GOTREF(__pyx_t_7);
-            __pyx_t_25 = __Pyx_PyObject_Format(__pyx_t_7, __pyx_kp_u_02); if (unlikely(!__pyx_t_25)) __PYX_ERR(0, 2526, __pyx_L3_error)
-            __Pyx_GOTREF(__pyx_t_25);
+            __pyx_t_33 = __Pyx_PyObject_Format(__pyx_t_7, __pyx_kp_u_02); if (unlikely(!__pyx_t_33)) __PYX_ERR(0, 2526, __pyx_L3_error)
+            __Pyx_GOTREF(__pyx_t_33);
             __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-            __pyx_t_24 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_25) > __pyx_t_24) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_25) : __pyx_t_24;
-            __pyx_t_9 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_25);
-            __Pyx_GIVEREF(__pyx_t_25);
-            PyTuple_SET_ITEM(__pyx_t_11, 1, __pyx_t_25);
-            __pyx_t_25 = 0;
-            __pyx_t_25 = __Pyx_PyObject_GetAttrStr(__pyx_v_value, __pyx_n_s_second); if (unlikely(!__pyx_t_25)) __PYX_ERR(0, 2526, __pyx_L3_error)
-            __Pyx_GOTREF(__pyx_t_25);
-            __pyx_t_7 = __Pyx_PyObject_Format(__pyx_t_25, __pyx_kp_u_02); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 2526, __pyx_L3_error)
+            __pyx_t_32 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_33) > __pyx_t_32) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_33) : __pyx_t_32;
+            __pyx_t_9 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_33);
+            __Pyx_GIVEREF(__pyx_t_33);
+            PyTuple_SET_ITEM(__pyx_t_11, 1, __pyx_t_33);
+            __pyx_t_33 = 0;
+            __pyx_t_33 = __Pyx_PyObject_GetAttrStr(__pyx_v_value, __pyx_n_s_second); if (unlikely(!__pyx_t_33)) __PYX_ERR(0, 2526, __pyx_L3_error)
+            __Pyx_GOTREF(__pyx_t_33);
+            __pyx_t_7 = __Pyx_PyObject_Format(__pyx_t_33, __pyx_kp_u_02); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 2526, __pyx_L3_error)
             __Pyx_GOTREF(__pyx_t_7);
-            __Pyx_DECREF(__pyx_t_25); __pyx_t_25 = 0;
-            __pyx_t_24 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_7) > __pyx_t_24) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_7) : __pyx_t_24;
+            __Pyx_DECREF(__pyx_t_33); __pyx_t_33 = 0;
+            __pyx_t_32 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_7) > __pyx_t_32) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_7) : __pyx_t_32;
             __pyx_t_9 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_7);
             __Pyx_GIVEREF(__pyx_t_7);
             PyTuple_SET_ITEM(__pyx_t_11, 2, __pyx_t_7);
             __pyx_t_7 = 0;
-            __pyx_t_7 = __Pyx_PyUnicode_Join(__pyx_t_11, 3, __pyx_t_9, __pyx_t_24); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 2526, __pyx_L3_error)
+            __pyx_t_7 = __Pyx_PyUnicode_Join(__pyx_t_11, 3, __pyx_t_9, __pyx_t_32); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 2526, __pyx_L3_error)
             __Pyx_GOTREF(__pyx_t_7);
             __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
             __pyx_t_14 = __pyx_f_5pyrfc_6_cyrfc_fillString(__pyx_t_7); if (unlikely(__pyx_t_14 == ((SAP_UC *)NULL))) __PYX_ERR(0, 2526, __pyx_L3_error)
             __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
             __pyx_v_cValue = __pyx_t_14;
 
             /* "pyrfc/_cyrfc.pyx":2525
  *             if value:
  *                 format_ok = True
  *                 if type(value) is time:             # <<<<<<<<<<<<<<
  *                     cValue = fillString(f'{value.hour:02}{value.minute:02}{value.second:02}')
  *                 else:
  */
-            goto __pyx_L55;
+            goto __pyx_L78;
           }
 
           /* "pyrfc/_cyrfc.pyx":2528
  *                     cValue = fillString(f'{value.hour:02}{value.minute:02}{value.second:02}')
  *                 else:
  *                     try:             # <<<<<<<<<<<<<<
  *                         if len(value) != 6:
@@ -32367,15 +33021,15 @@
                 /* "pyrfc/_cyrfc.pyx":2529
  *                 else:
  *                     try:
  *                         if len(value) != 6:             # <<<<<<<<<<<<<<
  *                             format_ok = False
  *                         else:
  */
-                __pyx_t_9 = PyObject_Length(__pyx_v_value); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1))) __PYX_ERR(0, 2529, __pyx_L56_error)
+                __pyx_t_9 = PyObject_Length(__pyx_v_value); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1))) __PYX_ERR(0, 2529, __pyx_L79_error)
                 __pyx_t_5 = ((__pyx_t_9 != 6) != 0);
                 if (__pyx_t_5) {
 
                   /* "pyrfc/_cyrfc.pyx":2530
  *                     try:
  *                         if len(value) != 6:
  *                             format_ok = False             # <<<<<<<<<<<<<<
@@ -32387,121 +33041,121 @@
                   /* "pyrfc/_cyrfc.pyx":2529
  *                 else:
  *                     try:
  *                         if len(value) != 6:             # <<<<<<<<<<<<<<
  *                             format_ok = False
  *                         else:
  */
-                  goto __pyx_L62;
+                  goto __pyx_L85;
                 }
 
                 /* "pyrfc/_cyrfc.pyx":2532
  *                             format_ok = False
  *                         else:
  *                             if len(value.rstrip()) > 0:             # <<<<<<<<<<<<<<
  *                                 time(int(value[:2]), int(value[2:4]), int(value[4:6]))
  *                             cValue = fillString(value)
  */
                 /*else*/ {
-                  __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_v_value, __pyx_n_s_rstrip); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 2532, __pyx_L56_error)
+                  __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_v_value, __pyx_n_s_rstrip); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 2532, __pyx_L79_error)
                   __Pyx_GOTREF(__pyx_t_11);
-                  __pyx_t_25 = NULL;
+                  __pyx_t_33 = NULL;
                   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_11))) {
-                    __pyx_t_25 = PyMethod_GET_SELF(__pyx_t_11);
-                    if (likely(__pyx_t_25)) {
+                    __pyx_t_33 = PyMethod_GET_SELF(__pyx_t_11);
+                    if (likely(__pyx_t_33)) {
                       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_11);
-                      __Pyx_INCREF(__pyx_t_25);
+                      __Pyx_INCREF(__pyx_t_33);
                       __Pyx_INCREF(function);
                       __Pyx_DECREF_SET(__pyx_t_11, function);
                     }
                   }
-                  __pyx_t_7 = (__pyx_t_25) ? __Pyx_PyObject_CallOneArg(__pyx_t_11, __pyx_t_25) : __Pyx_PyObject_CallNoArg(__pyx_t_11);
-                  __Pyx_XDECREF(__pyx_t_25); __pyx_t_25 = 0;
-                  if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 2532, __pyx_L56_error)
+                  __pyx_t_7 = (__pyx_t_33) ? __Pyx_PyObject_CallOneArg(__pyx_t_11, __pyx_t_33) : __Pyx_PyObject_CallNoArg(__pyx_t_11);
+                  __Pyx_XDECREF(__pyx_t_33); __pyx_t_33 = 0;
+                  if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 2532, __pyx_L79_error)
                   __Pyx_GOTREF(__pyx_t_7);
                   __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-                  __pyx_t_9 = PyObject_Length(__pyx_t_7); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1))) __PYX_ERR(0, 2532, __pyx_L56_error)
+                  __pyx_t_9 = PyObject_Length(__pyx_t_7); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1))) __PYX_ERR(0, 2532, __pyx_L79_error)
                   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
                   __pyx_t_5 = ((__pyx_t_9 > 0) != 0);
                   if (__pyx_t_5) {
 
                     /* "pyrfc/_cyrfc.pyx":2533
  *                         else:
  *                             if len(value.rstrip()) > 0:
  *                                 time(int(value[:2]), int(value[2:4]), int(value[4:6]))             # <<<<<<<<<<<<<<
  *                             cValue = fillString(value)
  *                     except Exception as ex:
  */
-                    __Pyx_GetModuleGlobalName(__pyx_t_11, __pyx_n_s_time); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 2533, __pyx_L56_error)
+                    __Pyx_GetModuleGlobalName(__pyx_t_11, __pyx_n_s_time); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 2533, __pyx_L79_error)
                     __Pyx_GOTREF(__pyx_t_11);
-                    __pyx_t_25 = __Pyx_PyObject_GetSlice(__pyx_v_value, 0, 2, NULL, NULL, &__pyx_slice__29, 0, 1, 1); if (unlikely(!__pyx_t_25)) __PYX_ERR(0, 2533, __pyx_L56_error)
-                    __Pyx_GOTREF(__pyx_t_25);
-                    __pyx_t_18 = __Pyx_PyNumber_Int(__pyx_t_25); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 2533, __pyx_L56_error)
+                    __pyx_t_33 = __Pyx_PyObject_GetSlice(__pyx_v_value, 0, 2, NULL, NULL, &__pyx_slice__30, 0, 1, 1); if (unlikely(!__pyx_t_33)) __PYX_ERR(0, 2533, __pyx_L79_error)
+                    __Pyx_GOTREF(__pyx_t_33);
+                    __pyx_t_18 = __Pyx_PyNumber_Int(__pyx_t_33); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 2533, __pyx_L79_error)
                     __Pyx_GOTREF(__pyx_t_18);
-                    __Pyx_DECREF(__pyx_t_25); __pyx_t_25 = 0;
-                    __pyx_t_25 = __Pyx_PyObject_GetSlice(__pyx_v_value, 2, 4, NULL, NULL, &__pyx_slice__40, 1, 1, 1); if (unlikely(!__pyx_t_25)) __PYX_ERR(0, 2533, __pyx_L56_error)
-                    __Pyx_GOTREF(__pyx_t_25);
-                    __pyx_t_6 = __Pyx_PyNumber_Int(__pyx_t_25); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 2533, __pyx_L56_error)
+                    __Pyx_DECREF(__pyx_t_33); __pyx_t_33 = 0;
+                    __pyx_t_33 = __Pyx_PyObject_GetSlice(__pyx_v_value, 2, 4, NULL, NULL, &__pyx_slice__41, 1, 1, 1); if (unlikely(!__pyx_t_33)) __PYX_ERR(0, 2533, __pyx_L79_error)
+                    __Pyx_GOTREF(__pyx_t_33);
+                    __pyx_t_6 = __Pyx_PyNumber_Int(__pyx_t_33); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 2533, __pyx_L79_error)
                     __Pyx_GOTREF(__pyx_t_6);
-                    __Pyx_DECREF(__pyx_t_25); __pyx_t_25 = 0;
-                    __pyx_t_25 = __Pyx_PyObject_GetSlice(__pyx_v_value, 4, 6, NULL, NULL, &__pyx_slice__38, 1, 1, 1); if (unlikely(!__pyx_t_25)) __PYX_ERR(0, 2533, __pyx_L56_error)
-                    __Pyx_GOTREF(__pyx_t_25);
-                    __pyx_t_21 = __Pyx_PyNumber_Int(__pyx_t_25); if (unlikely(!__pyx_t_21)) __PYX_ERR(0, 2533, __pyx_L56_error)
-                    __Pyx_GOTREF(__pyx_t_21);
-                    __Pyx_DECREF(__pyx_t_25); __pyx_t_25 = 0;
-                    __pyx_t_25 = NULL;
+                    __Pyx_DECREF(__pyx_t_33); __pyx_t_33 = 0;
+                    __pyx_t_33 = __Pyx_PyObject_GetSlice(__pyx_v_value, 4, 6, NULL, NULL, &__pyx_slice__39, 1, 1, 1); if (unlikely(!__pyx_t_33)) __PYX_ERR(0, 2533, __pyx_L79_error)
+                    __Pyx_GOTREF(__pyx_t_33);
+                    __pyx_t_28 = __Pyx_PyNumber_Int(__pyx_t_33); if (unlikely(!__pyx_t_28)) __PYX_ERR(0, 2533, __pyx_L79_error)
+                    __Pyx_GOTREF(__pyx_t_28);
+                    __Pyx_DECREF(__pyx_t_33); __pyx_t_33 = 0;
+                    __pyx_t_33 = NULL;
                     __pyx_t_10 = 0;
                     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_11))) {
-                      __pyx_t_25 = PyMethod_GET_SELF(__pyx_t_11);
-                      if (likely(__pyx_t_25)) {
+                      __pyx_t_33 = PyMethod_GET_SELF(__pyx_t_11);
+                      if (likely(__pyx_t_33)) {
                         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_11);
-                        __Pyx_INCREF(__pyx_t_25);
+                        __Pyx_INCREF(__pyx_t_33);
                         __Pyx_INCREF(function);
                         __Pyx_DECREF_SET(__pyx_t_11, function);
                         __pyx_t_10 = 1;
                       }
                     }
                     #if CYTHON_FAST_PYCALL
                     if (PyFunction_Check(__pyx_t_11)) {
-                      PyObject *__pyx_temp[4] = {__pyx_t_25, __pyx_t_18, __pyx_t_6, __pyx_t_21};
-                      __pyx_t_7 = __Pyx_PyFunction_FastCall(__pyx_t_11, __pyx_temp+1-__pyx_t_10, 3+__pyx_t_10); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 2533, __pyx_L56_error)
-                      __Pyx_XDECREF(__pyx_t_25); __pyx_t_25 = 0;
+                      PyObject *__pyx_temp[4] = {__pyx_t_33, __pyx_t_18, __pyx_t_6, __pyx_t_28};
+                      __pyx_t_7 = __Pyx_PyFunction_FastCall(__pyx_t_11, __pyx_temp+1-__pyx_t_10, 3+__pyx_t_10); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 2533, __pyx_L79_error)
+                      __Pyx_XDECREF(__pyx_t_33); __pyx_t_33 = 0;
                       __Pyx_GOTREF(__pyx_t_7);
                       __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
                       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-                      __Pyx_DECREF(__pyx_t_21); __pyx_t_21 = 0;
+                      __Pyx_DECREF(__pyx_t_28); __pyx_t_28 = 0;
                     } else
                     #endif
                     #if CYTHON_FAST_PYCCALL
                     if (__Pyx_PyFastCFunction_Check(__pyx_t_11)) {
-                      PyObject *__pyx_temp[4] = {__pyx_t_25, __pyx_t_18, __pyx_t_6, __pyx_t_21};
-                      __pyx_t_7 = __Pyx_PyCFunction_FastCall(__pyx_t_11, __pyx_temp+1-__pyx_t_10, 3+__pyx_t_10); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 2533, __pyx_L56_error)
-                      __Pyx_XDECREF(__pyx_t_25); __pyx_t_25 = 0;
+                      PyObject *__pyx_temp[4] = {__pyx_t_33, __pyx_t_18, __pyx_t_6, __pyx_t_28};
+                      __pyx_t_7 = __Pyx_PyCFunction_FastCall(__pyx_t_11, __pyx_temp+1-__pyx_t_10, 3+__pyx_t_10); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 2533, __pyx_L79_error)
+                      __Pyx_XDECREF(__pyx_t_33); __pyx_t_33 = 0;
                       __Pyx_GOTREF(__pyx_t_7);
                       __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
                       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-                      __Pyx_DECREF(__pyx_t_21); __pyx_t_21 = 0;
+                      __Pyx_DECREF(__pyx_t_28); __pyx_t_28 = 0;
                     } else
                     #endif
                     {
-                      __pyx_t_19 = PyTuple_New(3+__pyx_t_10); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 2533, __pyx_L56_error)
+                      __pyx_t_19 = PyTuple_New(3+__pyx_t_10); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 2533, __pyx_L79_error)
                       __Pyx_GOTREF(__pyx_t_19);
-                      if (__pyx_t_25) {
-                        __Pyx_GIVEREF(__pyx_t_25); PyTuple_SET_ITEM(__pyx_t_19, 0, __pyx_t_25); __pyx_t_25 = NULL;
+                      if (__pyx_t_33) {
+                        __Pyx_GIVEREF(__pyx_t_33); PyTuple_SET_ITEM(__pyx_t_19, 0, __pyx_t_33); __pyx_t_33 = NULL;
                       }
                       __Pyx_GIVEREF(__pyx_t_18);
                       PyTuple_SET_ITEM(__pyx_t_19, 0+__pyx_t_10, __pyx_t_18);
                       __Pyx_GIVEREF(__pyx_t_6);
                       PyTuple_SET_ITEM(__pyx_t_19, 1+__pyx_t_10, __pyx_t_6);
-                      __Pyx_GIVEREF(__pyx_t_21);
-                      PyTuple_SET_ITEM(__pyx_t_19, 2+__pyx_t_10, __pyx_t_21);
+                      __Pyx_GIVEREF(__pyx_t_28);
+                      PyTuple_SET_ITEM(__pyx_t_19, 2+__pyx_t_10, __pyx_t_28);
                       __pyx_t_18 = 0;
                       __pyx_t_6 = 0;
-                      __pyx_t_21 = 0;
-                      __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_11, __pyx_t_19, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 2533, __pyx_L56_error)
+                      __pyx_t_28 = 0;
+                      __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_11, __pyx_t_19, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 2533, __pyx_L79_error)
                       __Pyx_GOTREF(__pyx_t_7);
                       __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
                     }
                     __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
                     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
                     /* "pyrfc/_cyrfc.pyx":2532
@@ -32516,94 +33170,112 @@
                   /* "pyrfc/_cyrfc.pyx":2534
  *                             if len(value.rstrip()) > 0:
  *                                 time(int(value[:2]), int(value[2:4]), int(value[4:6]))
  *                             cValue = fillString(value)             # <<<<<<<<<<<<<<
  *                     except Exception as ex:
  *                         format_ok = False
  */
-                  __pyx_t_14 = __pyx_f_5pyrfc_6_cyrfc_fillString(__pyx_v_value); if (unlikely(__pyx_t_14 == ((SAP_UC *)NULL))) __PYX_ERR(0, 2534, __pyx_L56_error)
+                  __pyx_t_14 = __pyx_f_5pyrfc_6_cyrfc_fillString(__pyx_v_value); if (unlikely(__pyx_t_14 == ((SAP_UC *)NULL))) __PYX_ERR(0, 2534, __pyx_L79_error)
                   __pyx_v_cValue = __pyx_t_14;
                 }
-                __pyx_L62:;
+                __pyx_L85:;
 
                 /* "pyrfc/_cyrfc.pyx":2528
  *                     cValue = fillString(f'{value.hour:02}{value.minute:02}{value.second:02}')
  *                 else:
  *                     try:             # <<<<<<<<<<<<<<
  *                         if len(value) != 6:
  *                             format_ok = False
  */
               }
               __Pyx_XDECREF(__pyx_t_17); __pyx_t_17 = 0;
               __Pyx_XDECREF(__pyx_t_16); __pyx_t_16 = 0;
               __Pyx_XDECREF(__pyx_t_15); __pyx_t_15 = 0;
-              goto __pyx_L61_try_end;
-              __pyx_L56_error:;
+              goto __pyx_L84_try_end;
+              __pyx_L79_error:;
               __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
               __Pyx_XDECREF(__pyx_t_18); __pyx_t_18 = 0;
               __Pyx_XDECREF(__pyx_t_19); __pyx_t_19 = 0;
-              __Pyx_XDECREF(__pyx_t_21); __pyx_t_21 = 0;
-              __Pyx_XDECREF(__pyx_t_25); __pyx_t_25 = 0;
+              __Pyx_XDECREF(__pyx_t_28); __pyx_t_28 = 0;
+              __Pyx_XDECREF(__pyx_t_33); __pyx_t_33 = 0;
               __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
               __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
 
               /* "pyrfc/_cyrfc.pyx":2535
  *                                 time(int(value[:2]), int(value[2:4]), int(value[4:6]))
  *                             cValue = fillString(value)
  *                     except Exception as ex:             # <<<<<<<<<<<<<<
  *                         format_ok = False
  * 
  */
               __pyx_t_10 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
               if (__pyx_t_10) {
                 __Pyx_AddTraceback("pyrfc._cyrfc.fillVariable", __pyx_clineno, __pyx_lineno, __pyx_filename);
-                if (__Pyx_GetException(&__pyx_t_7, &__pyx_t_11, &__pyx_t_19) < 0) __PYX_ERR(0, 2535, __pyx_L58_except_error)
+                if (__Pyx_GetException(&__pyx_t_7, &__pyx_t_11, &__pyx_t_19) < 0) __PYX_ERR(0, 2535, __pyx_L81_except_error)
                 __Pyx_GOTREF(__pyx_t_7);
                 __Pyx_GOTREF(__pyx_t_11);
                 __Pyx_GOTREF(__pyx_t_19);
                 __Pyx_INCREF(__pyx_t_11);
                 __pyx_v_ex = __pyx_t_11;
+                /*try:*/ {
 
-                /* "pyrfc/_cyrfc.pyx":2536
+                  /* "pyrfc/_cyrfc.pyx":2536
  *                             cValue = fillString(value)
  *                     except Exception as ex:
  *                         format_ok = False             # <<<<<<<<<<<<<<
  * 
  *                 if not format_ok:
  */
-                __pyx_v_format_ok = 0;
+                  __pyx_v_format_ok = 0;
+                }
+
+                /* "pyrfc/_cyrfc.pyx":2535
+ *                                 time(int(value[:2]), int(value[2:4]), int(value[4:6]))
+ *                             cValue = fillString(value)
+ *                     except Exception as ex:             # <<<<<<<<<<<<<<
+ *                         format_ok = False
+ * 
+ */
+                /*finally:*/ {
+                  /*normal exit:*/{
+                    __Pyx_DECREF(__pyx_v_ex);
+                    __pyx_v_ex = NULL;
+                    goto __pyx_L93;
+                  }
+                  __pyx_L93:;
+                }
                 __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
                 __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
                 __Pyx_XDECREF(__pyx_t_19); __pyx_t_19 = 0;
-                goto __pyx_L57_exception_handled;
+                goto __pyx_L80_exception_handled;
               }
-              goto __pyx_L58_except_error;
-              __pyx_L58_except_error:;
+              goto __pyx_L81_except_error;
+              __pyx_L81_except_error:;
 
               /* "pyrfc/_cyrfc.pyx":2528
  *                     cValue = fillString(f'{value.hour:02}{value.minute:02}{value.second:02}')
  *                 else:
  *                     try:             # <<<<<<<<<<<<<<
  *                         if len(value) != 6:
  *                             format_ok = False
  */
               __Pyx_XGIVEREF(__pyx_t_17);
               __Pyx_XGIVEREF(__pyx_t_16);
               __Pyx_XGIVEREF(__pyx_t_15);
               __Pyx_ExceptionReset(__pyx_t_17, __pyx_t_16, __pyx_t_15);
               goto __pyx_L3_error;
-              __pyx_L57_exception_handled:;
+              __pyx_L80_exception_handled:;
               __Pyx_XGIVEREF(__pyx_t_17);
               __Pyx_XGIVEREF(__pyx_t_16);
               __Pyx_XGIVEREF(__pyx_t_15);
               __Pyx_ExceptionReset(__pyx_t_17, __pyx_t_16, __pyx_t_15);
-              __pyx_L61_try_end:;
+              __pyx_L84_try_end:;
             }
           }
-          __pyx_L55:;
+          __pyx_L78:;
 
           /* "pyrfc/_cyrfc.pyx":2538
  *                         format_ok = False
  * 
  *                 if not format_ok:             # <<<<<<<<<<<<<<
  *                     raise TypeError('time value required, received', value, 'of type', type(value))
  *                 rc = RfcSetTime(container, cName, cValue, &errorInfo)
@@ -32616,23 +33288,23 @@
  *                 if not format_ok:
  *                     raise TypeError('time value required, received', value, 'of type', type(value))             # <<<<<<<<<<<<<<
  *                 rc = RfcSetTime(container, cName, cValue, &errorInfo)
  *                 free(cValue)
  */
             __pyx_t_19 = PyTuple_New(4); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 2539, __pyx_L3_error)
             __Pyx_GOTREF(__pyx_t_19);
-            __Pyx_INCREF(__pyx_kp_s_time_value_required_received);
-            __Pyx_GIVEREF(__pyx_kp_s_time_value_required_received);
-            PyTuple_SET_ITEM(__pyx_t_19, 0, __pyx_kp_s_time_value_required_received);
+            __Pyx_INCREF(__pyx_kp_u_time_value_required_received);
+            __Pyx_GIVEREF(__pyx_kp_u_time_value_required_received);
+            PyTuple_SET_ITEM(__pyx_t_19, 0, __pyx_kp_u_time_value_required_received);
             __Pyx_INCREF(__pyx_v_value);
             __Pyx_GIVEREF(__pyx_v_value);
             PyTuple_SET_ITEM(__pyx_t_19, 1, __pyx_v_value);
-            __Pyx_INCREF(__pyx_kp_s_of_type);
-            __Pyx_GIVEREF(__pyx_kp_s_of_type);
-            PyTuple_SET_ITEM(__pyx_t_19, 2, __pyx_kp_s_of_type);
+            __Pyx_INCREF(__pyx_kp_u_of_type);
+            __Pyx_GIVEREF(__pyx_kp_u_of_type);
+            PyTuple_SET_ITEM(__pyx_t_19, 2, __pyx_kp_u_of_type);
             __Pyx_INCREF(((PyObject *)Py_TYPE(__pyx_v_value)));
             __Pyx_GIVEREF(((PyObject *)Py_TYPE(__pyx_v_value)));
             PyTuple_SET_ITEM(__pyx_t_19, 3, ((PyObject *)Py_TYPE(__pyx_v_value)));
             __pyx_t_11 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_t_19, NULL); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 2539, __pyx_L3_error)
             __Pyx_GOTREF(__pyx_t_11);
             __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
             __Pyx_Raise(__pyx_t_11, 0, 0, 0);
@@ -32669,28 +33341,28 @@
           /* "pyrfc/_cyrfc.pyx":2523
  *                 rc = RFC_OK
  *         elif typ == RFCTYPE_TIME:
  *             if value:             # <<<<<<<<<<<<<<
  *                 format_ok = True
  *                 if type(value) is time:
  */
-          goto __pyx_L54;
+          goto __pyx_L77;
         }
 
         /* "pyrfc/_cyrfc.pyx":2543
  *                 free(cValue)
  *             else:
  *                 rc = RFC_OK             # <<<<<<<<<<<<<<
  *         else:
  *             raise RFCError('Unknown RFC type %d when filling %s' % (typ, wrapString(cName)))
  */
         /*else*/ {
           __pyx_v_rc = RFC_OK;
         }
-        __pyx_L54:;
+        __pyx_L77:;
 
         /* "pyrfc/_cyrfc.pyx":2522
  *             else:
  *                 rc = RFC_OK
  *         elif typ == RFCTYPE_TIME:             # <<<<<<<<<<<<<<
  *             if value:
  *                 format_ok = True
@@ -32703,42 +33375,59 @@
  *         else:
  *             raise RFCError('Unknown RFC type %d when filling %s' % (typ, wrapString(cName)))             # <<<<<<<<<<<<<<
  *     except TypeError as e:
  *         # This way the field name will be attached in reverse direction
  */
         __Pyx_GetModuleGlobalName(__pyx_t_19, __pyx_n_s_RFCError); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 2545, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_19);
-        __pyx_t_7 = __Pyx_PyInt_From_RFCTYPE(__pyx_v_typ); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 2545, __pyx_L3_error)
+        __pyx_t_7 = PyTuple_New(4); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 2545, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_7);
-        __pyx_t_21 = __pyx_f_5pyrfc_6_cyrfc_wrapString(__pyx_v_cName, NULL); if (unlikely(!__pyx_t_21)) __PYX_ERR(0, 2545, __pyx_L3_error)
-        __Pyx_GOTREF(__pyx_t_21);
-        __pyx_t_6 = PyTuple_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 2545, __pyx_L3_error)
+        __pyx_t_9 = 0;
+        __pyx_t_32 = 127;
+        __Pyx_INCREF(__pyx_kp_u_Unknown_RFC_type);
+        __pyx_t_9 += 17;
+        __Pyx_GIVEREF(__pyx_kp_u_Unknown_RFC_type);
+        PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_kp_u_Unknown_RFC_type);
+        __pyx_t_28 = __Pyx_PyUnicode_From_RFCTYPE(__pyx_v_typ, 0, ' ', 'd'); if (unlikely(!__pyx_t_28)) __PYX_ERR(0, 2545, __pyx_L3_error)
+        __Pyx_GOTREF(__pyx_t_28);
+        __pyx_t_32 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_28) > __pyx_t_32) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_28) : __pyx_t_32;
+        __pyx_t_9 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_28);
+        __Pyx_GIVEREF(__pyx_t_28);
+        PyTuple_SET_ITEM(__pyx_t_7, 1, __pyx_t_28);
+        __pyx_t_28 = 0;
+        __Pyx_INCREF(__pyx_kp_u_when_filling);
+        __pyx_t_9 += 14;
+        __Pyx_GIVEREF(__pyx_kp_u_when_filling);
+        PyTuple_SET_ITEM(__pyx_t_7, 2, __pyx_kp_u_when_filling);
+        __pyx_t_28 = __pyx_f_5pyrfc_6_cyrfc_wrapString(__pyx_v_cName, NULL); if (unlikely(!__pyx_t_28)) __PYX_ERR(0, 2545, __pyx_L3_error)
+        __Pyx_GOTREF(__pyx_t_28);
+        __pyx_t_6 = __Pyx_PyObject_FormatSimpleAndDecref(PyObject_Unicode(__pyx_t_28), __pyx_empty_unicode); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 2545, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_6);
-        __Pyx_GIVEREF(__pyx_t_7);
-        PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_7);
-        __Pyx_GIVEREF(__pyx_t_21);
-        PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_t_21);
-        __pyx_t_7 = 0;
-        __pyx_t_21 = 0;
-        __pyx_t_21 = __Pyx_PyString_Format(__pyx_kp_s_Unknown_RFC_type_d_when_filling, __pyx_t_6); if (unlikely(!__pyx_t_21)) __PYX_ERR(0, 2545, __pyx_L3_error)
-        __Pyx_GOTREF(__pyx_t_21);
-        __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-        __pyx_t_6 = NULL;
+        __Pyx_DECREF(__pyx_t_28); __pyx_t_28 = 0;
+        __pyx_t_32 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_6) > __pyx_t_32) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_6) : __pyx_t_32;
+        __pyx_t_9 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_6);
+        __Pyx_GIVEREF(__pyx_t_6);
+        PyTuple_SET_ITEM(__pyx_t_7, 3, __pyx_t_6);
+        __pyx_t_6 = 0;
+        __pyx_t_6 = __Pyx_PyUnicode_Join(__pyx_t_7, 4, __pyx_t_9, __pyx_t_32); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 2545, __pyx_L3_error)
+        __Pyx_GOTREF(__pyx_t_6);
+        __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+        __pyx_t_7 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_19))) {
-          __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_19);
-          if (likely(__pyx_t_6)) {
+          __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_19);
+          if (likely(__pyx_t_7)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_19);
-            __Pyx_INCREF(__pyx_t_6);
+            __Pyx_INCREF(__pyx_t_7);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_19, function);
           }
         }
-        __pyx_t_11 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_19, __pyx_t_6, __pyx_t_21) : __Pyx_PyObject_CallOneArg(__pyx_t_19, __pyx_t_21);
-        __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-        __Pyx_DECREF(__pyx_t_21); __pyx_t_21 = 0;
+        __pyx_t_11 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_19, __pyx_t_7, __pyx_t_6) : __Pyx_PyObject_CallOneArg(__pyx_t_19, __pyx_t_6);
+        __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
+        __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
         if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 2545, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_11);
         __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
         __Pyx_Raise(__pyx_t_11, 0, 0, 0);
         __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
         __PYX_ERR(0, 2545, __pyx_L3_error)
         break;
@@ -32756,72 +33445,120 @@
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
     __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
     __Pyx_XDECREF(__pyx_t_18); __pyx_t_18 = 0;
     __Pyx_XDECREF(__pyx_t_19); __pyx_t_19 = 0;
-    __Pyx_XDECREF(__pyx_t_21); __pyx_t_21 = 0;
-    __Pyx_XDECREF(__pyx_t_25); __pyx_t_25 = 0;
+    __Pyx_XDECREF(__pyx_t_28); __pyx_t_28 = 0;
+    __Pyx_XDECREF(__pyx_t_33); __pyx_t_33 = 0;
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
 
     /* "pyrfc/_cyrfc.pyx":2546
  *         else:
  *             raise RFCError('Unknown RFC type %d when filling %s' % (typ, wrapString(cName)))
  *     except TypeError as e:             # <<<<<<<<<<<<<<
  *         # This way the field name will be attached in reverse direction
  *         # to the argument list of the exception. This helps users to find
  */
     __pyx_t_10 = __Pyx_PyErr_ExceptionMatches(__pyx_builtin_TypeError);
     if (__pyx_t_10) {
       __Pyx_AddTraceback("pyrfc._cyrfc.fillVariable", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_11, &__pyx_t_19, &__pyx_t_21) < 0) __PYX_ERR(0, 2546, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_11, &__pyx_t_19, &__pyx_t_6) < 0) __PYX_ERR(0, 2546, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_11);
       __Pyx_GOTREF(__pyx_t_19);
-      __Pyx_GOTREF(__pyx_t_21);
+      __Pyx_GOTREF(__pyx_t_6);
       __Pyx_INCREF(__pyx_t_19);
       __pyx_v_e = __pyx_t_19;
+      /*try:*/ {
 
-      /* "pyrfc/_cyrfc.pyx":2550
+        /* "pyrfc/_cyrfc.pyx":2550
  *         # to the argument list of the exception. This helps users to find
  *         # mistakes easier in complex mapping scenarios.
  *         e.args += (wrapString(cName), )             # <<<<<<<<<<<<<<
  *         raise
  *     if rc != RFC_OK:
  */
-      __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_e, __pyx_n_s_args); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 2550, __pyx_L5_except_error)
-      __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_7 = __pyx_f_5pyrfc_6_cyrfc_wrapString(__pyx_v_cName, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 2550, __pyx_L5_except_error)
-      __Pyx_GOTREF(__pyx_t_7);
-      __pyx_t_18 = PyTuple_New(1); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 2550, __pyx_L5_except_error)
-      __Pyx_GOTREF(__pyx_t_18);
-      __Pyx_GIVEREF(__pyx_t_7);
-      PyTuple_SET_ITEM(__pyx_t_18, 0, __pyx_t_7);
-      __pyx_t_7 = 0;
-      __pyx_t_7 = PyNumber_InPlaceAdd(__pyx_t_6, __pyx_t_18); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 2550, __pyx_L5_except_error)
-      __Pyx_GOTREF(__pyx_t_7);
-      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
-      if (__Pyx_PyObject_SetAttrStr(__pyx_v_e, __pyx_n_s_args, __pyx_t_7) < 0) __PYX_ERR(0, 2550, __pyx_L5_except_error)
-      __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+        __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_e, __pyx_n_s_args); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 2550, __pyx_L100_error)
+        __Pyx_GOTREF(__pyx_t_7);
+        __pyx_t_28 = __pyx_f_5pyrfc_6_cyrfc_wrapString(__pyx_v_cName, NULL); if (unlikely(!__pyx_t_28)) __PYX_ERR(0, 2550, __pyx_L100_error)
+        __Pyx_GOTREF(__pyx_t_28);
+        __pyx_t_18 = PyTuple_New(1); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 2550, __pyx_L100_error)
+        __Pyx_GOTREF(__pyx_t_18);
+        __Pyx_GIVEREF(__pyx_t_28);
+        PyTuple_SET_ITEM(__pyx_t_18, 0, __pyx_t_28);
+        __pyx_t_28 = 0;
+        __pyx_t_28 = PyNumber_InPlaceAdd(__pyx_t_7, __pyx_t_18); if (unlikely(!__pyx_t_28)) __PYX_ERR(0, 2550, __pyx_L100_error)
+        __Pyx_GOTREF(__pyx_t_28);
+        __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+        __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
+        if (__Pyx_PyObject_SetAttrStr(__pyx_v_e, __pyx_n_s_args, __pyx_t_28) < 0) __PYX_ERR(0, 2550, __pyx_L100_error)
+        __Pyx_DECREF(__pyx_t_28); __pyx_t_28 = 0;
 
-      /* "pyrfc/_cyrfc.pyx":2551
+        /* "pyrfc/_cyrfc.pyx":2551
  *         # mistakes easier in complex mapping scenarios.
  *         e.args += (wrapString(cName), )
  *         raise             # <<<<<<<<<<<<<<
  *     if rc != RFC_OK:
  *         raise wrapError(&errorInfo)
  */
-      __Pyx_GIVEREF(__pyx_t_11);
-      __Pyx_GIVEREF(__pyx_t_19);
-      __Pyx_XGIVEREF(__pyx_t_21);
-      __Pyx_ErrRestoreWithState(__pyx_t_11, __pyx_t_19, __pyx_t_21);
-      __pyx_t_11 = 0; __pyx_t_19 = 0; __pyx_t_21 = 0; 
-      __PYX_ERR(0, 2551, __pyx_L5_except_error)
+        __Pyx_GIVEREF(__pyx_t_11);
+        __Pyx_GIVEREF(__pyx_t_19);
+        __Pyx_XGIVEREF(__pyx_t_6);
+        __Pyx_ErrRestoreWithState(__pyx_t_11, __pyx_t_19, __pyx_t_6);
+        __pyx_t_11 = 0; __pyx_t_19 = 0; __pyx_t_6 = 0; 
+        __PYX_ERR(0, 2551, __pyx_L100_error)
+      }
+
+      /* "pyrfc/_cyrfc.pyx":2546
+ *         else:
+ *             raise RFCError('Unknown RFC type %d when filling %s' % (typ, wrapString(cName)))
+ *     except TypeError as e:             # <<<<<<<<<<<<<<
+ *         # This way the field name will be attached in reverse direction
+ *         # to the argument list of the exception. This helps users to find
+ */
+      /*finally:*/ {
+        __pyx_L100_error:;
+        /*exception exit:*/{
+          __Pyx_PyThreadState_declare
+          __Pyx_PyThreadState_assign
+          __pyx_t_15 = 0; __pyx_t_16 = 0; __pyx_t_17 = 0; __pyx_t_21 = 0; __pyx_t_22 = 0; __pyx_t_23 = 0;
+          __Pyx_XDECREF(__pyx_t_18); __pyx_t_18 = 0;
+          __Pyx_XDECREF(__pyx_t_28); __pyx_t_28 = 0;
+          __Pyx_XDECREF(__pyx_t_33); __pyx_t_33 = 0;
+          __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
+          if (PY_MAJOR_VERSION >= 3) __Pyx_ExceptionSwap(&__pyx_t_21, &__pyx_t_22, &__pyx_t_23);
+          if ((PY_MAJOR_VERSION < 3) || unlikely(__Pyx_GetException(&__pyx_t_15, &__pyx_t_16, &__pyx_t_17) < 0)) __Pyx_ErrFetch(&__pyx_t_15, &__pyx_t_16, &__pyx_t_17);
+          __Pyx_XGOTREF(__pyx_t_15);
+          __Pyx_XGOTREF(__pyx_t_16);
+          __Pyx_XGOTREF(__pyx_t_17);
+          __Pyx_XGOTREF(__pyx_t_21);
+          __Pyx_XGOTREF(__pyx_t_22);
+          __Pyx_XGOTREF(__pyx_t_23);
+          __pyx_t_10 = __pyx_lineno; __pyx_t_12 = __pyx_clineno; __pyx_t_34 = __pyx_filename;
+          {
+            __Pyx_DECREF(__pyx_v_e);
+            __pyx_v_e = NULL;
+          }
+          if (PY_MAJOR_VERSION >= 3) {
+            __Pyx_XGIVEREF(__pyx_t_21);
+            __Pyx_XGIVEREF(__pyx_t_22);
+            __Pyx_XGIVEREF(__pyx_t_23);
+            __Pyx_ExceptionReset(__pyx_t_21, __pyx_t_22, __pyx_t_23);
+          }
+          __Pyx_XGIVEREF(__pyx_t_15);
+          __Pyx_XGIVEREF(__pyx_t_16);
+          __Pyx_XGIVEREF(__pyx_t_17);
+          __Pyx_ErrRestore(__pyx_t_15, __pyx_t_16, __pyx_t_17);
+          __pyx_t_15 = 0; __pyx_t_16 = 0; __pyx_t_17 = 0; __pyx_t_21 = 0; __pyx_t_22 = 0; __pyx_t_23 = 0;
+          __pyx_lineno = __pyx_t_10; __pyx_clineno = __pyx_t_12; __pyx_filename = __pyx_t_34;
+          goto __pyx_L5_except_error;
+        }
+      }
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
     /* "pyrfc/_cyrfc.pyx":2422
  *     global _LOCALE_RADIX
  *     # print ("fill", wrapString(cName), value, type(value))
@@ -32850,18 +33587,18 @@
     /* "pyrfc/_cyrfc.pyx":2553
  *         raise
  *     if rc != RFC_OK:
  *         raise wrapError(&errorInfo)             # <<<<<<<<<<<<<<
  * 
  * cdef SAP_RAW* fillBytes(pystr) except NULL:
  */
-    __pyx_t_21 = __pyx_f_5pyrfc_6_cyrfc_wrapError((&__pyx_v_errorInfo)); if (unlikely(!__pyx_t_21)) __PYX_ERR(0, 2553, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_21);
-    __Pyx_Raise(__pyx_t_21, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_21); __pyx_t_21 = 0;
+    __pyx_t_6 = __pyx_f_5pyrfc_6_cyrfc_wrapError((&__pyx_v_errorInfo)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 2553, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __Pyx_Raise(__pyx_t_6, 0, 0, 0);
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __PYX_ERR(0, 2553, __pyx_L1_error)
 
     /* "pyrfc/_cyrfc.pyx":2552
  *         e.args += (wrapString(cName), )
  *         raise
  *     if rc != RFC_OK:             # <<<<<<<<<<<<<<
  *         raise wrapError(&errorInfo)
@@ -32882,16 +33619,16 @@
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_6);
   __Pyx_XDECREF(__pyx_t_7);
   __Pyx_XDECREF(__pyx_t_11);
   __Pyx_XDECREF(__pyx_t_18);
   __Pyx_XDECREF(__pyx_t_19);
-  __Pyx_XDECREF(__pyx_t_21);
-  __Pyx_XDECREF(__pyx_t_25);
+  __Pyx_XDECREF(__pyx_t_28);
+  __Pyx_XDECREF(__pyx_t_33);
   __Pyx_AddTraceback("pyrfc._cyrfc.fillVariable", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_name);
   __Pyx_XDECREF(__pyx_v_ex);
   __Pyx_XDECREF(__pyx_v_svalue);
   __Pyx_XDECREF(__pyx_v_locale_radix);
@@ -33144,15 +33881,15 @@
       if (likely(__pyx_t_2)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_2);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
-    __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_2, __pyx_kp_s_Not_a_valid_error_group) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_kp_s_Not_a_valid_error_group);
+    __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_2, __pyx_kp_u_Not_a_valid_error_group) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_kp_u_Not_a_valid_error_group);
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2572, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __PYX_ERR(0, 2572, __pyx_L1_error)
@@ -33197,15 +33934,15 @@
  *         # str = exception.message[0:512].ljust(512)
  *         str = exception.message[0:512]             # <<<<<<<<<<<<<<
  *         sapuc = fillString(str)
  *         strncpyU(errorInfo.message, sapuc, min(len(str)+1, 512))
  */
     __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_exception, __pyx_n_s_message); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2578, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = __Pyx_PyObject_GetSlice(__pyx_t_1, 0, 0x200, NULL, NULL, &__pyx_slice__41, 1, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2578, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetSlice(__pyx_t_1, 0, 0x200, NULL, NULL, &__pyx_slice__42, 1, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2578, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_v_str = __pyx_t_3;
     __pyx_t_3 = 0;
 
     /* "pyrfc/_cyrfc.pyx":2579
  *         # str = exception.message[0:512].ljust(512)
@@ -33292,15 +34029,15 @@
  *     if exception.key:  # fixed length, exactly 128 chars
  *         str = exception.key[0:128]             # <<<<<<<<<<<<<<
  *         sapuc = fillString(str)
  *         strncpyU(errorInfo.key, sapuc, min(len(str)+1, 128))
  */
     __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_exception, __pyx_n_s_key); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2584, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_1 = __Pyx_PyObject_GetSlice(__pyx_t_3, 0, 0x80, NULL, NULL, &__pyx_slice__42, 1, 1, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2584, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetSlice(__pyx_t_3, 0, 0x80, NULL, NULL, &__pyx_slice__43, 1, 1, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2584, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_XDECREF_SET(__pyx_v_str, __pyx_t_1);
     __pyx_t_1 = 0;
 
     /* "pyrfc/_cyrfc.pyx":2585
  *     if exception.key:  # fixed length, exactly 128 chars
@@ -33428,15 +34165,15 @@
  *     if exception.msg_type:
  *         sapuc = fillString(exception.msg_type[0:1])             # <<<<<<<<<<<<<<
  *         strncpyU(errorInfo.abapMsgType, sapuc, len(exception.msg_type[0:1]) + 1)
  *         free(sapuc)
  */
     __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_exception, __pyx_n_s_msg_type); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2593, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = __Pyx_PyObject_GetSlice(__pyx_t_1, 0, 1, NULL, NULL, &__pyx_slice__43, 1, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2593, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetSlice(__pyx_t_1, 0, 1, NULL, NULL, &__pyx_slice__44, 1, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2593, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_7 = __pyx_f_5pyrfc_6_cyrfc_fillString(__pyx_t_3); if (unlikely(__pyx_t_7 == ((SAP_UC *)NULL))) __PYX_ERR(0, 2593, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_v_sapuc = __pyx_t_7;
 
     /* "pyrfc/_cyrfc.pyx":2594
@@ -33444,15 +34181,15 @@
  *         sapuc = fillString(exception.msg_type[0:1])
  *         strncpyU(errorInfo.abapMsgType, sapuc, len(exception.msg_type[0:1]) + 1)             # <<<<<<<<<<<<<<
  *         free(sapuc)
  *     if exception.msg_number:
  */
     __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_exception, __pyx_n_s_msg_type); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2594, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_1 = __Pyx_PyObject_GetSlice(__pyx_t_3, 0, 1, NULL, NULL, &__pyx_slice__43, 1, 1, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2594, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetSlice(__pyx_t_3, 0, 1, NULL, NULL, &__pyx_slice__44, 1, 1, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2594, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_9 = PyObject_Length(__pyx_t_1); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1))) __PYX_ERR(0, 2594, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     strncpyU(__pyx_v_errorInfo->abapMsgType, __pyx_v_sapuc, (__pyx_t_9 + 1));
 
     /* "pyrfc/_cyrfc.pyx":2595
@@ -33554,15 +34291,15 @@
  *     if exception.msg_v1:
  *         sapuc = fillString(exception.msg_v1[0:50])             # <<<<<<<<<<<<<<
  *         strncpyU(errorInfo.abapMsgV1, sapuc, len(exception.msg_v1[0:50]) + 1)
  *         free(sapuc)
  */
     __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_exception, __pyx_n_s_msg_v1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2601, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = __Pyx_PyObject_GetSlice(__pyx_t_1, 0, 50, NULL, NULL, &__pyx_slice__44, 1, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2601, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetSlice(__pyx_t_1, 0, 50, NULL, NULL, &__pyx_slice__45, 1, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2601, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_7 = __pyx_f_5pyrfc_6_cyrfc_fillString(__pyx_t_3); if (unlikely(__pyx_t_7 == ((SAP_UC *)NULL))) __PYX_ERR(0, 2601, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_v_sapuc = __pyx_t_7;
 
     /* "pyrfc/_cyrfc.pyx":2602
@@ -33570,15 +34307,15 @@
  *         sapuc = fillString(exception.msg_v1[0:50])
  *         strncpyU(errorInfo.abapMsgV1, sapuc, len(exception.msg_v1[0:50]) + 1)             # <<<<<<<<<<<<<<
  *         free(sapuc)
  *     if exception.msg_v2:
  */
     __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_exception, __pyx_n_s_msg_v1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2602, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_1 = __Pyx_PyObject_GetSlice(__pyx_t_3, 0, 50, NULL, NULL, &__pyx_slice__44, 1, 1, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2602, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetSlice(__pyx_t_3, 0, 50, NULL, NULL, &__pyx_slice__45, 1, 1, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2602, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_9 = PyObject_Length(__pyx_t_1); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1))) __PYX_ERR(0, 2602, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     strncpyU(__pyx_v_errorInfo->abapMsgV1, __pyx_v_sapuc, (__pyx_t_9 + 1));
 
     /* "pyrfc/_cyrfc.pyx":2603
@@ -33617,15 +34354,15 @@
  *     if exception.msg_v2:
  *         sapuc = fillString(exception.msg_v2[0:50])             # <<<<<<<<<<<<<<
  *         strncpyU(errorInfo.abapMsgV2, sapuc, len(exception.msg_v2[0:50]) + 1)
  *         free(sapuc)
  */
     __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_exception, __pyx_n_s_msg_v2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2605, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = __Pyx_PyObject_GetSlice(__pyx_t_1, 0, 50, NULL, NULL, &__pyx_slice__44, 1, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2605, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetSlice(__pyx_t_1, 0, 50, NULL, NULL, &__pyx_slice__45, 1, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2605, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_7 = __pyx_f_5pyrfc_6_cyrfc_fillString(__pyx_t_3); if (unlikely(__pyx_t_7 == ((SAP_UC *)NULL))) __PYX_ERR(0, 2605, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_v_sapuc = __pyx_t_7;
 
     /* "pyrfc/_cyrfc.pyx":2606
@@ -33633,15 +34370,15 @@
  *         sapuc = fillString(exception.msg_v2[0:50])
  *         strncpyU(errorInfo.abapMsgV2, sapuc, len(exception.msg_v2[0:50]) + 1)             # <<<<<<<<<<<<<<
  *         free(sapuc)
  *     if exception.msg_v3:
  */
     __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_exception, __pyx_n_s_msg_v2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2606, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_1 = __Pyx_PyObject_GetSlice(__pyx_t_3, 0, 50, NULL, NULL, &__pyx_slice__44, 1, 1, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2606, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetSlice(__pyx_t_3, 0, 50, NULL, NULL, &__pyx_slice__45, 1, 1, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2606, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_9 = PyObject_Length(__pyx_t_1); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1))) __PYX_ERR(0, 2606, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     strncpyU(__pyx_v_errorInfo->abapMsgV2, __pyx_v_sapuc, (__pyx_t_9 + 1));
 
     /* "pyrfc/_cyrfc.pyx":2607
@@ -33680,15 +34417,15 @@
  *     if exception.msg_v3:
  *         sapuc = fillString(exception.msg_v3[0:50])             # <<<<<<<<<<<<<<
  *         strncpyU(errorInfo.abapMsgV3, sapuc, len(exception.msg_v3[0:50]) + 1)
  *         free(sapuc)
  */
     __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_exception, __pyx_n_s_msg_v3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2609, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = __Pyx_PyObject_GetSlice(__pyx_t_1, 0, 50, NULL, NULL, &__pyx_slice__44, 1, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2609, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetSlice(__pyx_t_1, 0, 50, NULL, NULL, &__pyx_slice__45, 1, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2609, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_7 = __pyx_f_5pyrfc_6_cyrfc_fillString(__pyx_t_3); if (unlikely(__pyx_t_7 == ((SAP_UC *)NULL))) __PYX_ERR(0, 2609, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_v_sapuc = __pyx_t_7;
 
     /* "pyrfc/_cyrfc.pyx":2610
@@ -33696,15 +34433,15 @@
  *         sapuc = fillString(exception.msg_v3[0:50])
  *         strncpyU(errorInfo.abapMsgV3, sapuc, len(exception.msg_v3[0:50]) + 1)             # <<<<<<<<<<<<<<
  *         free(sapuc)
  *     if exception.msg_v4:
  */
     __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_exception, __pyx_n_s_msg_v3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2610, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_1 = __Pyx_PyObject_GetSlice(__pyx_t_3, 0, 50, NULL, NULL, &__pyx_slice__44, 1, 1, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2610, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetSlice(__pyx_t_3, 0, 50, NULL, NULL, &__pyx_slice__45, 1, 1, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2610, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_9 = PyObject_Length(__pyx_t_1); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1))) __PYX_ERR(0, 2610, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     strncpyU(__pyx_v_errorInfo->abapMsgV3, __pyx_v_sapuc, (__pyx_t_9 + 1));
 
     /* "pyrfc/_cyrfc.pyx":2611
@@ -33743,15 +34480,15 @@
  *     if exception.msg_v4:
  *         sapuc = fillString(exception.msg_v4[0:50])             # <<<<<<<<<<<<<<
  *         strncpyU(errorInfo.abapMsgV4, sapuc, len(exception.msg_v4[0:50]) + 1)
  *         free(sapuc)
  */
     __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_exception, __pyx_n_s_msg_v4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2613, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = __Pyx_PyObject_GetSlice(__pyx_t_1, 0, 50, NULL, NULL, &__pyx_slice__44, 1, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2613, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetSlice(__pyx_t_1, 0, 50, NULL, NULL, &__pyx_slice__45, 1, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2613, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_7 = __pyx_f_5pyrfc_6_cyrfc_fillString(__pyx_t_3); if (unlikely(__pyx_t_7 == ((SAP_UC *)NULL))) __PYX_ERR(0, 2613, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_v_sapuc = __pyx_t_7;
 
     /* "pyrfc/_cyrfc.pyx":2614
@@ -33759,15 +34496,15 @@
  *         sapuc = fillString(exception.msg_v4[0:50])
  *         strncpyU(errorInfo.abapMsgV4, sapuc, len(exception.msg_v4[0:50]) + 1)             # <<<<<<<<<<<<<<
  *         free(sapuc)
  * 
  */
     __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_exception, __pyx_n_s_msg_v4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2614, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_1 = __Pyx_PyObject_GetSlice(__pyx_t_3, 0, 50, NULL, NULL, &__pyx_slice__44, 1, 1, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2614, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetSlice(__pyx_t_3, 0, 50, NULL, NULL, &__pyx_slice__45, 1, 1, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2614, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_9 = PyObject_Length(__pyx_t_1); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1))) __PYX_ERR(0, 2614, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     strncpyU(__pyx_v_errorInfo->abapMsgV4, __pyx_v_sapuc, (__pyx_t_9 + 1));
 
     /* "pyrfc/_cyrfc.pyx":2615
@@ -34060,20 +34797,20 @@
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_5, function);
     }
   }
-  __pyx_t_2 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_3, __pyx_kp_s__45) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_kp_s__45);
+  __pyx_t_2 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_3, __pyx_kp_u__46) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_kp_u__46);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2639, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dest, __pyx_t_2) < 0) __PYX_ERR(0, 2639, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_dest, __pyx_t_2) < 0) __PYX_ERR(0, 2639, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "pyrfc/_cyrfc.pyx":2640
  *     return {
  *         'dest': wrapString(attributes.dest, 64, True).rstrip('\0')
  *         , 'host': wrapString(attributes.host, 100, True).rstrip('\0')             # <<<<<<<<<<<<<<
  *         , 'partnerHost': wrapString(attributes.partnerHost, 100, True).rstrip('\0')
@@ -34093,20 +34830,20 @@
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
-  __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_5, __pyx_kp_s__45) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_kp_s__45);
+  __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_5, __pyx_kp_u__46) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_kp_u__46);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
   if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2640, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_host, __pyx_t_2) < 0) __PYX_ERR(0, 2639, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_host, __pyx_t_2) < 0) __PYX_ERR(0, 2639, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "pyrfc/_cyrfc.pyx":2641
  *         'dest': wrapString(attributes.dest, 64, True).rstrip('\0')
  *         , 'host': wrapString(attributes.host, 100, True).rstrip('\0')
  *         , 'partnerHost': wrapString(attributes.partnerHost, 100, True).rstrip('\0')             # <<<<<<<<<<<<<<
  *         , 'sysNumber': wrapString(attributes.sysNumber, 2, True).rstrip('\0')
@@ -34126,20 +34863,20 @@
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_5, function);
     }
   }
-  __pyx_t_2 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_3, __pyx_kp_s__45) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_kp_s__45);
+  __pyx_t_2 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_3, __pyx_kp_u__46) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_kp_u__46);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2641, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_partnerHost, __pyx_t_2) < 0) __PYX_ERR(0, 2639, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_partnerHost, __pyx_t_2) < 0) __PYX_ERR(0, 2639, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "pyrfc/_cyrfc.pyx":2642
  *         , 'host': wrapString(attributes.host, 100, True).rstrip('\0')
  *         , 'partnerHost': wrapString(attributes.partnerHost, 100, True).rstrip('\0')
  *         , 'sysNumber': wrapString(attributes.sysNumber, 2, True).rstrip('\0')             # <<<<<<<<<<<<<<
  *         , 'sysId': wrapString(attributes.sysId, 8, True).rstrip('\0')
@@ -34159,20 +34896,20 @@
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
-  __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_5, __pyx_kp_s__45) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_kp_s__45);
+  __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_5, __pyx_kp_u__46) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_kp_u__46);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
   if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2642, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_sysNumber, __pyx_t_2) < 0) __PYX_ERR(0, 2639, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_sysNumber, __pyx_t_2) < 0) __PYX_ERR(0, 2639, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "pyrfc/_cyrfc.pyx":2643
  *         , 'partnerHost': wrapString(attributes.partnerHost, 100, True).rstrip('\0')
  *         , 'sysNumber': wrapString(attributes.sysNumber, 2, True).rstrip('\0')
  *         , 'sysId': wrapString(attributes.sysId, 8, True).rstrip('\0')             # <<<<<<<<<<<<<<
  *         , 'client': wrapString(attributes.client, 3, True).rstrip('\0')
@@ -34192,20 +34929,20 @@
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_5, function);
     }
   }
-  __pyx_t_2 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_3, __pyx_kp_s__45) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_kp_s__45);
+  __pyx_t_2 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_3, __pyx_kp_u__46) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_kp_u__46);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2643, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_sysId, __pyx_t_2) < 0) __PYX_ERR(0, 2639, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_sysId, __pyx_t_2) < 0) __PYX_ERR(0, 2639, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "pyrfc/_cyrfc.pyx":2644
  *         , 'sysNumber': wrapString(attributes.sysNumber, 2, True).rstrip('\0')
  *         , 'sysId': wrapString(attributes.sysId, 8, True).rstrip('\0')
  *         , 'client': wrapString(attributes.client, 3, True).rstrip('\0')             # <<<<<<<<<<<<<<
  *         , 'user': wrapString(attributes.user, 12, True).rstrip('\0')
@@ -34225,20 +34962,20 @@
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
-  __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_5, __pyx_kp_s__45) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_kp_s__45);
+  __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_5, __pyx_kp_u__46) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_kp_u__46);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
   if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2644, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_client, __pyx_t_2) < 0) __PYX_ERR(0, 2639, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_client, __pyx_t_2) < 0) __PYX_ERR(0, 2639, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "pyrfc/_cyrfc.pyx":2645
  *         , 'sysId': wrapString(attributes.sysId, 8, True).rstrip('\0')
  *         , 'client': wrapString(attributes.client, 3, True).rstrip('\0')
  *         , 'user': wrapString(attributes.user, 12, True).rstrip('\0')             # <<<<<<<<<<<<<<
  *         , 'language': wrapString(attributes.language, 2, True).rstrip('\0')
@@ -34258,20 +34995,20 @@
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_5, function);
     }
   }
-  __pyx_t_2 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_3, __pyx_kp_s__45) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_kp_s__45);
+  __pyx_t_2 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_3, __pyx_kp_u__46) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_kp_u__46);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2645, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_user, __pyx_t_2) < 0) __PYX_ERR(0, 2639, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_user, __pyx_t_2) < 0) __PYX_ERR(0, 2639, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "pyrfc/_cyrfc.pyx":2646
  *         , 'client': wrapString(attributes.client, 3, True).rstrip('\0')
  *         , 'user': wrapString(attributes.user, 12, True).rstrip('\0')
  *         , 'language': wrapString(attributes.language, 2, True).rstrip('\0')             # <<<<<<<<<<<<<<
  *         , 'trace': wrapString(attributes.trace, 1, True).rstrip('\0')
@@ -34291,20 +35028,20 @@
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
-  __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_5, __pyx_kp_s__45) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_kp_s__45);
+  __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_5, __pyx_kp_u__46) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_kp_u__46);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
   if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2646, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_language, __pyx_t_2) < 0) __PYX_ERR(0, 2639, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_language, __pyx_t_2) < 0) __PYX_ERR(0, 2639, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "pyrfc/_cyrfc.pyx":2647
  *         , 'user': wrapString(attributes.user, 12, True).rstrip('\0')
  *         , 'language': wrapString(attributes.language, 2, True).rstrip('\0')
  *         , 'trace': wrapString(attributes.trace, 1, True).rstrip('\0')             # <<<<<<<<<<<<<<
  *         , 'isoLanguage': wrapString(attributes.isoLanguage, 2, True).rstrip('\0')
@@ -34324,20 +35061,20 @@
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_5, function);
     }
   }
-  __pyx_t_2 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_3, __pyx_kp_s__45) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_kp_s__45);
+  __pyx_t_2 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_3, __pyx_kp_u__46) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_kp_u__46);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2647, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_trace, __pyx_t_2) < 0) __PYX_ERR(0, 2639, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_trace, __pyx_t_2) < 0) __PYX_ERR(0, 2639, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "pyrfc/_cyrfc.pyx":2648
  *         , 'language': wrapString(attributes.language, 2, True).rstrip('\0')
  *         , 'trace': wrapString(attributes.trace, 1, True).rstrip('\0')
  *         , 'isoLanguage': wrapString(attributes.isoLanguage, 2, True).rstrip('\0')             # <<<<<<<<<<<<<<
  *         , 'codepage': wrapString(attributes.codepage, 4, True).rstrip('\0')
@@ -34357,20 +35094,20 @@
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
-  __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_5, __pyx_kp_s__45) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_kp_s__45);
+  __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_5, __pyx_kp_u__46) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_kp_u__46);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
   if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2648, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_isoLanguage, __pyx_t_2) < 0) __PYX_ERR(0, 2639, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_isoLanguage, __pyx_t_2) < 0) __PYX_ERR(0, 2639, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "pyrfc/_cyrfc.pyx":2649
  *         , 'trace': wrapString(attributes.trace, 1, True).rstrip('\0')
  *         , 'isoLanguage': wrapString(attributes.isoLanguage, 2, True).rstrip('\0')
  *         , 'codepage': wrapString(attributes.codepage, 4, True).rstrip('\0')             # <<<<<<<<<<<<<<
  *         , 'partnerCodepage': wrapString(attributes.partnerCodepage, 4, True).rstrip('\0')
@@ -34390,20 +35127,20 @@
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_5, function);
     }
   }
-  __pyx_t_2 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_3, __pyx_kp_s__45) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_kp_s__45);
+  __pyx_t_2 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_3, __pyx_kp_u__46) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_kp_u__46);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2649, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_codepage, __pyx_t_2) < 0) __PYX_ERR(0, 2639, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_codepage, __pyx_t_2) < 0) __PYX_ERR(0, 2639, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "pyrfc/_cyrfc.pyx":2650
  *         , 'isoLanguage': wrapString(attributes.isoLanguage, 2, True).rstrip('\0')
  *         , 'codepage': wrapString(attributes.codepage, 4, True).rstrip('\0')
  *         , 'partnerCodepage': wrapString(attributes.partnerCodepage, 4, True).rstrip('\0')             # <<<<<<<<<<<<<<
  *         , 'rfcRole': wrapString(attributes.rfcRole, 1, True).rstrip('\0')
@@ -34423,20 +35160,20 @@
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
-  __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_5, __pyx_kp_s__45) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_kp_s__45);
+  __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_5, __pyx_kp_u__46) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_kp_u__46);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
   if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2650, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_partnerCodepage, __pyx_t_2) < 0) __PYX_ERR(0, 2639, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_partnerCodepage, __pyx_t_2) < 0) __PYX_ERR(0, 2639, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "pyrfc/_cyrfc.pyx":2651
  *         , 'codepage': wrapString(attributes.codepage, 4, True).rstrip('\0')
  *         , 'partnerCodepage': wrapString(attributes.partnerCodepage, 4, True).rstrip('\0')
  *         , 'rfcRole': wrapString(attributes.rfcRole, 1, True).rstrip('\0')             # <<<<<<<<<<<<<<
  *         , 'type': wrapString(attributes.type, 1).rstrip('\0')
@@ -34456,20 +35193,20 @@
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_5, function);
     }
   }
-  __pyx_t_2 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_3, __pyx_kp_s__45) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_kp_s__45);
+  __pyx_t_2 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_3, __pyx_kp_u__46) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_kp_u__46);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2651, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_rfcRole, __pyx_t_2) < 0) __PYX_ERR(0, 2639, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_rfcRole, __pyx_t_2) < 0) __PYX_ERR(0, 2639, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "pyrfc/_cyrfc.pyx":2652
  *         , 'partnerCodepage': wrapString(attributes.partnerCodepage, 4, True).rstrip('\0')
  *         , 'rfcRole': wrapString(attributes.rfcRole, 1, True).rstrip('\0')
  *         , 'type': wrapString(attributes.type, 1).rstrip('\0')             # <<<<<<<<<<<<<<
  *         , 'partnerType': wrapString(attributes.partnerType, 1, True).rstrip('\0')
@@ -34488,20 +35225,20 @@
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
-  __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_5, __pyx_kp_s__45) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_kp_s__45);
+  __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_5, __pyx_kp_u__46) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_kp_u__46);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
   if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2652, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_type, __pyx_t_2) < 0) __PYX_ERR(0, 2639, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_type, __pyx_t_2) < 0) __PYX_ERR(0, 2639, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "pyrfc/_cyrfc.pyx":2653
  *         , 'rfcRole': wrapString(attributes.rfcRole, 1, True).rstrip('\0')
  *         , 'type': wrapString(attributes.type, 1).rstrip('\0')
  *         , 'partnerType': wrapString(attributes.partnerType, 1, True).rstrip('\0')             # <<<<<<<<<<<<<<
  *         , 'rel': wrapString(attributes.rel, 4, True).rstrip('\0')
@@ -34521,20 +35258,20 @@
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_5, function);
     }
   }
-  __pyx_t_2 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_3, __pyx_kp_s__45) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_kp_s__45);
+  __pyx_t_2 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_3, __pyx_kp_u__46) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_kp_u__46);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2653, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_partnerType, __pyx_t_2) < 0) __PYX_ERR(0, 2639, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_partnerType, __pyx_t_2) < 0) __PYX_ERR(0, 2639, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "pyrfc/_cyrfc.pyx":2654
  *         , 'type': wrapString(attributes.type, 1).rstrip('\0')
  *         , 'partnerType': wrapString(attributes.partnerType, 1, True).rstrip('\0')
  *         , 'rel': wrapString(attributes.rel, 4, True).rstrip('\0')             # <<<<<<<<<<<<<<
  *         , 'partnerRel': wrapString(attributes.partnerRel, 4, True).rstrip('\0')
@@ -34554,20 +35291,20 @@
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
-  __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_5, __pyx_kp_s__45) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_kp_s__45);
+  __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_5, __pyx_kp_u__46) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_kp_u__46);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
   if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2654, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_rel, __pyx_t_2) < 0) __PYX_ERR(0, 2639, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_rel, __pyx_t_2) < 0) __PYX_ERR(0, 2639, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "pyrfc/_cyrfc.pyx":2655
  *         , 'partnerType': wrapString(attributes.partnerType, 1, True).rstrip('\0')
  *         , 'rel': wrapString(attributes.rel, 4, True).rstrip('\0')
  *         , 'partnerRel': wrapString(attributes.partnerRel, 4, True).rstrip('\0')             # <<<<<<<<<<<<<<
  *         , 'kernelRel': wrapString(attributes.kernelRel, 4, True).rstrip('\0')
@@ -34587,20 +35324,20 @@
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_5, function);
     }
   }
-  __pyx_t_2 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_3, __pyx_kp_s__45) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_kp_s__45);
+  __pyx_t_2 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_3, __pyx_kp_u__46) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_kp_u__46);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2655, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_partnerRel, __pyx_t_2) < 0) __PYX_ERR(0, 2639, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_partnerRel, __pyx_t_2) < 0) __PYX_ERR(0, 2639, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "pyrfc/_cyrfc.pyx":2656
  *         , 'rel': wrapString(attributes.rel, 4, True).rstrip('\0')
  *         , 'partnerRel': wrapString(attributes.partnerRel, 4, True).rstrip('\0')
  *         , 'kernelRel': wrapString(attributes.kernelRel, 4, True).rstrip('\0')             # <<<<<<<<<<<<<<
  *         , 'cpicConvId': wrapString(attributes.cpicConvId, 8, True).rstrip('\0')
@@ -34620,20 +35357,20 @@
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
-  __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_5, __pyx_kp_s__45) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_kp_s__45);
+  __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_5, __pyx_kp_u__46) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_kp_u__46);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
   if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2656, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_kernelRel, __pyx_t_2) < 0) __PYX_ERR(0, 2639, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_kernelRel, __pyx_t_2) < 0) __PYX_ERR(0, 2639, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "pyrfc/_cyrfc.pyx":2657
  *         , 'partnerRel': wrapString(attributes.partnerRel, 4, True).rstrip('\0')
  *         , 'kernelRel': wrapString(attributes.kernelRel, 4, True).rstrip('\0')
  *         , 'cpicConvId': wrapString(attributes.cpicConvId, 8, True).rstrip('\0')             # <<<<<<<<<<<<<<
  *         , 'progName': wrapString(attributes.progName, 128, True).rstrip('\0')
@@ -34653,20 +35390,20 @@
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_5, function);
     }
   }
-  __pyx_t_2 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_3, __pyx_kp_s__45) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_kp_s__45);
+  __pyx_t_2 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_3, __pyx_kp_u__46) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_kp_u__46);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2657, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_cpicConvId, __pyx_t_2) < 0) __PYX_ERR(0, 2639, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_cpicConvId, __pyx_t_2) < 0) __PYX_ERR(0, 2639, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "pyrfc/_cyrfc.pyx":2658
  *         , 'kernelRel': wrapString(attributes.kernelRel, 4, True).rstrip('\0')
  *         , 'cpicConvId': wrapString(attributes.cpicConvId, 8, True).rstrip('\0')
  *         , 'progName': wrapString(attributes.progName, 128, True).rstrip('\0')             # <<<<<<<<<<<<<<
  *         , 'partnerBytesPerChar': wrapString(attributes.partnerBytesPerChar, 1, True).rstrip('\0')
@@ -34686,20 +35423,20 @@
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
-  __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_5, __pyx_kp_s__45) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_kp_s__45);
+  __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_5, __pyx_kp_u__46) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_kp_u__46);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
   if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2658, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_progName, __pyx_t_2) < 0) __PYX_ERR(0, 2639, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_progName, __pyx_t_2) < 0) __PYX_ERR(0, 2639, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "pyrfc/_cyrfc.pyx":2659
  *         , 'cpicConvId': wrapString(attributes.cpicConvId, 8, True).rstrip('\0')
  *         , 'progName': wrapString(attributes.progName, 128, True).rstrip('\0')
  *         , 'partnerBytesPerChar': wrapString(attributes.partnerBytesPerChar, 1, True).rstrip('\0')             # <<<<<<<<<<<<<<
  *         , 'partnerSystemCodepage': wrapString(attributes.partnerSystemCodepage, 4, True).rstrip('\0')
@@ -34719,20 +35456,20 @@
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_5, function);
     }
   }
-  __pyx_t_2 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_3, __pyx_kp_s__45) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_kp_s__45);
+  __pyx_t_2 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_3, __pyx_kp_u__46) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_kp_u__46);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2659, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_partnerBytesPerChar, __pyx_t_2) < 0) __PYX_ERR(0, 2639, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_partnerBytesPerChar, __pyx_t_2) < 0) __PYX_ERR(0, 2639, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "pyrfc/_cyrfc.pyx":2660
  *         , 'progName': wrapString(attributes.progName, 128, True).rstrip('\0')
  *         , 'partnerBytesPerChar': wrapString(attributes.partnerBytesPerChar, 1, True).rstrip('\0')
  *         , 'partnerSystemCodepage': wrapString(attributes.partnerSystemCodepage, 4, True).rstrip('\0')             # <<<<<<<<<<<<<<
  *         , 'partnerIP': wrapString(attributes.partnerIP, 15, True).rstrip('\0')
@@ -34752,20 +35489,20 @@
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
-  __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_5, __pyx_kp_s__45) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_kp_s__45);
+  __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_5, __pyx_kp_u__46) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_kp_u__46);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
   if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2660, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_partnerSystemCodepage, __pyx_t_2) < 0) __PYX_ERR(0, 2639, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_partnerSystemCodepage, __pyx_t_2) < 0) __PYX_ERR(0, 2639, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "pyrfc/_cyrfc.pyx":2661
  *         , 'partnerBytesPerChar': wrapString(attributes.partnerBytesPerChar, 1, True).rstrip('\0')
  *         , 'partnerSystemCodepage': wrapString(attributes.partnerSystemCodepage, 4, True).rstrip('\0')
  *         , 'partnerIP': wrapString(attributes.partnerIP, 15, True).rstrip('\0')             # <<<<<<<<<<<<<<
  *         , 'partnerIPv6': wrapString(attributes.partnerIPv6, 45, True).rstrip('\0')
@@ -34785,20 +35522,20 @@
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_5, function);
     }
   }
-  __pyx_t_2 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_3, __pyx_kp_s__45) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_kp_s__45);
+  __pyx_t_2 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_3, __pyx_kp_u__46) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_kp_u__46);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2661, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_partnerIP, __pyx_t_2) < 0) __PYX_ERR(0, 2639, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_partnerIP, __pyx_t_2) < 0) __PYX_ERR(0, 2639, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "pyrfc/_cyrfc.pyx":2662
  *         , 'partnerSystemCodepage': wrapString(attributes.partnerSystemCodepage, 4, True).rstrip('\0')
  *         , 'partnerIP': wrapString(attributes.partnerIP, 15, True).rstrip('\0')
  *         , 'partnerIPv6': wrapString(attributes.partnerIPv6, 45, True).rstrip('\0')             # <<<<<<<<<<<<<<
  *         , 'reserved': wrapString(attributes.reserved, 17, True).rstrip('\0')
@@ -34818,20 +35555,20 @@
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
-  __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_5, __pyx_kp_s__45) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_kp_s__45);
+  __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_5, __pyx_kp_u__46) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_kp_u__46);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
   if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2662, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_partnerIPv6, __pyx_t_2) < 0) __PYX_ERR(0, 2639, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_partnerIPv6, __pyx_t_2) < 0) __PYX_ERR(0, 2639, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "pyrfc/_cyrfc.pyx":2663
  *         , 'partnerIP': wrapString(attributes.partnerIP, 15, True).rstrip('\0')
  *         , 'partnerIPv6': wrapString(attributes.partnerIPv6, 45, True).rstrip('\0')
  *         , 'reserved': wrapString(attributes.reserved, 17, True).rstrip('\0')             # <<<<<<<<<<<<<<
  *     }
@@ -34851,20 +35588,20 @@
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_5, function);
     }
   }
-  __pyx_t_2 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_3, __pyx_kp_s__45) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_kp_s__45);
+  __pyx_t_2 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_3, __pyx_kp_u__46) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_kp_u__46);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2663, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_reserved, __pyx_t_2) < 0) __PYX_ERR(0, 2639, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_reserved, __pyx_t_2) < 0) __PYX_ERR(0, 2639, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* "pyrfc/_cyrfc.pyx":2637
  * # wrapper functions take C values and returns Python values
@@ -35189,15 +35926,15 @@
  *             'field_type': RfcFieldType(fieldDesc.type).name,
  *             'nuc_length': fieldDesc.nucLength,
  */
     __pyx_t_2 = __Pyx_PyDict_NewPresized(7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2697, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_3 = __pyx_f_5pyrfc_6_cyrfc_wrapString(__pyx_v_fieldDesc.name, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2697, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_name, __pyx_t_3) < 0) __PYX_ERR(0, 2697, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_name, __pyx_t_3) < 0) __PYX_ERR(0, 2697, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
     /* "pyrfc/_cyrfc.pyx":2698
  *         field_description = {
  *             'name': wrapString(fieldDesc.name),
  *             'field_type': RfcFieldType(fieldDesc.type).name,             # <<<<<<<<<<<<<<
  *             'nuc_length': fieldDesc.nucLength,
@@ -35222,75 +35959,75 @@
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2698, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_name); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 2698, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_field_type, __pyx_t_8) < 0) __PYX_ERR(0, 2697, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_field_type, __pyx_t_8) < 0) __PYX_ERR(0, 2697, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
     /* "pyrfc/_cyrfc.pyx":2699
  *             'name': wrapString(fieldDesc.name),
  *             'field_type': RfcFieldType(fieldDesc.type).name,
  *             'nuc_length': fieldDesc.nucLength,             # <<<<<<<<<<<<<<
  *             'nuc_offset': fieldDesc.nucOffset,
  *             'uc_length': fieldDesc.ucLength,
  */
     __pyx_t_8 = __Pyx_PyInt_From_unsigned_int(__pyx_v_fieldDesc.nucLength); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 2699, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
-    if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_nuc_length, __pyx_t_8) < 0) __PYX_ERR(0, 2697, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_nuc_length, __pyx_t_8) < 0) __PYX_ERR(0, 2697, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
     /* "pyrfc/_cyrfc.pyx":2700
  *             'field_type': RfcFieldType(fieldDesc.type).name,
  *             'nuc_length': fieldDesc.nucLength,
  *             'nuc_offset': fieldDesc.nucOffset,             # <<<<<<<<<<<<<<
  *             'uc_length': fieldDesc.ucLength,
  *             'uc_offset': fieldDesc.ucOffset,
  */
     __pyx_t_8 = __Pyx_PyInt_From_unsigned_int(__pyx_v_fieldDesc.nucOffset); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 2700, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
-    if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_nuc_offset, __pyx_t_8) < 0) __PYX_ERR(0, 2697, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_nuc_offset, __pyx_t_8) < 0) __PYX_ERR(0, 2697, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
     /* "pyrfc/_cyrfc.pyx":2701
  *             'nuc_length': fieldDesc.nucLength,
  *             'nuc_offset': fieldDesc.nucOffset,
  *             'uc_length': fieldDesc.ucLength,             # <<<<<<<<<<<<<<
  *             'uc_offset': fieldDesc.ucOffset,
  *             'decimals': fieldDesc.decimals
  */
     __pyx_t_8 = __Pyx_PyInt_From_unsigned_int(__pyx_v_fieldDesc.ucLength); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 2701, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
-    if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_uc_length, __pyx_t_8) < 0) __PYX_ERR(0, 2697, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_uc_length, __pyx_t_8) < 0) __PYX_ERR(0, 2697, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
     /* "pyrfc/_cyrfc.pyx":2702
  *             'nuc_offset': fieldDesc.nucOffset,
  *             'uc_length': fieldDesc.ucLength,
  *             'uc_offset': fieldDesc.ucOffset,             # <<<<<<<<<<<<<<
  *             'decimals': fieldDesc.decimals
  *         }
  */
     __pyx_t_8 = __Pyx_PyInt_From_unsigned_int(__pyx_v_fieldDesc.ucOffset); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 2702, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
-    if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_uc_offset, __pyx_t_8) < 0) __PYX_ERR(0, 2697, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_uc_offset, __pyx_t_8) < 0) __PYX_ERR(0, 2697, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
     /* "pyrfc/_cyrfc.pyx":2703
  *             'uc_length': fieldDesc.ucLength,
  *             'uc_offset': fieldDesc.ucOffset,
  *             'decimals': fieldDesc.decimals             # <<<<<<<<<<<<<<
  *         }
  *         if fieldDesc.typeDescHandle is NULL:
  */
     __pyx_t_8 = __Pyx_PyInt_From_unsigned_int(__pyx_v_fieldDesc.decimals); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 2703, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
-    if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_decimals, __pyx_t_8) < 0) __PYX_ERR(0, 2697, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_decimals, __pyx_t_8) < 0) __PYX_ERR(0, 2697, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     __Pyx_XDECREF_SET(__pyx_v_field_description, ((PyObject*)__pyx_t_2));
     __pyx_t_2 = 0;
 
     /* "pyrfc/_cyrfc.pyx":2705
  *             'decimals': fieldDesc.decimals
  *         }
@@ -35304,15 +36041,15 @@
       /* "pyrfc/_cyrfc.pyx":2706
  *         }
  *         if fieldDesc.typeDescHandle is NULL:
  *             field_description['type_description'] = None             # <<<<<<<<<<<<<<
  *         else:
  *             field_description['type_description'] = wrapTypeDescription(fieldDesc.typeDescHandle)
  */
-      if (unlikely(PyDict_SetItem(__pyx_v_field_description, __pyx_n_s_type_description, Py_None) < 0)) __PYX_ERR(0, 2706, __pyx_L1_error)
+      if (unlikely(PyDict_SetItem(__pyx_v_field_description, __pyx_n_u_type_description, Py_None) < 0)) __PYX_ERR(0, 2706, __pyx_L1_error)
 
       /* "pyrfc/_cyrfc.pyx":2705
  *             'decimals': fieldDesc.decimals
  *         }
  *         if fieldDesc.typeDescHandle is NULL:             # <<<<<<<<<<<<<<
  *             field_description['type_description'] = None
  *         else:
@@ -35326,15 +36063,15 @@
  *             field_description['type_description'] = wrapTypeDescription(fieldDesc.typeDescHandle)             # <<<<<<<<<<<<<<
  *         # Add field to object
  *         type_desc.add_field(**field_description)
  */
     /*else*/ {
       __pyx_t_2 = __pyx_f_5pyrfc_6_cyrfc_wrapTypeDescription(__pyx_v_fieldDesc.typeDescHandle); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2708, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      if (unlikely(PyDict_SetItem(__pyx_v_field_description, __pyx_n_s_type_description, __pyx_t_2) < 0)) __PYX_ERR(0, 2708, __pyx_L1_error)
+      if (unlikely(PyDict_SetItem(__pyx_v_field_description, __pyx_n_u_type_description, __pyx_t_2) < 0)) __PYX_ERR(0, 2708, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     }
     __pyx_L9:;
 
     /* "pyrfc/_cyrfc.pyx":2710
  *             field_description['type_description'] = wrapTypeDescription(fieldDesc.typeDescHandle)
  *         # Add field to object
@@ -35607,15 +36344,15 @@
  *             'parameter_type': RfcFieldType(paramDesc.type).name,
  *             'direction': RfcParameterDirection(paramDesc.direction).name,
  */
     __pyx_t_2 = __Pyx_PyDict_NewPresized(9); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2735, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_3 = __pyx_f_5pyrfc_6_cyrfc_wrapString(__pyx_v_paramDesc.name, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2735, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_name, __pyx_t_3) < 0) __PYX_ERR(0, 2735, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_name, __pyx_t_3) < 0) __PYX_ERR(0, 2735, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
     /* "pyrfc/_cyrfc.pyx":2736
  *         parameter_description = {
  *             'name': wrapString(paramDesc.name),
  *             'parameter_type': RfcFieldType(paramDesc.type).name,             # <<<<<<<<<<<<<<
  *             'direction': RfcParameterDirection(paramDesc.direction).name,
@@ -35640,15 +36377,15 @@
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2736, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_name); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 2736, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_parameter_type, __pyx_t_4) < 0) __PYX_ERR(0, 2735, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_parameter_type, __pyx_t_4) < 0) __PYX_ERR(0, 2735, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "pyrfc/_cyrfc.pyx":2737
  *             'name': wrapString(paramDesc.name),
  *             'parameter_type': RfcFieldType(paramDesc.type).name,
  *             'direction': RfcParameterDirection(paramDesc.direction).name,             # <<<<<<<<<<<<<<
  *             'nuc_length': paramDesc.nucLength,
@@ -35673,75 +36410,75 @@
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 2737, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_name); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2737, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_direction, __pyx_t_3) < 0) __PYX_ERR(0, 2735, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_direction, __pyx_t_3) < 0) __PYX_ERR(0, 2735, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
     /* "pyrfc/_cyrfc.pyx":2738
  *             'parameter_type': RfcFieldType(paramDesc.type).name,
  *             'direction': RfcParameterDirection(paramDesc.direction).name,
  *             'nuc_length': paramDesc.nucLength,             # <<<<<<<<<<<<<<
  *             'uc_length': paramDesc.ucLength,
  *             'decimals': paramDesc.decimals,
  */
     __pyx_t_3 = __Pyx_PyInt_From_unsigned_int(__pyx_v_paramDesc.nucLength); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2738, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_nuc_length, __pyx_t_3) < 0) __PYX_ERR(0, 2735, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_nuc_length, __pyx_t_3) < 0) __PYX_ERR(0, 2735, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
     /* "pyrfc/_cyrfc.pyx":2739
  *             'direction': RfcParameterDirection(paramDesc.direction).name,
  *             'nuc_length': paramDesc.nucLength,
  *             'uc_length': paramDesc.ucLength,             # <<<<<<<<<<<<<<
  *             'decimals': paramDesc.decimals,
  *             'default_value': wrapString(paramDesc.defaultValue),
  */
     __pyx_t_3 = __Pyx_PyInt_From_unsigned_int(__pyx_v_paramDesc.ucLength); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2739, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_uc_length, __pyx_t_3) < 0) __PYX_ERR(0, 2735, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_uc_length, __pyx_t_3) < 0) __PYX_ERR(0, 2735, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
     /* "pyrfc/_cyrfc.pyx":2740
  *             'nuc_length': paramDesc.nucLength,
  *             'uc_length': paramDesc.ucLength,
  *             'decimals': paramDesc.decimals,             # <<<<<<<<<<<<<<
  *             'default_value': wrapString(paramDesc.defaultValue),
  *             'parameter_text': wrapString(paramDesc.parameterText),
  */
     __pyx_t_3 = __Pyx_PyInt_From_unsigned_int(__pyx_v_paramDesc.decimals); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2740, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_decimals, __pyx_t_3) < 0) __PYX_ERR(0, 2735, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_decimals, __pyx_t_3) < 0) __PYX_ERR(0, 2735, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
     /* "pyrfc/_cyrfc.pyx":2741
  *             'uc_length': paramDesc.ucLength,
  *             'decimals': paramDesc.decimals,
  *             'default_value': wrapString(paramDesc.defaultValue),             # <<<<<<<<<<<<<<
  *             'parameter_text': wrapString(paramDesc.parameterText),
  *             'optional': bool(paramDesc.optional)
  */
     __pyx_t_3 = __pyx_f_5pyrfc_6_cyrfc_wrapString(__pyx_v_paramDesc.defaultValue, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2741, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_default_value, __pyx_t_3) < 0) __PYX_ERR(0, 2735, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_default_value, __pyx_t_3) < 0) __PYX_ERR(0, 2735, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
     /* "pyrfc/_cyrfc.pyx":2742
  *             'decimals': paramDesc.decimals,
  *             'default_value': wrapString(paramDesc.defaultValue),
  *             'parameter_text': wrapString(paramDesc.parameterText),             # <<<<<<<<<<<<<<
  *             'optional': bool(paramDesc.optional)
  *             # skip: void* extendedDescription;
  */
     __pyx_t_3 = __pyx_f_5pyrfc_6_cyrfc_wrapString(__pyx_v_paramDesc.parameterText, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2742, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_parameter_text, __pyx_t_3) < 0) __PYX_ERR(0, 2735, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_parameter_text, __pyx_t_3) < 0) __PYX_ERR(0, 2735, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
     /* "pyrfc/_cyrfc.pyx":2743
  *             'default_value': wrapString(paramDesc.defaultValue),
  *             'parameter_text': wrapString(paramDesc.parameterText),
  *             'optional': bool(paramDesc.optional)             # <<<<<<<<<<<<<<
  *             # skip: void* extendedDescription;
@@ -35749,15 +36486,15 @@
  */
     __pyx_t_3 = __Pyx_PyInt_From_SAP_RAW(__pyx_v_paramDesc.optional); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2743, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 2743, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_3 = __Pyx_PyBool_FromLong((!(!__pyx_t_1))); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2743, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_optional, __pyx_t_3) < 0) __PYX_ERR(0, 2735, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_optional, __pyx_t_3) < 0) __PYX_ERR(0, 2735, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_XDECREF_SET(__pyx_v_parameter_description, ((PyObject*)__pyx_t_2));
     __pyx_t_2 = 0;
 
     /* "pyrfc/_cyrfc.pyx":2747
  *             # This field can be used by the application programmer (i.e. you) to store arbitrary extra information.
  *         }
@@ -35771,15 +36508,15 @@
       /* "pyrfc/_cyrfc.pyx":2748
  *         }
  *         if paramDesc.typeDescHandle is NULL:
  *             parameter_description['type_description'] = None             # <<<<<<<<<<<<<<
  *         else:
  *             parameter_description['type_description'] = wrapTypeDescription(paramDesc.typeDescHandle)
  */
-      if (unlikely(PyDict_SetItem(__pyx_v_parameter_description, __pyx_n_s_type_description, Py_None) < 0)) __PYX_ERR(0, 2748, __pyx_L1_error)
+      if (unlikely(PyDict_SetItem(__pyx_v_parameter_description, __pyx_n_u_type_description, Py_None) < 0)) __PYX_ERR(0, 2748, __pyx_L1_error)
 
       /* "pyrfc/_cyrfc.pyx":2747
  *             # This field can be used by the application programmer (i.e. you) to store arbitrary extra information.
  *         }
  *         if paramDesc.typeDescHandle is NULL:             # <<<<<<<<<<<<<<
  *             parameter_description['type_description'] = None
  *         else:
@@ -35793,15 +36530,15 @@
  *             parameter_description['type_description'] = wrapTypeDescription(paramDesc.typeDescHandle)             # <<<<<<<<<<<<<<
  *         func_desc.add_parameter(**parameter_description)
  * 
  */
     /*else*/ {
       __pyx_t_2 = __pyx_f_5pyrfc_6_cyrfc_wrapTypeDescription(__pyx_v_paramDesc.typeDescHandle); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2750, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      if (unlikely(PyDict_SetItem(__pyx_v_parameter_description, __pyx_n_s_type_description, __pyx_t_2) < 0)) __PYX_ERR(0, 2750, __pyx_L1_error)
+      if (unlikely(PyDict_SetItem(__pyx_v_parameter_description, __pyx_n_u_type_description, __pyx_t_2) < 0)) __PYX_ERR(0, 2750, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     }
     __pyx_L8:;
 
     /* "pyrfc/_cyrfc.pyx":2751
  *         else:
  *             parameter_description['type_description'] = wrapTypeDescription(paramDesc.typeDescHandle)
@@ -36032,29 +36769,29 @@
  */
   __pyx_t_1 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2789, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_3.__pyx_n = 1;
   __pyx_t_3.uclen = __pyx_int_1;
   __pyx_t_2 = __pyx_f_5pyrfc_6_cyrfc_wrapString((&__pyx_v_uIdentifier.unitType), &__pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2789, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = PyObject_RichCompare(__pyx_n_s_Q, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 2789, __pyx_L1_error)
+  __pyx_t_4 = PyObject_RichCompare(__pyx_n_u_Q, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 2789, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_queued, __pyx_t_4) < 0) __PYX_ERR(0, 2789, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_queued, __pyx_t_4) < 0) __PYX_ERR(0, 2789, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
   /* "pyrfc/_cyrfc.pyx":2790
  *     return {
  *         'queued': "Q" == wrapString(&uIdentifier.unitType, 1),
  *         'id': wrapString(uIdentifier.unitID)             # <<<<<<<<<<<<<<
  *     }
  * 
  */
   __pyx_t_4 = __pyx_f_5pyrfc_6_cyrfc_wrapString(__pyx_v_uIdentifier.unitID, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 2790, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_id, __pyx_t_4) < 0) __PYX_ERR(0, 2789, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_id, __pyx_t_4) < 0) __PYX_ERR(0, 2789, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* "pyrfc/_cyrfc.pyx":2787
  *     return result
@@ -36113,168 +36850,168 @@
  *     unit_attributes = {}
  *     unit_attributes['kernel_trace'] = uattr.kernelTrace != 0             # <<<<<<<<<<<<<<
  *     unit_attributes['sat_trace'] = uattr.satTrace != 0
  *     unit_attributes['unit_history'] = uattr.unitHistory != 0
  */
   __pyx_t_1 = __Pyx_PyBool_FromLong((__pyx_v_uattr->kernelTrace != 0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2795, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (unlikely(PyDict_SetItem(__pyx_v_unit_attributes, __pyx_n_s_kernel_trace, __pyx_t_1) < 0)) __PYX_ERR(0, 2795, __pyx_L1_error)
+  if (unlikely(PyDict_SetItem(__pyx_v_unit_attributes, __pyx_n_u_kernel_trace, __pyx_t_1) < 0)) __PYX_ERR(0, 2795, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "pyrfc/_cyrfc.pyx":2796
  *     unit_attributes = {}
  *     unit_attributes['kernel_trace'] = uattr.kernelTrace != 0
  *     unit_attributes['sat_trace'] = uattr.satTrace != 0             # <<<<<<<<<<<<<<
  *     unit_attributes['unit_history'] = uattr.unitHistory != 0
  *     unit_attributes['lock'] = uattr.lock != 0
  */
   __pyx_t_1 = __Pyx_PyBool_FromLong((__pyx_v_uattr->satTrace != 0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2796, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (unlikely(PyDict_SetItem(__pyx_v_unit_attributes, __pyx_n_s_sat_trace, __pyx_t_1) < 0)) __PYX_ERR(0, 2796, __pyx_L1_error)
+  if (unlikely(PyDict_SetItem(__pyx_v_unit_attributes, __pyx_n_u_sat_trace, __pyx_t_1) < 0)) __PYX_ERR(0, 2796, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "pyrfc/_cyrfc.pyx":2797
  *     unit_attributes['kernel_trace'] = uattr.kernelTrace != 0
  *     unit_attributes['sat_trace'] = uattr.satTrace != 0
  *     unit_attributes['unit_history'] = uattr.unitHistory != 0             # <<<<<<<<<<<<<<
  *     unit_attributes['lock'] = uattr.lock != 0
  *     unit_attributes['no_commit_check'] = uattr.noCommitCheck != 0
  */
   __pyx_t_1 = __Pyx_PyBool_FromLong((__pyx_v_uattr->unitHistory != 0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2797, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (unlikely(PyDict_SetItem(__pyx_v_unit_attributes, __pyx_n_s_unit_history, __pyx_t_1) < 0)) __PYX_ERR(0, 2797, __pyx_L1_error)
+  if (unlikely(PyDict_SetItem(__pyx_v_unit_attributes, __pyx_n_u_unit_history, __pyx_t_1) < 0)) __PYX_ERR(0, 2797, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "pyrfc/_cyrfc.pyx":2798
  *     unit_attributes['sat_trace'] = uattr.satTrace != 0
  *     unit_attributes['unit_history'] = uattr.unitHistory != 0
  *     unit_attributes['lock'] = uattr.lock != 0             # <<<<<<<<<<<<<<
  *     unit_attributes['no_commit_check'] = uattr.noCommitCheck != 0
  *     unit_attributes['user'] = wrapString(uattr.user, 12, True)
  */
   __pyx_t_1 = __Pyx_PyBool_FromLong((__pyx_v_uattr->lock != 0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2798, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (unlikely(PyDict_SetItem(__pyx_v_unit_attributes, __pyx_n_s_lock, __pyx_t_1) < 0)) __PYX_ERR(0, 2798, __pyx_L1_error)
+  if (unlikely(PyDict_SetItem(__pyx_v_unit_attributes, __pyx_n_u_lock, __pyx_t_1) < 0)) __PYX_ERR(0, 2798, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "pyrfc/_cyrfc.pyx":2799
  *     unit_attributes['unit_history'] = uattr.unitHistory != 0
  *     unit_attributes['lock'] = uattr.lock != 0
  *     unit_attributes['no_commit_check'] = uattr.noCommitCheck != 0             # <<<<<<<<<<<<<<
  *     unit_attributes['user'] = wrapString(uattr.user, 12, True)
  *     unit_attributes['client'] = wrapString(uattr.client, 3, True)
  */
   __pyx_t_1 = __Pyx_PyBool_FromLong((__pyx_v_uattr->noCommitCheck != 0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2799, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (unlikely(PyDict_SetItem(__pyx_v_unit_attributes, __pyx_n_s_no_commit_check, __pyx_t_1) < 0)) __PYX_ERR(0, 2799, __pyx_L1_error)
+  if (unlikely(PyDict_SetItem(__pyx_v_unit_attributes, __pyx_n_u_no_commit_check, __pyx_t_1) < 0)) __PYX_ERR(0, 2799, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "pyrfc/_cyrfc.pyx":2800
  *     unit_attributes['lock'] = uattr.lock != 0
  *     unit_attributes['no_commit_check'] = uattr.noCommitCheck != 0
  *     unit_attributes['user'] = wrapString(uattr.user, 12, True)             # <<<<<<<<<<<<<<
  *     unit_attributes['client'] = wrapString(uattr.client, 3, True)
  *     unit_attributes['t_code'] = wrapString(uattr.tCode, 20, True)
  */
   __pyx_t_2.__pyx_n = 2;
   __pyx_t_2.uclen = __pyx_int_12;
   __pyx_t_2.rstrip = Py_True;
   __pyx_t_1 = __pyx_f_5pyrfc_6_cyrfc_wrapString(__pyx_v_uattr->user, &__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2800, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (unlikely(PyDict_SetItem(__pyx_v_unit_attributes, __pyx_n_s_user, __pyx_t_1) < 0)) __PYX_ERR(0, 2800, __pyx_L1_error)
+  if (unlikely(PyDict_SetItem(__pyx_v_unit_attributes, __pyx_n_u_user, __pyx_t_1) < 0)) __PYX_ERR(0, 2800, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "pyrfc/_cyrfc.pyx":2801
  *     unit_attributes['no_commit_check'] = uattr.noCommitCheck != 0
  *     unit_attributes['user'] = wrapString(uattr.user, 12, True)
  *     unit_attributes['client'] = wrapString(uattr.client, 3, True)             # <<<<<<<<<<<<<<
  *     unit_attributes['t_code'] = wrapString(uattr.tCode, 20, True)
  *     unit_attributes['program'] = wrapString(uattr.program, 40, True)
  */
   __pyx_t_2.__pyx_n = 2;
   __pyx_t_2.uclen = __pyx_int_3;
   __pyx_t_2.rstrip = Py_True;
   __pyx_t_1 = __pyx_f_5pyrfc_6_cyrfc_wrapString(__pyx_v_uattr->client, &__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2801, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (unlikely(PyDict_SetItem(__pyx_v_unit_attributes, __pyx_n_s_client, __pyx_t_1) < 0)) __PYX_ERR(0, 2801, __pyx_L1_error)
+  if (unlikely(PyDict_SetItem(__pyx_v_unit_attributes, __pyx_n_u_client, __pyx_t_1) < 0)) __PYX_ERR(0, 2801, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "pyrfc/_cyrfc.pyx":2802
  *     unit_attributes['user'] = wrapString(uattr.user, 12, True)
  *     unit_attributes['client'] = wrapString(uattr.client, 3, True)
  *     unit_attributes['t_code'] = wrapString(uattr.tCode, 20, True)             # <<<<<<<<<<<<<<
  *     unit_attributes['program'] = wrapString(uattr.program, 40, True)
  *     unit_attributes['hostname'] = wrapString(uattr.hostname, 40, True)
  */
   __pyx_t_2.__pyx_n = 2;
   __pyx_t_2.uclen = __pyx_int_20;
   __pyx_t_2.rstrip = Py_True;
   __pyx_t_1 = __pyx_f_5pyrfc_6_cyrfc_wrapString(__pyx_v_uattr->tCode, &__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2802, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (unlikely(PyDict_SetItem(__pyx_v_unit_attributes, __pyx_n_s_t_code, __pyx_t_1) < 0)) __PYX_ERR(0, 2802, __pyx_L1_error)
+  if (unlikely(PyDict_SetItem(__pyx_v_unit_attributes, __pyx_n_u_t_code, __pyx_t_1) < 0)) __PYX_ERR(0, 2802, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "pyrfc/_cyrfc.pyx":2803
  *     unit_attributes['client'] = wrapString(uattr.client, 3, True)
  *     unit_attributes['t_code'] = wrapString(uattr.tCode, 20, True)
  *     unit_attributes['program'] = wrapString(uattr.program, 40, True)             # <<<<<<<<<<<<<<
  *     unit_attributes['hostname'] = wrapString(uattr.hostname, 40, True)
  *     unit_attributes['sending_date'] = wrapString(uattr.sendingDate, 8, True)
  */
   __pyx_t_2.__pyx_n = 2;
   __pyx_t_2.uclen = __pyx_int_40;
   __pyx_t_2.rstrip = Py_True;
   __pyx_t_1 = __pyx_f_5pyrfc_6_cyrfc_wrapString(__pyx_v_uattr->program, &__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2803, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (unlikely(PyDict_SetItem(__pyx_v_unit_attributes, __pyx_n_s_program, __pyx_t_1) < 0)) __PYX_ERR(0, 2803, __pyx_L1_error)
+  if (unlikely(PyDict_SetItem(__pyx_v_unit_attributes, __pyx_n_u_program, __pyx_t_1) < 0)) __PYX_ERR(0, 2803, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "pyrfc/_cyrfc.pyx":2804
  *     unit_attributes['t_code'] = wrapString(uattr.tCode, 20, True)
  *     unit_attributes['program'] = wrapString(uattr.program, 40, True)
  *     unit_attributes['hostname'] = wrapString(uattr.hostname, 40, True)             # <<<<<<<<<<<<<<
  *     unit_attributes['sending_date'] = wrapString(uattr.sendingDate, 8, True)
  *     unit_attributes['sending_time'] = wrapString(uattr.sendingTime, 6, True)
  */
   __pyx_t_2.__pyx_n = 2;
   __pyx_t_2.uclen = __pyx_int_40;
   __pyx_t_2.rstrip = Py_True;
   __pyx_t_1 = __pyx_f_5pyrfc_6_cyrfc_wrapString(__pyx_v_uattr->hostname, &__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2804, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (unlikely(PyDict_SetItem(__pyx_v_unit_attributes, __pyx_n_s_hostname, __pyx_t_1) < 0)) __PYX_ERR(0, 2804, __pyx_L1_error)
+  if (unlikely(PyDict_SetItem(__pyx_v_unit_attributes, __pyx_n_u_hostname, __pyx_t_1) < 0)) __PYX_ERR(0, 2804, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "pyrfc/_cyrfc.pyx":2805
  *     unit_attributes['program'] = wrapString(uattr.program, 40, True)
  *     unit_attributes['hostname'] = wrapString(uattr.hostname, 40, True)
  *     unit_attributes['sending_date'] = wrapString(uattr.sendingDate, 8, True)             # <<<<<<<<<<<<<<
  *     unit_attributes['sending_time'] = wrapString(uattr.sendingTime, 6, True)
  *     return unit_attributes
  */
   __pyx_t_2.__pyx_n = 2;
   __pyx_t_2.uclen = __pyx_int_8;
   __pyx_t_2.rstrip = Py_True;
   __pyx_t_1 = __pyx_f_5pyrfc_6_cyrfc_wrapString(__pyx_v_uattr->sendingDate, &__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2805, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (unlikely(PyDict_SetItem(__pyx_v_unit_attributes, __pyx_n_s_sending_date, __pyx_t_1) < 0)) __PYX_ERR(0, 2805, __pyx_L1_error)
+  if (unlikely(PyDict_SetItem(__pyx_v_unit_attributes, __pyx_n_u_sending_date, __pyx_t_1) < 0)) __PYX_ERR(0, 2805, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "pyrfc/_cyrfc.pyx":2806
  *     unit_attributes['hostname'] = wrapString(uattr.hostname, 40, True)
  *     unit_attributes['sending_date'] = wrapString(uattr.sendingDate, 8, True)
  *     unit_attributes['sending_time'] = wrapString(uattr.sendingTime, 6, True)             # <<<<<<<<<<<<<<
  *     return unit_attributes
  * 
  */
   __pyx_t_2.__pyx_n = 2;
   __pyx_t_2.uclen = __pyx_int_6;
   __pyx_t_2.rstrip = Py_True;
   __pyx_t_1 = __pyx_f_5pyrfc_6_cyrfc_wrapString(__pyx_v_uattr->sendingTime, &__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2806, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (unlikely(PyDict_SetItem(__pyx_v_unit_attributes, __pyx_n_s_sending_time, __pyx_t_1) < 0)) __PYX_ERR(0, 2806, __pyx_L1_error)
+  if (unlikely(PyDict_SetItem(__pyx_v_unit_attributes, __pyx_n_u_sending_time, __pyx_t_1) < 0)) __PYX_ERR(0, 2806, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "pyrfc/_cyrfc.pyx":2807
  *     unit_attributes['sending_date'] = wrapString(uattr.sendingDate, 8, True)
  *     unit_attributes['sending_time'] = wrapString(uattr.sendingTime, 6, True)
  *     return unit_attributes             # <<<<<<<<<<<<<<
  * 
@@ -36405,26 +37142,26 @@
     /* "pyrfc/_cyrfc.pyx":2825
  *             )
  *     if len(result) == 1:
  *         if '' in result:             # <<<<<<<<<<<<<<
  *             result = result['']
  *     return result
  */
-    __pyx_t_7 = (__Pyx_PySequence_ContainsTF(__pyx_kp_s__5, __pyx_v_result, Py_EQ)); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 2825, __pyx_L1_error)
+    __pyx_t_7 = (__Pyx_PySequence_ContainsTF(__pyx_kp_u__5, __pyx_v_result, Py_EQ)); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 2825, __pyx_L1_error)
     __pyx_t_8 = (__pyx_t_7 != 0);
     if (__pyx_t_8) {
 
       /* "pyrfc/_cyrfc.pyx":2826
  *     if len(result) == 1:
  *         if '' in result:
  *             result = result['']             # <<<<<<<<<<<<<<
  *     return result
  * 
  */
-      __pyx_t_1 = __Pyx_PyDict_GetItem(__pyx_v_result, __pyx_kp_s__5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2826, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyDict_GetItem(__pyx_v_result, __pyx_kp_u__5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2826, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF_SET(__pyx_v_result, __pyx_t_1);
       __pyx_t_1 = 0;
 
       /* "pyrfc/_cyrfc.pyx":2825
  *             )
  *     if len(result) == 1:
@@ -36659,14 +37396,16 @@
   PyObject *__pyx_t_19 = NULL;
   char const *__pyx_t_20;
   char const *__pyx_t_21;
   char const *__pyx_t_22;
   int __pyx_t_23;
   int __pyx_t_24;
   PyObject *__pyx_t_25 = NULL;
+  Py_ssize_t __pyx_t_26;
+  Py_UCS4 __pyx_t_27;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("wrapVariable", 0);
 
   /* "pyrfc/_cyrfc.pyx":2881
  *     cdef RFC_TIME timeValue
@@ -38416,20 +39155,20 @@
  *             utcValue = wrapString(stringValue, resultLen)
  *             # replace the "," separator with "."
  *             return utcValue[:19]+'.'+utcValue[20:]             # <<<<<<<<<<<<<<
  *         finally:
  *             free(stringValue)
  */
       __Pyx_XDECREF(__pyx_r);
-      __pyx_t_4 = __Pyx_PyObject_GetSlice(__pyx_v_utcValue, 0, 19, NULL, NULL, &__pyx_slice__46, 0, 1, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3021, __pyx_L55_error)
+      __pyx_t_4 = __Pyx_PyObject_GetSlice(__pyx_v_utcValue, 0, 19, NULL, NULL, &__pyx_slice__47, 0, 1, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3021, __pyx_L55_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_3 = PyNumber_Add(__pyx_t_4, __pyx_kp_s__20); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3021, __pyx_L55_error)
+      __pyx_t_3 = PyNumber_Add(__pyx_t_4, __pyx_kp_u__21); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3021, __pyx_L55_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_4 = __Pyx_PyObject_GetSlice(__pyx_v_utcValue, 20, 0, NULL, NULL, &__pyx_slice__47, 1, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3021, __pyx_L55_error)
+      __pyx_t_4 = __Pyx_PyObject_GetSlice(__pyx_v_utcValue, 20, 0, NULL, NULL, &__pyx_slice__48, 1, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3021, __pyx_L55_error)
       __Pyx_GOTREF(__pyx_t_4);
       __pyx_t_2 = PyNumber_Add(__pyx_t_3, __pyx_t_4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 3021, __pyx_L55_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __pyx_r = __pyx_t_2;
       __pyx_t_2 = 0;
@@ -38573,15 +39312,15 @@
       /* "pyrfc/_cyrfc.pyx":3031
  *         # return date or None
  *         if config & _MASK_DTIME:
  *             if (value == '00000000') or not value:             # <<<<<<<<<<<<<<
  *                 return None
  *             return datetime.strptime(value, '%Y%m%d').date()
  */
-      __pyx_t_23 = (__Pyx_PyString_Equals(__pyx_v_value, __pyx_kp_s_00000000, Py_EQ)); if (unlikely(__pyx_t_23 < 0)) __PYX_ERR(0, 3031, __pyx_L1_error)
+      __pyx_t_23 = (__Pyx_PyUnicode_Equals(__pyx_v_value, __pyx_kp_u_00000000, Py_EQ)); if (unlikely(__pyx_t_23 < 0)) __PYX_ERR(0, 3031, __pyx_L1_error)
       if (!__pyx_t_23) {
       } else {
         __pyx_t_1 = __pyx_t_23;
         goto __pyx_L63_bool_binop_done;
       }
       __pyx_t_23 = __Pyx_PyObject_IsTrue(__pyx_v_value); if (unlikely(__pyx_t_23 < 0)) __PYX_ERR(0, 3031, __pyx_L1_error)
       __pyx_t_24 = ((!__pyx_t_23) != 0);
@@ -38632,40 +39371,40 @@
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_19, function);
           __pyx_t_6 = 1;
         }
       }
       #if CYTHON_FAST_PYCALL
       if (PyFunction_Check(__pyx_t_19)) {
-        PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_v_value, __pyx_kp_s_Y_m_d};
+        PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_v_value, __pyx_kp_u_Y_m_d};
         __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_19, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 3033, __pyx_L1_error)
         __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
         __Pyx_GOTREF(__pyx_t_2);
       } else
       #endif
       #if CYTHON_FAST_PYCCALL
       if (__Pyx_PyFastCFunction_Check(__pyx_t_19)) {
-        PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_v_value, __pyx_kp_s_Y_m_d};
+        PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_v_value, __pyx_kp_u_Y_m_d};
         __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_19, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 3033, __pyx_L1_error)
         __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
         __Pyx_GOTREF(__pyx_t_2);
       } else
       #endif
       {
         __pyx_t_25 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_25)) __PYX_ERR(0, 3033, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_25);
         if (__pyx_t_3) {
           __Pyx_GIVEREF(__pyx_t_3); PyTuple_SET_ITEM(__pyx_t_25, 0, __pyx_t_3); __pyx_t_3 = NULL;
         }
         __Pyx_INCREF(__pyx_v_value);
         __Pyx_GIVEREF(__pyx_v_value);
         PyTuple_SET_ITEM(__pyx_t_25, 0+__pyx_t_6, __pyx_v_value);
-        __Pyx_INCREF(__pyx_kp_s_Y_m_d);
-        __Pyx_GIVEREF(__pyx_kp_s_Y_m_d);
-        PyTuple_SET_ITEM(__pyx_t_25, 1+__pyx_t_6, __pyx_kp_s_Y_m_d);
+        __Pyx_INCREF(__pyx_kp_u_Y_m_d);
+        __Pyx_GIVEREF(__pyx_kp_u_Y_m_d);
+        PyTuple_SET_ITEM(__pyx_t_25, 1+__pyx_t_6, __pyx_kp_u_Y_m_d);
         __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_19, __pyx_t_25, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 3033, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_25); __pyx_t_25 = 0;
       }
       __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
       __pyx_t_19 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_date); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 3033, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_19);
@@ -38701,15 +39440,15 @@
     /* "pyrfc/_cyrfc.pyx":3035
  *             return datetime.strptime(value, '%Y%m%d').date()
  *         # return date string or ''
  *         if (value == '00000000') or not value:             # <<<<<<<<<<<<<<
  *             return ''
  *         return value
  */
-    __pyx_t_24 = (__Pyx_PyString_Equals(__pyx_v_value, __pyx_kp_s_00000000, Py_EQ)); if (unlikely(__pyx_t_24 < 0)) __PYX_ERR(0, 3035, __pyx_L1_error)
+    __pyx_t_24 = (__Pyx_PyUnicode_Equals(__pyx_v_value, __pyx_kp_u_00000000, Py_EQ)); if (unlikely(__pyx_t_24 < 0)) __PYX_ERR(0, 3035, __pyx_L1_error)
     if (!__pyx_t_24) {
     } else {
       __pyx_t_1 = __pyx_t_24;
       goto __pyx_L66_bool_binop_done;
     }
     __pyx_t_24 = __Pyx_PyObject_IsTrue(__pyx_v_value); if (unlikely(__pyx_t_24 < 0)) __PYX_ERR(0, 3035, __pyx_L1_error)
     __pyx_t_23 = ((!__pyx_t_24) != 0);
@@ -38721,16 +39460,16 @@
  *         # return date string or ''
  *         if (value == '00000000') or not value:
  *             return ''             # <<<<<<<<<<<<<<
  *         return value
  *     elif typ == RFCTYPE_TIME:
  */
       __Pyx_XDECREF(__pyx_r);
-      __Pyx_INCREF(__pyx_kp_s__5);
-      __pyx_r = __pyx_kp_s__5;
+      __Pyx_INCREF(__pyx_kp_u__5);
+      __pyx_r = __pyx_kp_u__5;
       goto __pyx_L0;
 
       /* "pyrfc/_cyrfc.pyx":3035
  *             return datetime.strptime(value, '%Y%m%d').date()
  *         # return date string or ''
  *         if (value == '00000000') or not value:             # <<<<<<<<<<<<<<
  *             return ''
@@ -38885,40 +39624,40 @@
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_25, function);
           __pyx_t_6 = 1;
         }
       }
       #if CYTHON_FAST_PYCALL
       if (PyFunction_Check(__pyx_t_25)) {
-        PyObject *__pyx_temp[3] = {__pyx_t_2, __pyx_v_value, __pyx_kp_s_H_M_S};
+        PyObject *__pyx_temp[3] = {__pyx_t_2, __pyx_v_value, __pyx_kp_u_H_M_S};
         __pyx_t_4 = __Pyx_PyFunction_FastCall(__pyx_t_25, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3047, __pyx_L1_error)
         __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
         __Pyx_GOTREF(__pyx_t_4);
       } else
       #endif
       #if CYTHON_FAST_PYCCALL
       if (__Pyx_PyFastCFunction_Check(__pyx_t_25)) {
-        PyObject *__pyx_temp[3] = {__pyx_t_2, __pyx_v_value, __pyx_kp_s_H_M_S};
+        PyObject *__pyx_temp[3] = {__pyx_t_2, __pyx_v_value, __pyx_kp_u_H_M_S};
         __pyx_t_4 = __Pyx_PyCFunction_FastCall(__pyx_t_25, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3047, __pyx_L1_error)
         __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
         __Pyx_GOTREF(__pyx_t_4);
       } else
       #endif
       {
         __pyx_t_3 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3047, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         if (__pyx_t_2) {
           __Pyx_GIVEREF(__pyx_t_2); PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_2); __pyx_t_2 = NULL;
         }
         __Pyx_INCREF(__pyx_v_value);
         __Pyx_GIVEREF(__pyx_v_value);
         PyTuple_SET_ITEM(__pyx_t_3, 0+__pyx_t_6, __pyx_v_value);
-        __Pyx_INCREF(__pyx_kp_s_H_M_S);
-        __Pyx_GIVEREF(__pyx_kp_s_H_M_S);
-        PyTuple_SET_ITEM(__pyx_t_3, 1+__pyx_t_6, __pyx_kp_s_H_M_S);
+        __Pyx_INCREF(__pyx_kp_u_H_M_S);
+        __Pyx_GIVEREF(__pyx_kp_u_H_M_S);
+        PyTuple_SET_ITEM(__pyx_t_3, 1+__pyx_t_6, __pyx_kp_u_H_M_S);
         __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_25, __pyx_t_3, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3047, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       }
       __Pyx_DECREF(__pyx_t_25); __pyx_t_25 = 0;
       __pyx_t_25 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_time); if (unlikely(!__pyx_t_25)) __PYX_ERR(0, 3047, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_25);
@@ -38966,16 +39705,16 @@
  *         # return time string or ''
  *         if not value:
  *             return ''             # <<<<<<<<<<<<<<
  *         return value
  *     else:
  */
       __Pyx_XDECREF(__pyx_r);
-      __Pyx_INCREF(__pyx_kp_s__5);
-      __pyx_r = __pyx_kp_s__5;
+      __Pyx_INCREF(__pyx_kp_u__5);
+      __pyx_r = __pyx_kp_u__5;
       goto __pyx_L0;
 
       /* "pyrfc/_cyrfc.pyx":3049
  *             return datetime.strptime(value, '%H%M%S').time()
  *         # return time string or ''
  *         if not value:             # <<<<<<<<<<<<<<
  *             return ''
@@ -39010,42 +39749,59 @@
  *     else:
  *         raise RFCError('Unknown RFC type %d when wrapping %s' % (typ, wrapString(cName)))             # <<<<<<<<<<<<<<
  * 
  * cdef wrapError(RFC_ERROR_INFO* errorInfo):
  */
     __Pyx_GetModuleGlobalName(__pyx_t_25, __pyx_n_s_RFCError); if (unlikely(!__pyx_t_25)) __PYX_ERR(0, 3053, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_25);
-    __pyx_t_4 = __Pyx_PyInt_From_RFCTYPE(__pyx_v_typ); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3053, __pyx_L1_error)
+    __pyx_t_4 = PyTuple_New(4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3053, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_3 = __pyx_f_5pyrfc_6_cyrfc_wrapString(__pyx_v_cName, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3053, __pyx_L1_error)
+    __pyx_t_26 = 0;
+    __pyx_t_27 = 127;
+    __Pyx_INCREF(__pyx_kp_u_Unknown_RFC_type);
+    __pyx_t_26 += 17;
+    __Pyx_GIVEREF(__pyx_kp_u_Unknown_RFC_type);
+    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_kp_u_Unknown_RFC_type);
+    __pyx_t_3 = __Pyx_PyUnicode_From_RFCTYPE(__pyx_v_typ, 0, ' ', 'd'); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3053, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 3053, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_GIVEREF(__pyx_t_4);
-    PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_4);
+    __pyx_t_27 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_3) > __pyx_t_27) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_3) : __pyx_t_27;
+    __pyx_t_26 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_3);
     __Pyx_GIVEREF(__pyx_t_3);
-    PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_t_3);
-    __pyx_t_4 = 0;
+    PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_3);
     __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyString_Format(__pyx_kp_s_Unknown_RFC_type_d_when_wrapping, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3053, __pyx_L1_error)
+    __Pyx_INCREF(__pyx_kp_u_when_wrapping);
+    __pyx_t_26 += 15;
+    __Pyx_GIVEREF(__pyx_kp_u_when_wrapping);
+    PyTuple_SET_ITEM(__pyx_t_4, 2, __pyx_kp_u_when_wrapping);
+    __pyx_t_3 = __pyx_f_5pyrfc_6_cyrfc_wrapString(__pyx_v_cName, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3053, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = NULL;
+    __pyx_t_2 = __Pyx_PyObject_FormatSimpleAndDecref(PyObject_Unicode(__pyx_t_3), __pyx_empty_unicode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 3053, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __pyx_t_27 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_2) > __pyx_t_27) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_2) : __pyx_t_27;
+    __pyx_t_26 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_2);
+    __Pyx_GIVEREF(__pyx_t_2);
+    PyTuple_SET_ITEM(__pyx_t_4, 3, __pyx_t_2);
+    __pyx_t_2 = 0;
+    __pyx_t_2 = __Pyx_PyUnicode_Join(__pyx_t_4, 4, __pyx_t_26, __pyx_t_27); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 3053, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __pyx_t_4 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_25))) {
-      __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_25);
-      if (likely(__pyx_t_2)) {
+      __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_25);
+      if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_25);
-        __Pyx_INCREF(__pyx_t_2);
+        __Pyx_INCREF(__pyx_t_4);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_25, function);
       }
     }
-    __pyx_t_19 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_25, __pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_25, __pyx_t_3);
-    __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __pyx_t_19 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_25, __pyx_t_4, __pyx_t_2) : __Pyx_PyObject_CallOneArg(__pyx_t_25, __pyx_t_2);
+    __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 3053, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_19);
     __Pyx_DECREF(__pyx_t_25); __pyx_t_25 = 0;
     __Pyx_Raise(__pyx_t_19, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
     __PYX_ERR(0, 3053, __pyx_L1_error)
     break;
@@ -39519,16 +40275,16 @@
  *         uclen = strlenU(uc)
  *     if uclen == 0:
  *         return ''             # <<<<<<<<<<<<<<
  *     cdef unsigned utf8_size = uclen * 5 + 1
  *     cdef char *utf8 = <char*> malloc(utf8_size)
  */
     __Pyx_XDECREF(__pyx_r);
-    __Pyx_INCREF(__pyx_kp_s__5);
-    __pyx_r = __pyx_kp_s__5;
+    __Pyx_INCREF(__pyx_kp_u__5);
+    __pyx_r = __pyx_kp_u__5;
     goto __pyx_L0;
 
     /* "pyrfc/_cyrfc.pyx":3078
  *     if uclen == -1:
  *         uclen = strlenU(uc)
  *     if uclen == 0:             # <<<<<<<<<<<<<<
  *         return ''
@@ -39614,15 +40370,15 @@
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_INCREF(__pyx_v_uclen);
     __Pyx_GIVEREF(__pyx_v_uclen);
     PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_v_uclen);
     __Pyx_GIVEREF(__pyx_t_5);
     PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_t_5);
     __pyx_t_5 = 0;
-    __pyx_t_5 = __Pyx_PyString_Format(__pyx_kp_s_wrapString_uclen_u_utf8_size_u, __pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3087, __pyx_L1_error)
+    __pyx_t_5 = PyUnicode_Format(__pyx_kp_u_wrapString_uclen_u_utf8_size_u, __pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3087, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __pyx_t_6 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
       __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_1);
       if (likely(__pyx_t_6)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
@@ -39928,16 +40684,16 @@
  *         uclen = strlenU(uc)
  *     if uclen == 0:
  *         return ''             # <<<<<<<<<<<<<<
  *     cdef unsigned utf8_size = uclen * 5 + 1
  *     cdef char *utf8 = <char*> malloc(utf8_size)
  */
     __Pyx_XDECREF(__pyx_r);
-    __Pyx_INCREF(__pyx_kp_s__5);
-    __pyx_r = __pyx_kp_s__5;
+    __Pyx_INCREF(__pyx_kp_u__5);
+    __pyx_r = __pyx_kp_u__5;
     goto __pyx_L0;
 
     /* "pyrfc/_cyrfc.pyx":3102
  *     if uclen == -1:
  *         uclen = strlenU(uc)
  *     if uclen == 0:             # <<<<<<<<<<<<<<
  *         return ''
@@ -40023,15 +40779,15 @@
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_INCREF(__pyx_v_uclen);
     __Pyx_GIVEREF(__pyx_v_uclen);
     PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_v_uclen);
     __Pyx_GIVEREF(__pyx_t_5);
     PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_t_5);
     __pyx_t_5 = 0;
-    __pyx_t_5 = __Pyx_PyString_Format(__pyx_kp_s_wrapString_uclen_u_utf8_size_u, __pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3111, __pyx_L1_error)
+    __pyx_t_5 = PyUnicode_Format(__pyx_kp_u_wrapString_uclen_u_utf8_size_u, __pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3111, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __pyx_t_6 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
       __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_1);
       if (likely(__pyx_t_6)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
@@ -40337,15 +41093,15 @@
   /* "cfunc.to_py":65
  * @cname("__Pyx_CFunc_object____object___to_py")
  * cdef object __Pyx_CFunc_object____object___to_py(object (*f)(object) ):
  *     def wrap(object client_connection):             # <<<<<<<<<<<<<<
  *         """wrap(client_connection)"""
  *         return f(client_connection)
  */
-  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_11cfunc_dot_to_py_36__Pyx_CFunc_object____object___to_py_1wrap, 0, __pyx_n_s_Pyx_CFunc_object____object___t, ((PyObject*)__pyx_cur_scope), __pyx_n_s_cfunc_to_py, __pyx_d, ((PyObject *)__pyx_codeobj__49)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 65, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_11cfunc_dot_to_py_36__Pyx_CFunc_object____object___to_py_1wrap, 0, __pyx_n_s_Pyx_CFunc_object____object___t, ((PyObject*)__pyx_cur_scope), __pyx_n_s_cfunc_to_py, __pyx_d, ((PyObject *)__pyx_codeobj__50)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 65, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_wrap = __pyx_t_1;
   __pyx_t_1 = 0;
 
   /* "cfunc.to_py":68
  *         """wrap(client_connection)"""
  *         return f(client_connection)
@@ -41663,81 +42419,81 @@
     #define CYTHON_SMALL_CODE __attribute__((cold))
 #else
     #define CYTHON_SMALL_CODE
 #endif
 #endif
 
 static __Pyx_StringTabEntry __pyx_string_tab[] = {
-  {&__pyx_kp_s_00000000, __pyx_k_00000000, sizeof(__pyx_k_00000000), 0, 0, 1, 0},
+  {&__pyx_kp_u_00000000, __pyx_k_00000000, sizeof(__pyx_k_00000000), 0, 1, 0, 0},
   {&__pyx_kp_u_02, __pyx_k_02, sizeof(__pyx_k_02), 0, 1, 0, 0},
   {&__pyx_kp_u_04, __pyx_k_04, sizeof(__pyx_k_04), 0, 1, 0, 0},
   {&__pyx_n_s_ABAPApplicationError, __pyx_k_ABAPApplicationError, sizeof(__pyx_k_ABAPApplicationError), 0, 0, 1, 1},
   {&__pyx_n_s_ABAPRuntimeError, __pyx_k_ABAPRuntimeError, sizeof(__pyx_k_ABAPRuntimeError), 0, 0, 1, 1},
   {&__pyx_kp_s_A_function_description_This_cla, __pyx_k_A_function_description_This_cla, sizeof(__pyx_k_A_function_description_This_cla), 0, 0, 1, 0},
   {&__pyx_kp_s_A_type_description_This_class_w, __pyx_k_A_type_description_This_class_w, sizeof(__pyx_k_A_type_description_This_class_w), 0, 0, 1, 0},
-  {&__pyx_kp_s_Argument_attributes_not_valid_t, __pyx_k_Argument_attributes_not_valid_t, sizeof(__pyx_k_Argument_attributes_not_valid_t), 0, 0, 1, 0},
-  {&__pyx_kp_s_Argument_background_must_be_a_bo, __pyx_k_Argument_background_must_be_a_bo, sizeof(__pyx_k_Argument_background_must_be_a_bo), 0, 0, 1, 0},
-  {&__pyx_kp_s_Argument_queue_names_not_valid_t, __pyx_k_Argument_queue_names_not_valid_t, sizeof(__pyx_k_Argument_queue_names_not_valid_t), 0, 0, 1, 0},
-  {&__pyx_kp_s_Argument_unit_not_valid_Is_unit, __pyx_k_Argument_unit_not_valid_Is_unit, sizeof(__pyx_k_Argument_unit_not_valid_Is_unit), 0, 0, 1, 0},
+  {&__pyx_kp_u_Argument_attributes_not_valid_t, __pyx_k_Argument_attributes_not_valid_t, sizeof(__pyx_k_Argument_attributes_not_valid_t), 0, 1, 0, 0},
+  {&__pyx_kp_u_Argument_background_must_be_a_bo, __pyx_k_Argument_background_must_be_a_bo, sizeof(__pyx_k_Argument_background_must_be_a_bo), 0, 1, 0, 0},
+  {&__pyx_kp_u_Argument_queue_names_not_valid_t, __pyx_k_Argument_queue_names_not_valid_t, sizeof(__pyx_k_Argument_queue_names_not_valid_t), 0, 1, 0, 0},
+  {&__pyx_kp_u_Argument_unit_not_valid_Is_unit, __pyx_k_Argument_unit_not_valid_Is_unit, sizeof(__pyx_k_Argument_unit_not_valid_Is_unit), 0, 1, 0, 0},
   {&__pyx_kp_u_Authentication_exception_raised, __pyx_k_Authentication_exception_raised, sizeof(__pyx_k_Authentication_exception_raised), 0, 1, 0, 0},
   {&__pyx_kp_u_BgRfc_callback_function_key_not, __pyx_k_BgRfc_callback_function_key_not, sizeof(__pyx_k_BgRfc_callback_function_key_not), 0, 1, 0, 0},
   {&__pyx_kp_u_BgRfc_callback_function_referenc, __pyx_k_BgRfc_callback_function_referenc, sizeof(__pyx_k_BgRfc_callback_function_referenc), 0, 1, 0, 0},
   {&__pyx_kp_u_Callback_functions_may_only_rai, __pyx_k_Callback_functions_may_only_rai, sizeof(__pyx_k_Callback_functions_may_only_rai), 0, 1, 0, 0},
   {&__pyx_n_s_CommunicationError, __pyx_k_CommunicationError, sizeof(__pyx_k_CommunicationError), 0, 0, 1, 1},
   {&__pyx_n_s_Connection, __pyx_k_Connection, sizeof(__pyx_k_Connection), 0, 0, 1, 1},
   {&__pyx_n_s_ConnectionParameters, __pyx_k_ConnectionParameters, sizeof(__pyx_k_ConnectionParameters), 0, 0, 1, 1},
   {&__pyx_kp_u_Connection_configuration_option, __pyx_k_Connection_configuration_option, sizeof(__pyx_k_Connection_configuration_option), 0, 1, 0, 0},
-  {&__pyx_kp_s_Connection_object_required_recei, __pyx_k_Connection_object_required_recei, sizeof(__pyx_k_Connection_object_required_recei), 0, 0, 1, 0},
-  {&__pyx_kp_s_Connection_parameters_missing, __pyx_k_Connection_parameters_missing, sizeof(__pyx_k_Connection_parameters_missing), 0, 0, 1, 0},
+  {&__pyx_kp_u_Connection_object_required_recei, __pyx_k_Connection_object_required_recei, sizeof(__pyx_k_Connection_object_required_recei), 0, 1, 0, 0},
+  {&__pyx_kp_u_Connection_parameters_missing, __pyx_k_Connection_parameters_missing, sizeof(__pyx_k_Connection_parameters_missing), 0, 1, 0, 0},
   {&__pyx_kp_u_Connection_was_canceled, __pyx_k_Connection_was_canceled, sizeof(__pyx_k_Connection_was_canceled), 0, 1, 0, 0},
-  {&__pyx_kp_s_Crypto_library_not_found, __pyx_k_Crypto_library_not_found, sizeof(__pyx_k_Crypto_library_not_found), 0, 0, 1, 0},
+  {&__pyx_kp_u_Crypto_library_not_found, __pyx_k_Crypto_library_not_found, sizeof(__pyx_k_Crypto_library_not_found), 0, 1, 0, 0},
   {&__pyx_n_s_Decimal, __pyx_k_Decimal, sizeof(__pyx_k_Decimal), 0, 0, 1, 1},
   {&__pyx_n_s_Enum, __pyx_k_Enum, sizeof(__pyx_k_Enum), 0, 0, 1, 1},
   {&__pyx_kp_u_Error_code, __pyx_k_Error_code, sizeof(__pyx_k_Error_code), 0, 1, 0, 0},
-  {&__pyx_kp_s_Error_in_bgRFC_handler_onCheck, __pyx_k_Error_in_bgRFC_handler_onCheck, sizeof(__pyx_k_Error_in_bgRFC_handler_onCheck), 0, 0, 1, 0},
-  {&__pyx_kp_s_Error_in_bgRFC_handler_onCommit, __pyx_k_Error_in_bgRFC_handler_onCommit, sizeof(__pyx_k_Error_in_bgRFC_handler_onCommit), 0, 0, 1, 0},
-  {&__pyx_kp_s_Error_in_bgRFC_handler_onConfirm, __pyx_k_Error_in_bgRFC_handler_onConfirm, sizeof(__pyx_k_Error_in_bgRFC_handler_onConfirm), 0, 0, 1, 0},
-  {&__pyx_kp_s_Error_in_bgRFC_handler_onGetStat, __pyx_k_Error_in_bgRFC_handler_onGetStat, sizeof(__pyx_k_Error_in_bgRFC_handler_onGetStat), 0, 0, 1, 0},
-  {&__pyx_kp_s_Error_in_bgRFC_handler_onRollbac, __pyx_k_Error_in_bgRFC_handler_onRollbac, sizeof(__pyx_k_Error_in_bgRFC_handler_onRollbac), 0, 0, 1, 0},
+  {&__pyx_kp_u_Error_in_bgRFC_handler_onCheck, __pyx_k_Error_in_bgRFC_handler_onCheck, sizeof(__pyx_k_Error_in_bgRFC_handler_onCheck), 0, 1, 0, 0},
+  {&__pyx_kp_u_Error_in_bgRFC_handler_onCommit, __pyx_k_Error_in_bgRFC_handler_onCommit, sizeof(__pyx_k_Error_in_bgRFC_handler_onCommit), 0, 1, 0, 0},
+  {&__pyx_kp_u_Error_in_bgRFC_handler_onConfirm, __pyx_k_Error_in_bgRFC_handler_onConfirm, sizeof(__pyx_k_Error_in_bgRFC_handler_onConfirm), 0, 1, 0, 0},
+  {&__pyx_kp_u_Error_in_bgRFC_handler_onGetStat, __pyx_k_Error_in_bgRFC_handler_onGetStat, sizeof(__pyx_k_Error_in_bgRFC_handler_onGetStat), 0, 1, 0, 0},
+  {&__pyx_kp_u_Error_in_bgRFC_handler_onRollbac, __pyx_k_Error_in_bgRFC_handler_onRollbac, sizeof(__pyx_k_Error_in_bgRFC_handler_onRollbac), 0, 1, 0, 0},
   {&__pyx_kp_u_Error_while_retrieving_connecti, __pyx_k_Error_while_retrieving_connecti, sizeof(__pyx_k_Error_while_retrieving_connecti), 0, 1, 0, 0},
   {&__pyx_n_s_ExternalApplicationError, __pyx_k_ExternalApplicationError, sizeof(__pyx_k_ExternalApplicationError), 0, 0, 1, 1},
   {&__pyx_n_s_ExternalAuthorizationError, __pyx_k_ExternalAuthorizationError, sizeof(__pyx_k_ExternalAuthorizationError), 0, 0, 1, 1},
   {&__pyx_n_s_ExternalRuntimeError, __pyx_k_ExternalRuntimeError, sizeof(__pyx_k_ExternalRuntimeError), 0, 0, 1, 1},
   {&__pyx_kp_u_Function, __pyx_k_Function, sizeof(__pyx_k_Function), 0, 1, 0, 0},
   {&__pyx_kp_u_FunctionDescription, __pyx_k_FunctionDescription, sizeof(__pyx_k_FunctionDescription), 0, 1, 0, 0},
   {&__pyx_n_s_FunctionDescription_2, __pyx_k_FunctionDescription_2, sizeof(__pyx_k_FunctionDescription_2), 0, 0, 1, 1},
   {&__pyx_n_s_FunctionDescription___init, __pyx_k_FunctionDescription___init, sizeof(__pyx_k_FunctionDescription___init), 0, 0, 1, 1},
   {&__pyx_n_s_FunctionDescription___repr, __pyx_k_FunctionDescription___repr, sizeof(__pyx_k_FunctionDescription___repr), 0, 0, 1, 1},
   {&__pyx_n_s_FunctionDescription_add_paramete, __pyx_k_FunctionDescription_add_paramete, sizeof(__pyx_k_FunctionDescription_add_paramete), 0, 0, 1, 1},
-  {&__pyx_kp_s_H_M_S, __pyx_k_H_M_S, sizeof(__pyx_k_H_M_S), 0, 0, 1, 0},
-  {&__pyx_kp_s_Invalid_connection_handle, __pyx_k_Invalid_connection_handle, sizeof(__pyx_k_Invalid_connection_handle), 0, 0, 1, 0},
-  {&__pyx_kp_s_Invalid_exception_raised_by_call, __pyx_k_Invalid_exception_raised_by_call, sizeof(__pyx_k_Invalid_exception_raised_by_call), 0, 0, 1, 0},
+  {&__pyx_kp_u_H_M_S, __pyx_k_H_M_S, sizeof(__pyx_k_H_M_S), 0, 1, 0, 0},
+  {&__pyx_kp_u_Invalid_connection_handle, __pyx_k_Invalid_connection_handle, sizeof(__pyx_k_Invalid_connection_handle), 0, 1, 0, 0},
+  {&__pyx_kp_u_Invalid_exception_raised_by_call, __pyx_k_Invalid_exception_raised_by_call, sizeof(__pyx_k_Invalid_exception_raised_by_call), 0, 1, 0, 0},
   {&__pyx_kp_u_Invalid_length_of_unit_id_should, __pyx_k_Invalid_length_of_unit_id_should, sizeof(__pyx_k_Invalid_length_of_unit_id_should), 0, 1, 0, 0},
-  {&__pyx_kp_s_Invocation_finished_submitting, __pyx_k_Invocation_finished_submitting, sizeof(__pyx_k_Invocation_finished_submitting), 0, 0, 1, 0},
+  {&__pyx_kp_u_Invocation_finished_submitting, __pyx_k_Invocation_finished_submitting, sizeof(__pyx_k_Invocation_finished_submitting), 0, 1, 0, 0},
   {&__pyx_n_s_Iterable, __pyx_k_Iterable, sizeof(__pyx_k_Iterable), 0, 0, 1, 1},
   {&__pyx_n_s_LOCALE_RADIX, __pyx_k_LOCALE_RADIX, sizeof(__pyx_k_LOCALE_RADIX), 0, 0, 1, 1},
   {&__pyx_kp_u_Length_of_parameter_unit_id_must, __pyx_k_Length_of_parameter_unit_id_must, sizeof(__pyx_k_Length_of_parameter_unit_id_must), 0, 1, 0, 0},
   {&__pyx_n_s_LogonError, __pyx_k_LogonError, sizeof(__pyx_k_LogonError), 0, 0, 1, 1},
   {&__pyx_n_s_MASK_DTIME, __pyx_k_MASK_DTIME, sizeof(__pyx_k_MASK_DTIME), 0, 0, 1, 1},
   {&__pyx_n_s_MASK_RETURN_IMPORT_PARAMS, __pyx_k_MASK_RETURN_IMPORT_PARAMS, sizeof(__pyx_k_MASK_RETURN_IMPORT_PARAMS), 0, 0, 1, 1},
   {&__pyx_n_s_MASK_RSTRIP, __pyx_k_MASK_RSTRIP, sizeof(__pyx_k_MASK_RSTRIP), 0, 0, 1, 1},
   {&__pyx_kp_u_New_handle, __pyx_k_New_handle, sizeof(__pyx_k_New_handle), 0, 1, 0, 0},
-  {&__pyx_kp_s_No_connections_assigned, __pyx_k_No_connections_assigned, sizeof(__pyx_k_No_connections_assigned), 0, 0, 1, 0},
+  {&__pyx_kp_u_No_connections_assigned, __pyx_k_No_connections_assigned, sizeof(__pyx_k_No_connections_assigned), 0, 1, 0, 0},
   {&__pyx_kp_u_No_metadata_found_for_function, __pyx_k_No_metadata_found_for_function, sizeof(__pyx_k_No_metadata_found_for_function), 0, 1, 0, 0},
-  {&__pyx_kp_s_No_state_check_possible_of_non_b, __pyx_k_No_state_check_possible_of_non_b, sizeof(__pyx_k_No_state_check_possible_of_non_b), 0, 0, 1, 0},
-  {&__pyx_kp_s_No_transaction_handle_for_this_c, __pyx_k_No_transaction_handle_for_this_c, sizeof(__pyx_k_No_transaction_handle_for_this_c), 0, 0, 1, 0},
-  {&__pyx_kp_s_No_unit_handle_for_this_connecti, __pyx_k_No_unit_handle_for_this_connecti, sizeof(__pyx_k_No_unit_handle_for_this_connecti), 0, 0, 1, 0},
-  {&__pyx_kp_s_Not_a_valid_error_group, __pyx_k_Not_a_valid_error_group, sizeof(__pyx_k_Not_a_valid_error_group), 0, 0, 1, 0},
+  {&__pyx_kp_u_No_state_check_possible_of_non_b, __pyx_k_No_state_check_possible_of_non_b, sizeof(__pyx_k_No_state_check_possible_of_non_b), 0, 1, 0, 0},
+  {&__pyx_kp_u_No_transaction_handle_for_this_c, __pyx_k_No_transaction_handle_for_this_c, sizeof(__pyx_k_No_transaction_handle_for_this_c), 0, 1, 0, 0},
+  {&__pyx_kp_u_No_unit_handle_for_this_connecti, __pyx_k_No_unit_handle_for_this_connecti, sizeof(__pyx_k_No_unit_handle_for_this_connecti), 0, 1, 0, 0},
+  {&__pyx_kp_u_Not_a_valid_error_group, __pyx_k_Not_a_valid_error_group, sizeof(__pyx_k_Not_a_valid_error_group), 0, 1, 0, 0},
   {&__pyx_n_s_OK, __pyx_k_OK, sizeof(__pyx_k_OK), 0, 0, 1, 1},
-  {&__pyx_kp_s_Parameter_calls_must_be_iterable, __pyx_k_Parameter_calls_must_be_iterable, sizeof(__pyx_k_Parameter_calls_must_be_iterable), 0, 0, 1, 0},
-  {&__pyx_kp_s_Parameter_calls_must_contain_at, __pyx_k_Parameter_calls_must_contain_at, sizeof(__pyx_k_Parameter_calls_must_contain_at), 0, 0, 1, 0},
-  {&__pyx_kp_s_Parameter_calls_must_contain_val, __pyx_k_Parameter_calls_must_contain_val, sizeof(__pyx_k_Parameter_calls_must_contain_val), 0, 0, 1, 0},
-  {&__pyx_kp_s_Parameter_unit_not_valid_Please, __pyx_k_Parameter_unit_not_valid_Please, sizeof(__pyx_k_Parameter_unit_not_valid_Please), 0, 0, 1, 0},
+  {&__pyx_kp_u_Parameter_calls_must_be_iterable, __pyx_k_Parameter_calls_must_be_iterable, sizeof(__pyx_k_Parameter_calls_must_be_iterable), 0, 1, 0, 0},
+  {&__pyx_kp_u_Parameter_calls_must_contain_at, __pyx_k_Parameter_calls_must_contain_at, sizeof(__pyx_k_Parameter_calls_must_contain_at), 0, 1, 0, 0},
+  {&__pyx_kp_u_Parameter_calls_must_contain_val, __pyx_k_Parameter_calls_must_contain_val, sizeof(__pyx_k_Parameter_calls_must_contain_val), 0, 1, 0, 0},
+  {&__pyx_kp_u_Parameter_unit_not_valid_Please, __pyx_k_Parameter_unit_not_valid_Please, sizeof(__pyx_k_Parameter_unit_not_valid_Please), 0, 1, 0, 0},
   {&__pyx_n_s_Pyx_CFunc_object____object___t, __pyx_k_Pyx_CFunc_object____object___t, sizeof(__pyx_k_Pyx_CFunc_object____object___t), 0, 0, 1, 1},
-  {&__pyx_n_s_Q, __pyx_k_Q, sizeof(__pyx_k_Q), 0, 0, 1, 1},
+  {&__pyx_n_u_Q, __pyx_k_Q, sizeof(__pyx_k_Q), 0, 1, 0, 1},
   {&__pyx_n_s_RCStatus, __pyx_k_RCStatus, sizeof(__pyx_k_RCStatus), 0, 0, 1, 1},
   {&__pyx_n_s_RFCError, __pyx_k_RFCError, sizeof(__pyx_k_RFCError), 0, 0, 1, 1},
   {&__pyx_n_s_RFCTYPE_ABAPOBJECT, __pyx_k_RFCTYPE_ABAPOBJECT, sizeof(__pyx_k_RFCTYPE_ABAPOBJECT), 0, 0, 1, 1},
   {&__pyx_n_s_RFCTYPE_BCD, __pyx_k_RFCTYPE_BCD, sizeof(__pyx_k_RFCTYPE_BCD), 0, 0, 1, 1},
   {&__pyx_n_s_RFCTYPE_BYTE, __pyx_k_RFCTYPE_BYTE, sizeof(__pyx_k_RFCTYPE_BYTE), 0, 0, 1, 1},
   {&__pyx_n_s_RFCTYPE_CDAY, __pyx_k_RFCTYPE_CDAY, sizeof(__pyx_k_RFCTYPE_CDAY), 0, 0, 1, 1},
   {&__pyx_n_s_RFCTYPE_CHAR, __pyx_k_RFCTYPE_CHAR, sizeof(__pyx_k_RFCTYPE_CHAR), 0, 0, 1, 1},
@@ -41769,396 +42525,420 @@
   {&__pyx_n_s_RFC_EXECUTED, __pyx_k_RFC_EXECUTED, sizeof(__pyx_k_RFC_EXECUTED), 0, 0, 1, 1},
   {&__pyx_n_s_RFC_EXPORT, __pyx_k_RFC_EXPORT, sizeof(__pyx_k_RFC_EXPORT), 0, 0, 1, 1},
   {&__pyx_n_s_RFC_EXTERNAL_FAILURE, __pyx_k_RFC_EXTERNAL_FAILURE, sizeof(__pyx_k_RFC_EXTERNAL_FAILURE), 0, 0, 1, 1},
   {&__pyx_n_s_RFC_IMPORT, __pyx_k_RFC_IMPORT, sizeof(__pyx_k_RFC_IMPORT), 0, 0, 1, 1},
   {&__pyx_n_s_RFC_NOT_FOUND, __pyx_k_RFC_NOT_FOUND, sizeof(__pyx_k_RFC_NOT_FOUND), 0, 0, 1, 1},
   {&__pyx_n_s_RFC_TABLES, __pyx_k_RFC_TABLES, sizeof(__pyx_k_RFC_TABLES), 0, 0, 1, 1},
   {&__pyx_kp_u_Remote_function_module, __pyx_k_Remote_function_module, sizeof(__pyx_k_Remote_function_module), 0, 1, 0, 0},
-  {&__pyx_kp_s_Remote_function_module_name_must, __pyx_k_Remote_function_module_name_must, sizeof(__pyx_k_Remote_function_module_name_must), 0, 0, 1, 0},
+  {&__pyx_kp_u_Remote_function_module_name_must, __pyx_k_Remote_function_module_name_must, sizeof(__pyx_k_Remote_function_module_name_must), 0, 1, 0, 0},
   {&__pyx_kp_u_Request_for, __pyx_k_Request_for, sizeof(__pyx_k_Request_for), 0, 1, 0, 0},
   {&__pyx_n_s_RfcFieldType, __pyx_k_RfcFieldType, sizeof(__pyx_k_RfcFieldType), 0, 0, 1, 1},
   {&__pyx_n_s_RfcParameterDirection, __pyx_k_RfcParameterDirection, sizeof(__pyx_k_RfcParameterDirection), 0, 0, 1, 1},
   {&__pyx_n_s_Server, __pyx_k_Server, sizeof(__pyx_k_Server), 0, 0, 1, 1},
+  {&__pyx_n_u_Server, __pyx_k_Server, sizeof(__pyx_k_Server), 0, 1, 0, 1},
   {&__pyx_n_s_ServerConnection, __pyx_k_ServerConnection, sizeof(__pyx_k_ServerConnection), 0, 0, 1, 1},
-  {&__pyx_kp_s_Server_close, __pyx_k_Server_close, sizeof(__pyx_k_Server_close), 0, 0, 1, 0},
-  {&__pyx_kp_s_Server_connection, __pyx_k_Server_connection, sizeof(__pyx_k_Server_connection), 0, 0, 1, 0},
+  {&__pyx_kp_u_Server_close, __pyx_k_Server_close, sizeof(__pyx_k_Server_close), 0, 1, 0, 0},
+  {&__pyx_kp_u_Server_connection, __pyx_k_Server_connection, sizeof(__pyx_k_Server_connection), 0, 1, 0, 0},
   {&__pyx_kp_u_Server_function, __pyx_k_Server_function, sizeof(__pyx_k_Server_function), 0, 1, 0, 0},
-  {&__pyx_kp_s_Server_function_installed, __pyx_k_Server_function_installed, sizeof(__pyx_k_Server_function_installed), 0, 0, 1, 0},
-  {&__pyx_n_s_T, __pyx_k_T, sizeof(__pyx_k_T), 0, 0, 1, 1},
+  {&__pyx_kp_u_Server_function_installed, __pyx_k_Server_function_installed, sizeof(__pyx_k_Server_function_installed), 0, 1, 0, 0},
+  {&__pyx_n_u_T, __pyx_k_T, sizeof(__pyx_k_T), 0, 1, 0, 1},
   {&__pyx_kp_u_TID, __pyx_k_TID, sizeof(__pyx_k_TID), 0, 1, 0, 0},
-  {&__pyx_kp_s_There_is_an_active_unit_for_this, __pyx_k_There_is_an_active_unit_for_this, sizeof(__pyx_k_There_is_an_active_unit_for_this), 0, 0, 1, 0},
+  {&__pyx_kp_u_There_is_an_active_unit_for_this, __pyx_k_There_is_an_active_unit_for_this, sizeof(__pyx_k_There_is_an_active_unit_for_this), 0, 1, 0, 0},
   {&__pyx_n_s_Thread, __pyx_k_Thread, sizeof(__pyx_k_Thread), 0, 0, 1, 1},
   {&__pyx_n_s_Throughput, __pyx_k_Throughput, sizeof(__pyx_k_Throughput), 0, 0, 1, 1},
   {&__pyx_n_s_Timer, __pyx_k_Timer, sizeof(__pyx_k_Timer), 0, 0, 1, 1},
   {&__pyx_kp_u_TypeDescription, __pyx_k_TypeDescription, sizeof(__pyx_k_TypeDescription), 0, 1, 0, 0},
   {&__pyx_n_s_TypeDescription_2, __pyx_k_TypeDescription_2, sizeof(__pyx_k_TypeDescription_2), 0, 0, 1, 1},
   {&__pyx_n_s_TypeDescription___init, __pyx_k_TypeDescription___init, sizeof(__pyx_k_TypeDescription___init), 0, 0, 1, 1},
   {&__pyx_n_s_TypeDescription___repr, __pyx_k_TypeDescription___repr, sizeof(__pyx_k_TypeDescription___repr), 0, 0, 1, 1},
   {&__pyx_n_s_TypeDescription_add_field, __pyx_k_TypeDescription_add_field, sizeof(__pyx_k_TypeDescription_add_field), 0, 0, 1, 1},
   {&__pyx_n_s_TypeError, __pyx_k_TypeError, sizeof(__pyx_k_TypeError), 0, 0, 1, 1},
   {&__pyx_kp_u_UTC, __pyx_k_UTC, sizeof(__pyx_k_UTC), 0, 1, 0, 0},
   {&__pyx_kp_u_Unit, __pyx_k_Unit, sizeof(__pyx_k_Unit), 0, 1, 0, 0},
   {&__pyx_n_s_UnitCallType, __pyx_k_UnitCallType, sizeof(__pyx_k_UnitCallType), 0, 0, 1, 1},
   {&__pyx_n_s_UnitState, __pyx_k_UnitState, sizeof(__pyx_k_UnitState), 0, 0, 1, 1},
-  {&__pyx_kp_s_Unknown_RFC_type_d_when_filling, __pyx_k_Unknown_RFC_type_d_when_filling, sizeof(__pyx_k_Unknown_RFC_type_d_when_filling), 0, 0, 1, 0},
-  {&__pyx_kp_s_Unknown_RFC_type_d_when_wrapping, __pyx_k_Unknown_RFC_type_d_when_wrapping, sizeof(__pyx_k_Unknown_RFC_type_d_when_wrapping), 0, 0, 1, 0},
-  {&__pyx_kp_s_User_user_from_system_sysId_clie, __pyx_k_User_user_from_system_sysId_clie, sizeof(__pyx_k_User_user_from_system_sysId_clie), 0, 0, 1, 0},
+  {&__pyx_kp_u_Unknown_RFC_type, __pyx_k_Unknown_RFC_type, sizeof(__pyx_k_Unknown_RFC_type), 0, 1, 0, 0},
+  {&__pyx_kp_u_User_user_from_system_sysId_clie, __pyx_k_User_user_from_system_sysId_clie, sizeof(__pyx_k_User_user_from_system_sysId_clie), 0, 1, 0, 0},
   {&__pyx_kp_u_Values, __pyx_k_Values, sizeof(__pyx_k_Values), 0, 1, 0, 0},
-  {&__pyx_kp_s_Y_m_d, __pyx_k_Y_m_d, sizeof(__pyx_k_Y_m_d), 0, 0, 1, 0},
-  {&__pyx_kp_s__20, __pyx_k__20, sizeof(__pyx_k__20), 0, 0, 1, 0},
-  {&__pyx_kp_u__20, __pyx_k__20, sizeof(__pyx_k__20), 0, 1, 0, 0},
-  {&__pyx_kp_u__23, __pyx_k__23, sizeof(__pyx_k__23), 0, 1, 0, 0},
+  {&__pyx_kp_u_Y_m_d, __pyx_k_Y_m_d, sizeof(__pyx_k_Y_m_d), 0, 1, 0, 0},
+  {&__pyx_kp_u__21, __pyx_k__21, sizeof(__pyx_k__21), 0, 1, 0, 0},
   {&__pyx_kp_u__24, __pyx_k__24, sizeof(__pyx_k__24), 0, 1, 0, 0},
-  {&__pyx_kp_u__27, __pyx_k__27, sizeof(__pyx_k__27), 0, 1, 0, 0},
+  {&__pyx_kp_u__25, __pyx_k__25, sizeof(__pyx_k__25), 0, 1, 0, 0},
   {&__pyx_kp_u__28, __pyx_k__28, sizeof(__pyx_k__28), 0, 1, 0, 0},
+  {&__pyx_kp_u__29, __pyx_k__29, sizeof(__pyx_k__29), 0, 1, 0, 0},
   {&__pyx_kp_u__3, __pyx_k__3, sizeof(__pyx_k__3), 0, 1, 0, 0},
   {&__pyx_kp_u__4, __pyx_k__4, sizeof(__pyx_k__4), 0, 1, 0, 0},
-  {&__pyx_kp_s__45, __pyx_k__45, sizeof(__pyx_k__45), 0, 0, 1, 0},
-  {&__pyx_kp_s__5, __pyx_k__5, sizeof(__pyx_k__5), 0, 0, 1, 0},
-  {&__pyx_n_s__50, __pyx_k__50, sizeof(__pyx_k__50), 0, 0, 1, 1},
+  {&__pyx_kp_u__46, __pyx_k__46, sizeof(__pyx_k__46), 0, 1, 0, 0},
+  {&__pyx_kp_u__5, __pyx_k__5, sizeof(__pyx_k__5), 0, 1, 0, 0},
+  {&__pyx_n_s__51, __pyx_k__51, sizeof(__pyx_k__51), 0, 0, 1, 1},
   {&__pyx_kp_u__6, __pyx_k__6, sizeof(__pyx_k__6), 0, 1, 0, 0},
-  {&__pyx_kp_s_a_decimal_value_required_receive, __pyx_k_a_decimal_value_required_receive, sizeof(__pyx_k_a_decimal_value_required_receive), 0, 0, 1, 0},
-  {&__pyx_kp_s_a_numeric_string_is_required_rec, __pyx_k_a_numeric_string_is_required_rec, sizeof(__pyx_k_a_numeric_string_is_required_rec), 0, 0, 1, 0},
-  {&__pyx_n_s_active_unit, __pyx_k_active_unit, sizeof(__pyx_k_active_unit), 0, 0, 1, 1},
+  {&__pyx_kp_u_a_decimal_value_required_receive, __pyx_k_a_decimal_value_required_receive, sizeof(__pyx_k_a_decimal_value_required_receive), 0, 1, 0, 0},
+  {&__pyx_kp_u_a_numeric_string_is_required_rec, __pyx_k_a_numeric_string_is_required_rec, sizeof(__pyx_k_a_numeric_string_is_required_rec), 0, 1, 0, 0},
+  {&__pyx_n_u_active_unit, __pyx_k_active_unit, sizeof(__pyx_k_active_unit), 0, 1, 0, 1},
   {&__pyx_n_s_add, __pyx_k_add, sizeof(__pyx_k_add), 0, 0, 1, 1},
   {&__pyx_n_s_add_field, __pyx_k_add_field, sizeof(__pyx_k_add_field), 0, 0, 1, 1},
   {&__pyx_n_s_add_parameter, __pyx_k_add_parameter, sizeof(__pyx_k_add_parameter), 0, 0, 1, 1},
   {&__pyx_n_s_alive, __pyx_k_alive, sizeof(__pyx_k_alive), 0, 0, 1, 1},
   {&__pyx_kp_u_already_installed, __pyx_k_already_installed, sizeof(__pyx_k_already_installed), 0, 1, 0, 0},
-  {&__pyx_kp_s_an_integer_required_received, __pyx_k_an_integer_required_received, sizeof(__pyx_k_an_integer_required_received), 0, 0, 1, 0},
-  {&__pyx_kp_s_an_string_is_required_received, __pyx_k_an_string_is_required_received, sizeof(__pyx_k_an_string_is_required_received), 0, 0, 1, 0},
+  {&__pyx_kp_u_an_integer_required_received, __pyx_k_an_integer_required_received, sizeof(__pyx_k_an_integer_required_received), 0, 1, 0, 0},
+  {&__pyx_kp_u_an_string_is_required_received, __pyx_k_an_string_is_required_received, sizeof(__pyx_k_an_string_is_required_received), 0, 1, 0, 0},
   {&__pyx_n_s_append, __pyx_k_append, sizeof(__pyx_k_append), 0, 0, 1, 1},
-  {&__pyx_n_s_applicationTime, __pyx_k_applicationTime, sizeof(__pyx_k_applicationTime), 0, 0, 1, 1},
+  {&__pyx_n_u_applicationTime, __pyx_k_applicationTime, sizeof(__pyx_k_applicationTime), 0, 1, 0, 1},
   {&__pyx_n_s_args, __pyx_k_args, sizeof(__pyx_k_args), 0, 0, 1, 1},
   {&__pyx_n_s_attributes, __pyx_k_attributes, sizeof(__pyx_k_attributes), 0, 0, 1, 1},
-  {&__pyx_n_s_auth_check, __pyx_k_auth_check, sizeof(__pyx_k_auth_check), 0, 0, 1, 1},
+  {&__pyx_n_u_auth_check, __pyx_k_auth_check, sizeof(__pyx_k_auth_check), 0, 1, 0, 1},
   {&__pyx_kp_u_authorization_check_for, __pyx_k_authorization_check_for, sizeof(__pyx_k_authorization_check_for), 0, 1, 0, 0},
   {&__pyx_n_s_auto, __pyx_k_auto, sizeof(__pyx_k_auto), 0, 0, 1, 1},
   {&__pyx_n_s_background, __pyx_k_background, sizeof(__pyx_k_background), 0, 0, 1, 1},
+  {&__pyx_n_u_background, __pyx_k_background, sizeof(__pyx_k_background), 0, 1, 0, 1},
   {&__pyx_n_s_background_unit, __pyx_k_background_unit, sizeof(__pyx_k_background_unit), 0, 0, 1, 1},
-  {&__pyx_kp_s_bgRFC_handler_onGetState_is_not, __pyx_k_bgRFC_handler_onGetState_is_not, sizeof(__pyx_k_bgRFC_handler_onGetState_is_not), 0, 0, 1, 0},
+  {&__pyx_kp_u_bgRFC_handler_onGetState_is_not, __pyx_k_bgRFC_handler_onGetState_is_not, sizeof(__pyx_k_bgRFC_handler_onGetState_is_not), 0, 1, 0, 0},
   {&__pyx_n_s_bgRfcFunction, __pyx_k_bgRfcFunction, sizeof(__pyx_k_bgRfcFunction), 0, 0, 1, 1},
   {&__pyx_n_s_bgRfcFunction_2, __pyx_k_bgRfcFunction_2, sizeof(__pyx_k_bgRfcFunction_2), 0, 0, 1, 1},
   {&__pyx_kp_u_but_found, __pyx_k_but_found, sizeof(__pyx_k_but_found), 0, 1, 0, 0},
-  {&__pyx_n_s_call_type, __pyx_k_call_type, sizeof(__pyx_k_call_type), 0, 0, 1, 1},
+  {&__pyx_n_u_call_type, __pyx_k_call_type, sizeof(__pyx_k_call_type), 0, 1, 0, 1},
   {&__pyx_n_s_callback, __pyx_k_callback, sizeof(__pyx_k_callback), 0, 0, 1, 1},
+  {&__pyx_n_u_callback, __pyx_k_callback, sizeof(__pyx_k_callback), 0, 1, 0, 1},
   {&__pyx_n_s_calls, __pyx_k_calls, sizeof(__pyx_k_calls), 0, 0, 1, 1},
   {&__pyx_n_s_cancel, __pyx_k_cancel, sizeof(__pyx_k_cancel), 0, 0, 1, 1},
   {&__pyx_n_s_cancel_connection, __pyx_k_cancel_connection, sizeof(__pyx_k_cancel_connection), 0, 0, 1, 1},
   {&__pyx_n_s_cfunc_to_py, __pyx_k_cfunc_to_py, sizeof(__pyx_k_cfunc_to_py), 0, 0, 1, 1},
   {&__pyx_kp_u_chars_found, __pyx_k_chars_found, sizeof(__pyx_k_chars_found), 0, 1, 0, 0},
-  {&__pyx_n_s_check, __pyx_k_check, sizeof(__pyx_k_check), 0, 0, 1, 1},
+  {&__pyx_n_u_check, __pyx_k_check, sizeof(__pyx_k_check), 0, 1, 0, 1},
   {&__pyx_n_s_clear, __pyx_k_clear, sizeof(__pyx_k_clear), 0, 0, 1, 1},
-  {&__pyx_n_s_client, __pyx_k_client, sizeof(__pyx_k_client), 0, 0, 1, 1},
+  {&__pyx_n_u_client, __pyx_k_client, sizeof(__pyx_k_client), 0, 1, 0, 1},
   {&__pyx_n_s_client_connection, __pyx_k_client_connection, sizeof(__pyx_k_client_connection), 0, 0, 1, 1},
   {&__pyx_n_s_client_params, __pyx_k_client_params, sizeof(__pyx_k_client_params), 0, 0, 1, 1},
   {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
   {&__pyx_n_s_close, __pyx_k_close, sizeof(__pyx_k_close), 0, 0, 1, 1},
   {&__pyx_n_s_close_2, __pyx_k_close_2, sizeof(__pyx_k_close_2), 0, 0, 1, 1},
   {&__pyx_n_s_code, __pyx_k_code, sizeof(__pyx_k_code), 0, 0, 1, 1},
   {&__pyx_kp_u_code_set_to_RFC_ABAP_EXCEPTION, __pyx_k_code_set_to_RFC_ABAP_EXCEPTION, sizeof(__pyx_k_code_set_to_RFC_ABAP_EXCEPTION), 0, 1, 0, 0},
   {&__pyx_kp_u_code_set_to_RFC_ABAP_MESSAGE, __pyx_k_code_set_to_RFC_ABAP_MESSAGE, sizeof(__pyx_k_code_set_to_RFC_ABAP_MESSAGE), 0, 1, 0, 0},
   {&__pyx_kp_u_code_set_to_RFC_EXTERNAL_FAILUR, __pyx_k_code_set_to_RFC_EXTERNAL_FAILUR, sizeof(__pyx_k_code_set_to_RFC_EXTERNAL_FAILUR), 0, 1, 0, 0},
-  {&__pyx_n_s_codepage, __pyx_k_codepage, sizeof(__pyx_k_codepage), 0, 0, 1, 1},
+  {&__pyx_n_u_codepage, __pyx_k_codepage, sizeof(__pyx_k_codepage), 0, 1, 0, 1},
   {&__pyx_n_s_collections_abc, __pyx_k_collections_abc, sizeof(__pyx_k_collections_abc), 0, 0, 1, 1},
-  {&__pyx_n_s_commit, __pyx_k_commit, sizeof(__pyx_k_commit), 0, 0, 1, 1},
+  {&__pyx_n_u_commit, __pyx_k_commit, sizeof(__pyx_k_commit), 0, 1, 0, 1},
   {&__pyx_n_s_committed, __pyx_k_committed, sizeof(__pyx_k_committed), 0, 0, 1, 1},
   {&__pyx_n_s_config, __pyx_k_config, sizeof(__pyx_k_config), 0, 0, 1, 1},
-  {&__pyx_n_s_confirm, __pyx_k_confirm, sizeof(__pyx_k_confirm), 0, 0, 1, 1},
+  {&__pyx_n_u_confirm, __pyx_k_confirm, sizeof(__pyx_k_confirm), 0, 1, 0, 1},
   {&__pyx_n_s_confirm_transaction, __pyx_k_confirm_transaction, sizeof(__pyx_k_confirm_transaction), 0, 0, 1, 1},
   {&__pyx_n_s_confirm_unit, __pyx_k_confirm_unit, sizeof(__pyx_k_confirm_unit), 0, 0, 1, 1},
   {&__pyx_n_s_confirmed, __pyx_k_confirmed, sizeof(__pyx_k_confirmed), 0, 0, 1, 1},
   {&__pyx_n_s_connection, __pyx_k_connection, sizeof(__pyx_k_connection), 0, 0, 1, 1},
-  {&__pyx_n_s_connection_attributes, __pyx_k_connection_attributes, sizeof(__pyx_k_connection_attributes), 0, 0, 1, 1},
+  {&__pyx_n_u_connection_attributes, __pyx_k_connection_attributes, sizeof(__pyx_k_connection_attributes), 0, 1, 0, 1},
   {&__pyx_n_s_connections, __pyx_k_connections, sizeof(__pyx_k_connections), 0, 0, 1, 1},
-  {&__pyx_n_s_cpicConvId, __pyx_k_cpicConvId, sizeof(__pyx_k_cpicConvId), 0, 0, 1, 1},
+  {&__pyx_n_u_cpicConvId, __pyx_k_cpicConvId, sizeof(__pyx_k_cpicConvId), 0, 1, 0, 1},
   {&__pyx_n_s_create_and_submit_transaction, __pyx_k_create_and_submit_transaction, sizeof(__pyx_k_create_and_submit_transaction), 0, 0, 1, 1},
   {&__pyx_n_s_create_and_submit_unit, __pyx_k_create_and_submit_unit, sizeof(__pyx_k_create_and_submit_unit), 0, 0, 1, 1},
   {&__pyx_n_s_created, __pyx_k_created, sizeof(__pyx_k_created), 0, 0, 1, 1},
-  {&__pyx_n_s_currentBusyCount, __pyx_k_currentBusyCount, sizeof(__pyx_k_currentBusyCount), 0, 0, 1, 1},
+  {&__pyx_n_u_currentBusyCount, __pyx_k_currentBusyCount, sizeof(__pyx_k_currentBusyCount), 0, 1, 0, 1},
+  {&__pyx_n_u_d, __pyx_k_d, sizeof(__pyx_k_d), 0, 1, 0, 1},
   {&__pyx_n_s_date, __pyx_k_date, sizeof(__pyx_k_date), 0, 0, 1, 1},
-  {&__pyx_kp_s_date_value_required_received, __pyx_k_date_value_required_received, sizeof(__pyx_k_date_value_required_received), 0, 0, 1, 0},
+  {&__pyx_kp_u_date_value_required_received, __pyx_k_date_value_required_received, sizeof(__pyx_k_date_value_required_received), 0, 1, 0, 0},
   {&__pyx_n_s_datetime, __pyx_k_datetime, sizeof(__pyx_k_datetime), 0, 0, 1, 1},
   {&__pyx_n_s_day, __pyx_k_day, sizeof(__pyx_k_day), 0, 0, 1, 1},
   {&__pyx_n_s_debug, __pyx_k_debug, sizeof(__pyx_k_debug), 0, 0, 1, 1},
+  {&__pyx_n_u_debug, __pyx_k_debug, sizeof(__pyx_k_debug), 0, 1, 0, 1},
   {&__pyx_n_s_decimal, __pyx_k_decimal, sizeof(__pyx_k_decimal), 0, 0, 1, 1},
-  {&__pyx_n_s_decimal_point, __pyx_k_decimal_point, sizeof(__pyx_k_decimal_point), 0, 0, 1, 1},
+  {&__pyx_n_u_decimal_point, __pyx_k_decimal_point, sizeof(__pyx_k_decimal_point), 0, 1, 0, 1},
   {&__pyx_n_s_decimals, __pyx_k_decimals, sizeof(__pyx_k_decimals), 0, 0, 1, 1},
+  {&__pyx_n_u_decimals, __pyx_k_decimals, sizeof(__pyx_k_decimals), 0, 1, 0, 1},
   {&__pyx_n_s_decode, __pyx_k_decode, sizeof(__pyx_k_decode), 0, 0, 1, 1},
   {&__pyx_n_s_default_auth_check, __pyx_k_default_auth_check, sizeof(__pyx_k_default_auth_check), 0, 0, 1, 1},
   {&__pyx_n_s_default_value, __pyx_k_default_value, sizeof(__pyx_k_default_value), 0, 0, 1, 1},
+  {&__pyx_n_u_default_value, __pyx_k_default_value, sizeof(__pyx_k_default_value), 0, 1, 0, 1},
   {&__pyx_kp_u_default_value_string, __pyx_k_default_value_string, sizeof(__pyx_k_default_value_string), 0, 1, 0, 0},
   {&__pyx_n_s_del, __pyx_k_del, sizeof(__pyx_k_del), 0, 0, 1, 1},
-  {&__pyx_n_s_deserializationTime, __pyx_k_deserializationTime, sizeof(__pyx_k_deserializationTime), 0, 0, 1, 1},
-  {&__pyx_n_s_dest, __pyx_k_dest, sizeof(__pyx_k_dest), 0, 0, 1, 1},
+  {&__pyx_n_u_deserializationTime, __pyx_k_deserializationTime, sizeof(__pyx_k_deserializationTime), 0, 1, 0, 1},
+  {&__pyx_n_u_dest, __pyx_k_dest, sizeof(__pyx_k_dest), 0, 1, 0, 1},
   {&__pyx_n_s_destroy, __pyx_k_destroy, sizeof(__pyx_k_destroy), 0, 0, 1, 1},
   {&__pyx_n_s_destroy_transaction, __pyx_k_destroy_transaction, sizeof(__pyx_k_destroy_transaction), 0, 0, 1, 1},
   {&__pyx_n_s_destroy_unit, __pyx_k_destroy_unit, sizeof(__pyx_k_destroy_unit), 0, 0, 1, 1},
-  {&__pyx_kp_s_dictionary_required_for_structur, __pyx_k_dictionary_required_for_structur, sizeof(__pyx_k_dictionary_required_for_structur), 0, 0, 1, 0},
+  {&__pyx_kp_u_dictionary_required_for_structur, __pyx_k_dictionary_required_for_structur, sizeof(__pyx_k_dictionary_required_for_structur), 0, 1, 0, 0},
   {&__pyx_n_s_direction, __pyx_k_direction, sizeof(__pyx_k_direction), 0, 0, 1, 1},
+  {&__pyx_n_u_direction, __pyx_k_direction, sizeof(__pyx_k_direction), 0, 1, 0, 1},
   {&__pyx_kp_u_direction_string, __pyx_k_direction_string, sizeof(__pyx_k_direction_string), 0, 1, 0, 0},
   {&__pyx_n_s_doc, __pyx_k_doc, sizeof(__pyx_k_doc), 0, 0, 1, 1},
-  {&__pyx_n_s_dtime, __pyx_k_dtime, sizeof(__pyx_k_dtime), 0, 0, 1, 1},
+  {&__pyx_n_u_dtime, __pyx_k_dtime, sizeof(__pyx_k_dtime), 0, 1, 0, 1},
   {&__pyx_n_s_encode, __pyx_k_encode, sizeof(__pyx_k_encode), 0, 0, 1, 1},
-  {&__pyx_n_s_end, __pyx_k_end, sizeof(__pyx_k_end), 0, 0, 1, 1},
   {&__pyx_n_s_enum, __pyx_k_enum, sizeof(__pyx_k_enum), 0, 0, 1, 1},
   {&__pyx_n_s_enum_names, __pyx_k_enum_names, sizeof(__pyx_k_enum_names), 0, 0, 1, 1},
   {&__pyx_n_s_enum_values, __pyx_k_enum_values, sizeof(__pyx_k_enum_values), 0, 0, 1, 1},
   {&__pyx_n_s_enumerate, __pyx_k_enumerate, sizeof(__pyx_k_enumerate), 0, 0, 1, 1},
   {&__pyx_n_s_errorInfo, __pyx_k_errorInfo, sizeof(__pyx_k_errorInfo), 0, 0, 1, 1},
   {&__pyx_n_s_exc_info, __pyx_k_exc_info, sizeof(__pyx_k_exc_info), 0, 0, 1, 1},
   {&__pyx_n_s_exception, __pyx_k_exception, sizeof(__pyx_k_exception), 0, 0, 1, 1},
   {&__pyx_n_s_executed, __pyx_k_executed, sizeof(__pyx_k_executed), 0, 0, 1, 1},
   {&__pyx_kp_u_field, __pyx_k_field, sizeof(__pyx_k_field), 0, 1, 0, 0},
   {&__pyx_kp_u_field_name_string, __pyx_k_field_name_string, sizeof(__pyx_k_field_name_string), 0, 1, 0, 0},
   {&__pyx_kp_u_field_name_string_2, __pyx_k_field_name_string_2, sizeof(__pyx_k_field_name_string_2), 0, 1, 0, 0},
   {&__pyx_n_s_field_type, __pyx_k_field_type, sizeof(__pyx_k_field_type), 0, 0, 1, 1},
+  {&__pyx_n_u_field_type, __pyx_k_field_type, sizeof(__pyx_k_field_type), 0, 1, 0, 1},
   {&__pyx_kp_u_field_type_string, __pyx_k_field_type_string, sizeof(__pyx_k_field_type_string), 0, 1, 0, 0},
   {&__pyx_n_s_fields, __pyx_k_fields, sizeof(__pyx_k_fields), 0, 0, 1, 1},
   {&__pyx_kp_u_fields_n_uclength, __pyx_k_fields_n_uclength, sizeof(__pyx_k_fields_n_uclength), 0, 1, 0, 0},
-  {&__pyx_n_s_file, __pyx_k_file, sizeof(__pyx_k_file), 0, 0, 1, 1},
   {&__pyx_n_s_format, __pyx_k_format, sizeof(__pyx_k_format), 0, 0, 1, 1},
   {&__pyx_n_s_free, __pyx_k_free, sizeof(__pyx_k_free), 0, 0, 1, 1},
-  {&__pyx_n_s_func_desc_handle, __pyx_k_func_desc_handle, sizeof(__pyx_k_func_desc_handle), 0, 0, 1, 1},
+  {&__pyx_n_u_func_desc_handle, __pyx_k_func_desc_handle, sizeof(__pyx_k_func_desc_handle), 0, 1, 0, 1},
   {&__pyx_n_s_func_name, __pyx_k_func_name, sizeof(__pyx_k_func_name), 0, 0, 1, 1},
   {&__pyx_n_s_function_name, __pyx_k_function_name, sizeof(__pyx_k_function_name), 0, 0, 1, 1},
-  {&__pyx_n_s_genericHandler, __pyx_k_genericHandler, sizeof(__pyx_k_genericHandler), 0, 0, 1, 1},
+  {&__pyx_n_u_genericHandler, __pyx_k_genericHandler, sizeof(__pyx_k_genericHandler), 0, 1, 0, 1},
   {&__pyx_n_s_get, __pyx_k_get, sizeof(__pyx_k_get), 0, 0, 1, 1},
   {&__pyx_n_s_getFromConnection, __pyx_k_getFromConnection, sizeof(__pyx_k_getFromConnection), 0, 0, 1, 1},
-  {&__pyx_n_s_getState, __pyx_k_getState, sizeof(__pyx_k_getState), 0, 0, 1, 1},
+  {&__pyx_n_u_getState, __pyx_k_getState, sizeof(__pyx_k_getState), 0, 1, 0, 1},
   {&__pyx_n_s_get_nwrfclib_version, __pyx_k_get_nwrfclib_version, sizeof(__pyx_k_get_nwrfclib_version), 0, 0, 1, 1},
   {&__pyx_n_s_get_transaction_id, __pyx_k_get_transaction_id, sizeof(__pyx_k_get_transaction_id), 0, 0, 1, 1},
   {&__pyx_n_s_get_unit_id, __pyx_k_get_unit_id, sizeof(__pyx_k_get_unit_id), 0, 0, 1, 1},
   {&__pyx_n_s_get_unit_state, __pyx_k_get_unit_state, sizeof(__pyx_k_get_unit_state), 0, 0, 1, 1},
   {&__pyx_n_s_gethostname, __pyx_k_gethostname, sizeof(__pyx_k_gethostname), 0, 0, 1, 1},
   {&__pyx_n_s_getstate, __pyx_k_getstate, sizeof(__pyx_k_getstate), 0, 0, 1, 1},
   {&__pyx_n_s_handle, __pyx_k_handle, sizeof(__pyx_k_handle), 0, 0, 1, 1},
   {&__pyx_kp_u_handle_2, __pyx_k_handle_2, sizeof(__pyx_k_handle_2), 0, 1, 0, 0},
   {&__pyx_n_s_handle_3, __pyx_k_handle_3, sizeof(__pyx_k_handle_3), 0, 0, 1, 1},
   {&__pyx_kp_u_has_invalid_state, __pyx_k_has_invalid_state, sizeof(__pyx_k_has_invalid_state), 0, 1, 0, 0},
-  {&__pyx_n_s_host, __pyx_k_host, sizeof(__pyx_k_host), 0, 0, 1, 1},
-  {&__pyx_n_s_hostname, __pyx_k_hostname, sizeof(__pyx_k_hostname), 0, 0, 1, 1},
+  {&__pyx_n_u_host, __pyx_k_host, sizeof(__pyx_k_host), 0, 1, 0, 1},
+  {&__pyx_n_u_hostname, __pyx_k_hostname, sizeof(__pyx_k_hostname), 0, 1, 0, 1},
   {&__pyx_n_s_hour, __pyx_k_hour, sizeof(__pyx_k_hour), 0, 0, 1, 1},
-  {&__pyx_n_s_id, __pyx_k_id, sizeof(__pyx_k_id), 0, 0, 1, 1},
+  {&__pyx_n_u_id, __pyx_k_id, sizeof(__pyx_k_id), 0, 1, 0, 1},
   {&__pyx_n_s_idunitStateentifier, __pyx_k_idunitStateentifier, sizeof(__pyx_k_idunitStateentifier), 0, 0, 1, 1},
   {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
   {&__pyx_n_s_in_process, __pyx_k_in_process, sizeof(__pyx_k_in_process), 0, 0, 1, 1},
   {&__pyx_n_s_init, __pyx_k_init, sizeof(__pyx_k_init), 0, 0, 1, 1},
   {&__pyx_n_s_install_bgrfc_handlers, __pyx_k_install_bgrfc_handlers, sizeof(__pyx_k_install_bgrfc_handlers), 0, 0, 1, 1},
   {&__pyx_n_s_int_field, __pyx_k_int_field, sizeof(__pyx_k_int_field), 0, 0, 1, 1},
   {&__pyx_kp_u_invalid_state, __pyx_k_invalid_state, sizeof(__pyx_k_invalid_state), 0, 1, 0, 0},
   {&__pyx_kp_u_invocation_rejected_because_the, __pyx_k_invocation_rejected_because_the, sizeof(__pyx_k_invocation_rejected_because_the), 0, 1, 0, 0},
   {&__pyx_n_s_is_alive, __pyx_k_is_alive, sizeof(__pyx_k_is_alive), 0, 0, 1, 1},
   {&__pyx_kp_u_is_not_callable, __pyx_k_is_not_callable, sizeof(__pyx_k_is_not_callable), 0, 1, 0, 0},
   {&__pyx_kp_u_is_not_supported, __pyx_k_is_not_supported, sizeof(__pyx_k_is_not_supported), 0, 1, 0, 0},
-  {&__pyx_n_s_is_stateful, __pyx_k_is_stateful, sizeof(__pyx_k_is_stateful), 0, 0, 1, 1},
+  {&__pyx_n_u_is_stateful, __pyx_k_is_stateful, sizeof(__pyx_k_is_stateful), 0, 1, 0, 1},
   {&__pyx_n_s_is_valid, __pyx_k_is_valid, sizeof(__pyx_k_is_valid), 0, 0, 1, 1},
   {&__pyx_n_s_isdigit, __pyx_k_isdigit, sizeof(__pyx_k_isdigit), 0, 0, 1, 1},
   {&__pyx_n_s_isfile, __pyx_k_isfile, sizeof(__pyx_k_isfile), 0, 0, 1, 1},
-  {&__pyx_n_s_isoLanguage, __pyx_k_isoLanguage, sizeof(__pyx_k_isoLanguage), 0, 0, 1, 1},
+  {&__pyx_n_u_isoLanguage, __pyx_k_isoLanguage, sizeof(__pyx_k_isoLanguage), 0, 1, 0, 1},
   {&__pyx_n_s_items, __pyx_k_items, sizeof(__pyx_k_items), 0, 0, 1, 1},
   {&__pyx_n_s_iteritems, __pyx_k_iteritems, sizeof(__pyx_k_iteritems), 0, 0, 1, 1},
   {&__pyx_n_s_join, __pyx_k_join, sizeof(__pyx_k_join), 0, 0, 1, 1},
-  {&__pyx_n_s_kernelRel, __pyx_k_kernelRel, sizeof(__pyx_k_kernelRel), 0, 0, 1, 1},
-  {&__pyx_n_s_kernel_trace, __pyx_k_kernel_trace, sizeof(__pyx_k_kernel_trace), 0, 0, 1, 1},
+  {&__pyx_n_u_kernelRel, __pyx_k_kernelRel, sizeof(__pyx_k_kernelRel), 0, 1, 0, 1},
+  {&__pyx_n_u_kernel_trace, __pyx_k_kernel_trace, sizeof(__pyx_k_kernel_trace), 0, 1, 0, 1},
   {&__pyx_n_s_key, __pyx_k_key, sizeof(__pyx_k_key), 0, 0, 1, 1},
   {&__pyx_n_s_lang_iso, __pyx_k_lang_iso, sizeof(__pyx_k_lang_iso), 0, 0, 1, 1},
   {&__pyx_n_s_lang_sap, __pyx_k_lang_sap, sizeof(__pyx_k_lang_sap), 0, 0, 1, 1},
-  {&__pyx_n_s_language, __pyx_k_language, sizeof(__pyx_k_language), 0, 0, 1, 1},
+  {&__pyx_n_u_language, __pyx_k_language, sizeof(__pyx_k_language), 0, 1, 0, 1},
   {&__pyx_n_s_language_iso_to_sap, __pyx_k_language_iso_to_sap, sizeof(__pyx_k_language_iso_to_sap), 0, 0, 1, 1},
   {&__pyx_n_s_language_sap_to_iso, __pyx_k_language_sap_to_iso, sizeof(__pyx_k_language_sap_to_iso), 0, 0, 1, 1},
   {&__pyx_kp_u_launched, __pyx_k_launched, sizeof(__pyx_k_launched), 0, 1, 0, 0},
   {&__pyx_kp_u_length, __pyx_k_length, sizeof(__pyx_k_length), 0, 1, 0, 0},
-  {&__pyx_kp_s_list_required_for_table_paramete, __pyx_k_list_required_for_table_paramete, sizeof(__pyx_k_list_required_for_table_paramete), 0, 0, 1, 0},
+  {&__pyx_kp_u_list_required_for_table_paramete, __pyx_k_list_required_for_table_paramete, sizeof(__pyx_k_list_required_for_table_paramete), 0, 1, 0, 0},
   {&__pyx_n_s_locale, __pyx_k_locale, sizeof(__pyx_k_locale), 0, 0, 1, 1},
   {&__pyx_n_s_localeconv, __pyx_k_localeconv, sizeof(__pyx_k_localeconv), 0, 0, 1, 1},
-  {&__pyx_n_s_lock, __pyx_k_lock, sizeof(__pyx_k_lock), 0, 0, 1, 1},
+  {&__pyx_n_u_lock, __pyx_k_lock, sizeof(__pyx_k_lock), 0, 1, 0, 1},
   {&__pyx_n_s_log_message, __pyx_k_log_message, sizeof(__pyx_k_log_message), 0, 0, 1, 1},
   {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
   {&__pyx_n_s_major, __pyx_k_major, sizeof(__pyx_k_major), 0, 0, 1, 1},
+  {&__pyx_n_u_major, __pyx_k_major, sizeof(__pyx_k_major), 0, 1, 0, 1},
   {&__pyx_n_s_message, __pyx_k_message, sizeof(__pyx_k_message), 0, 0, 1, 1},
   {&__pyx_n_s_metaclass, __pyx_k_metaclass, sizeof(__pyx_k_metaclass), 0, 0, 1, 1},
-  {&__pyx_n_s_metadataLookup, __pyx_k_metadataLookup, sizeof(__pyx_k_metadataLookup), 0, 0, 1, 1},
+  {&__pyx_n_u_metadataLookup, __pyx_k_metadataLookup, sizeof(__pyx_k_metadataLookup), 0, 1, 0, 1},
   {&__pyx_n_s_minor, __pyx_k_minor, sizeof(__pyx_k_minor), 0, 0, 1, 1},
+  {&__pyx_n_u_minor, __pyx_k_minor, sizeof(__pyx_k_minor), 0, 1, 0, 1},
   {&__pyx_n_s_minute, __pyx_k_minute, sizeof(__pyx_k_minute), 0, 0, 1, 1},
   {&__pyx_n_s_module, __pyx_k_module, sizeof(__pyx_k_module), 0, 0, 1, 1},
   {&__pyx_n_s_month, __pyx_k_month, sizeof(__pyx_k_month), 0, 0, 1, 1},
   {&__pyx_n_s_msg_class, __pyx_k_msg_class, sizeof(__pyx_k_msg_class), 0, 0, 1, 1},
   {&__pyx_n_s_msg_number, __pyx_k_msg_number, sizeof(__pyx_k_msg_number), 0, 0, 1, 1},
   {&__pyx_n_s_msg_type, __pyx_k_msg_type, sizeof(__pyx_k_msg_type), 0, 0, 1, 1},
   {&__pyx_n_s_msg_v1, __pyx_k_msg_v1, sizeof(__pyx_k_msg_v1), 0, 0, 1, 1},
   {&__pyx_n_s_msg_v2, __pyx_k_msg_v2, sizeof(__pyx_k_msg_v2), 0, 0, 1, 1},
   {&__pyx_n_s_msg_v3, __pyx_k_msg_v3, sizeof(__pyx_k_msg_v3), 0, 0, 1, 1},
   {&__pyx_n_s_msg_v4, __pyx_k_msg_v4, sizeof(__pyx_k_msg_v4), 0, 0, 1, 1},
-  {&__pyx_kp_s_multi_count, __pyx_k_multi_count, sizeof(__pyx_k_multi_count), 0, 0, 1, 0},
+  {&__pyx_kp_u_multi_count, __pyx_k_multi_count, sizeof(__pyx_k_multi_count), 0, 1, 0, 0},
   {&__pyx_kp_u_must_be_in, __pyx_k_must_be_in, sizeof(__pyx_k_must_be_in), 0, 1, 0, 0},
   {&__pyx_kp_u_must_be_in_2, __pyx_k_must_be_in_2, sizeof(__pyx_k_must_be_in_2), 0, 1, 0, 0},
   {&__pyx_kp_u_must_be_of_type_integer, __pyx_k_must_be_of_type_integer, sizeof(__pyx_k_must_be_of_type_integer), 0, 1, 0, 0},
   {&__pyx_kp_u_must_not_exceed_30_chars, __pyx_k_must_not_exceed_30_chars, sizeof(__pyx_k_must_not_exceed_30_chars), 0, 1, 0, 0},
   {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
+  {&__pyx_n_u_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 1, 0, 1},
   {&__pyx_n_s_name_2, __pyx_k_name_2, sizeof(__pyx_k_name_2), 0, 0, 1, 1},
-  {&__pyx_n_s_no_commit_check, __pyx_k_no_commit_check, sizeof(__pyx_k_no_commit_check), 0, 0, 1, 1},
+  {&__pyx_n_u_no_commit_check, __pyx_k_no_commit_check, sizeof(__pyx_k_no_commit_check), 0, 1, 0, 1},
   {&__pyx_kp_s_no_default___reduce___due_to_non, __pyx_k_no_default___reduce___due_to_non, sizeof(__pyx_k_no_default___reduce___due_to_non), 0, 0, 1, 0},
   {&__pyx_n_s_not_found, __pyx_k_not_found, sizeof(__pyx_k_not_found), 0, 0, 1, 1},
-  {&__pyx_n_s_not_requested, __pyx_k_not_requested, sizeof(__pyx_k_not_requested), 0, 0, 1, 1},
+  {&__pyx_n_u_not_requested, __pyx_k_not_requested, sizeof(__pyx_k_not_requested), 0, 1, 0, 1},
   {&__pyx_n_s_nuc_length, __pyx_k_nuc_length, sizeof(__pyx_k_nuc_length), 0, 0, 1, 1},
+  {&__pyx_n_u_nuc_length, __pyx_k_nuc_length, sizeof(__pyx_k_nuc_length), 0, 1, 0, 1},
   {&__pyx_n_s_nuc_offset, __pyx_k_nuc_offset, sizeof(__pyx_k_nuc_offset), 0, 0, 1, 1},
-  {&__pyx_n_s_numberOfCalls, __pyx_k_numberOfCalls, sizeof(__pyx_k_numberOfCalls), 0, 0, 1, 1},
+  {&__pyx_n_u_nuc_offset, __pyx_k_nuc_offset, sizeof(__pyx_k_nuc_offset), 0, 1, 0, 1},
+  {&__pyx_n_u_numberOfCalls, __pyx_k_numberOfCalls, sizeof(__pyx_k_numberOfCalls), 0, 1, 0, 1},
   {&__pyx_n_s_object, __pyx_k_object, sizeof(__pyx_k_object), 0, 0, 1, 1},
-  {&__pyx_kp_s_of_type, __pyx_k_of_type, sizeof(__pyx_k_of_type), 0, 0, 1, 0},
+  {&__pyx_kp_u_of_type, __pyx_k_of_type, sizeof(__pyx_k_of_type), 0, 1, 0, 0},
   {&__pyx_n_s_open, __pyx_k_open, sizeof(__pyx_k_open), 0, 0, 1, 1},
   {&__pyx_n_s_optional, __pyx_k_optional, sizeof(__pyx_k_optional), 0, 0, 1, 1},
+  {&__pyx_n_u_optional, __pyx_k_optional, sizeof(__pyx_k_optional), 0, 1, 0, 1},
   {&__pyx_n_s_options, __pyx_k_options, sizeof(__pyx_k_options), 0, 0, 1, 1},
-  {&__pyx_kp_s_or_confirm_unit, __pyx_k_or_confirm_unit, sizeof(__pyx_k_or_confirm_unit), 0, 0, 1, 0},
   {&__pyx_n_s_origin, __pyx_k_origin, sizeof(__pyx_k_origin), 0, 0, 1, 1},
   {&__pyx_n_s_os_path, __pyx_k_os_path, sizeof(__pyx_k_os_path), 0, 0, 1, 1},
   {&__pyx_n_s_parameter_text, __pyx_k_parameter_text, sizeof(__pyx_k_parameter_text), 0, 0, 1, 1},
-  {&__pyx_kp_s_parameter_text_string_parameter, __pyx_k_parameter_text_string_parameter, sizeof(__pyx_k_parameter_text_string_parameter), 0, 0, 1, 0},
+  {&__pyx_n_u_parameter_text, __pyx_k_parameter_text, sizeof(__pyx_k_parameter_text), 0, 1, 0, 1},
+  {&__pyx_kp_u_parameter_text_string_parameter, __pyx_k_parameter_text_string_parameter, sizeof(__pyx_k_parameter_text_string_parameter), 0, 1, 0, 0},
   {&__pyx_n_s_parameter_type, __pyx_k_parameter_type, sizeof(__pyx_k_parameter_type), 0, 0, 1, 1},
+  {&__pyx_n_u_parameter_type, __pyx_k_parameter_type, sizeof(__pyx_k_parameter_type), 0, 1, 0, 1},
   {&__pyx_kp_u_parameter_type_string, __pyx_k_parameter_type_string, sizeof(__pyx_k_parameter_type_string), 0, 1, 0, 0},
   {&__pyx_n_s_parameters, __pyx_k_parameters, sizeof(__pyx_k_parameters), 0, 0, 1, 1},
   {&__pyx_kp_u_params, __pyx_k_params, sizeof(__pyx_k_params), 0, 1, 0, 0},
-  {&__pyx_n_s_partnerBytesPerChar, __pyx_k_partnerBytesPerChar, sizeof(__pyx_k_partnerBytesPerChar), 0, 0, 1, 1},
-  {&__pyx_n_s_partnerCodepage, __pyx_k_partnerCodepage, sizeof(__pyx_k_partnerCodepage), 0, 0, 1, 1},
-  {&__pyx_n_s_partnerHost, __pyx_k_partnerHost, sizeof(__pyx_k_partnerHost), 0, 0, 1, 1},
-  {&__pyx_n_s_partnerIP, __pyx_k_partnerIP, sizeof(__pyx_k_partnerIP), 0, 0, 1, 1},
-  {&__pyx_n_s_partnerIPv6, __pyx_k_partnerIPv6, sizeof(__pyx_k_partnerIPv6), 0, 0, 1, 1},
-  {&__pyx_n_s_partnerRel, __pyx_k_partnerRel, sizeof(__pyx_k_partnerRel), 0, 0, 1, 1},
-  {&__pyx_n_s_partnerSystemCodepage, __pyx_k_partnerSystemCodepage, sizeof(__pyx_k_partnerSystemCodepage), 0, 0, 1, 1},
-  {&__pyx_n_s_partnerType, __pyx_k_partnerType, sizeof(__pyx_k_partnerType), 0, 0, 1, 1},
-  {&__pyx_n_s_patchLevel, __pyx_k_patchLevel, sizeof(__pyx_k_patchLevel), 0, 0, 1, 1},
+  {&__pyx_n_u_partnerBytesPerChar, __pyx_k_partnerBytesPerChar, sizeof(__pyx_k_partnerBytesPerChar), 0, 1, 0, 1},
+  {&__pyx_n_u_partnerCodepage, __pyx_k_partnerCodepage, sizeof(__pyx_k_partnerCodepage), 0, 1, 0, 1},
+  {&__pyx_n_u_partnerHost, __pyx_k_partnerHost, sizeof(__pyx_k_partnerHost), 0, 1, 0, 1},
+  {&__pyx_n_u_partnerIP, __pyx_k_partnerIP, sizeof(__pyx_k_partnerIP), 0, 1, 0, 1},
+  {&__pyx_n_u_partnerIPv6, __pyx_k_partnerIPv6, sizeof(__pyx_k_partnerIPv6), 0, 1, 0, 1},
+  {&__pyx_n_u_partnerRel, __pyx_k_partnerRel, sizeof(__pyx_k_partnerRel), 0, 1, 0, 1},
+  {&__pyx_n_u_partnerSystemCodepage, __pyx_k_partnerSystemCodepage, sizeof(__pyx_k_partnerSystemCodepage), 0, 1, 0, 1},
+  {&__pyx_n_u_partnerType, __pyx_k_partnerType, sizeof(__pyx_k_partnerType), 0, 1, 0, 1},
+  {&__pyx_n_u_patchLevel, __pyx_k_patchLevel, sizeof(__pyx_k_patchLevel), 0, 1, 0, 1},
   {&__pyx_n_s_patchlevel, __pyx_k_patchlevel, sizeof(__pyx_k_patchlevel), 0, 0, 1, 1},
   {&__pyx_n_s_pathName, __pyx_k_pathName, sizeof(__pyx_k_pathName), 0, 0, 1, 1},
   {&__pyx_n_s_path_name, __pyx_k_path_name, sizeof(__pyx_k_path_name), 0, 0, 1, 1},
-  {&__pyx_n_s_peakBusyCount, __pyx_k_peakBusyCount, sizeof(__pyx_k_peakBusyCount), 0, 0, 1, 1},
+  {&__pyx_n_u_peakBusyCount, __pyx_k_peakBusyCount, sizeof(__pyx_k_peakBusyCount), 0, 1, 0, 1},
   {&__pyx_n_s_platform, __pyx_k_platform, sizeof(__pyx_k_platform), 0, 0, 1, 1},
-  {&__pyx_n_s_port, __pyx_k_port, sizeof(__pyx_k_port), 0, 0, 1, 1},
+  {&__pyx_n_u_platform, __pyx_k_platform, sizeof(__pyx_k_platform), 0, 1, 0, 1},
+  {&__pyx_n_u_port, __pyx_k_port, sizeof(__pyx_k_port), 0, 1, 0, 1},
   {&__pyx_n_s_prepare, __pyx_k_prepare, sizeof(__pyx_k_prepare), 0, 0, 1, 1},
   {&__pyx_n_s_print, __pyx_k_print, sizeof(__pyx_k_print), 0, 0, 1, 1},
-  {&__pyx_n_s_progName, __pyx_k_progName, sizeof(__pyx_k_progName), 0, 0, 1, 1},
-  {&__pyx_n_s_program, __pyx_k_program, sizeof(__pyx_k_program), 0, 0, 1, 1},
-  {&__pyx_n_s_protocolType, __pyx_k_protocolType, sizeof(__pyx_k_protocolType), 0, 0, 1, 1},
+  {&__pyx_n_u_progName, __pyx_k_progName, sizeof(__pyx_k_progName), 0, 1, 0, 1},
+  {&__pyx_n_u_program, __pyx_k_program, sizeof(__pyx_k_program), 0, 1, 0, 1},
+  {&__pyx_n_u_protocolType, __pyx_k_protocolType, sizeof(__pyx_k_protocolType), 0, 1, 0, 1},
   {&__pyx_n_s_pyrfc__cyrfc, __pyx_k_pyrfc__cyrfc, sizeof(__pyx_k_pyrfc__cyrfc), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_vtable, __pyx_k_pyx_vtable, sizeof(__pyx_k_pyx_vtable), 0, 0, 1, 1},
   {&__pyx_n_s_qualname, __pyx_k_qualname, sizeof(__pyx_k_qualname), 0, 0, 1, 1},
   {&__pyx_n_s_queue_name, __pyx_k_queue_name, sizeof(__pyx_k_queue_name), 0, 0, 1, 1},
   {&__pyx_n_s_queue_names, __pyx_k_queue_names, sizeof(__pyx_k_queue_names), 0, 0, 1, 1},
   {&__pyx_n_s_queued, __pyx_k_queued, sizeof(__pyx_k_queued), 0, 0, 1, 1},
+  {&__pyx_n_u_queued, __pyx_k_queued, sizeof(__pyx_k_queued), 0, 1, 0, 1},
   {&__pyx_kp_u_raises_ABAPApplicationError, __pyx_k_raises_ABAPApplicationError, sizeof(__pyx_k_raises_ABAPApplicationError), 0, 1, 0, 0},
   {&__pyx_kp_u_raises_ABAPRuntimeError, __pyx_k_raises_ABAPRuntimeError, sizeof(__pyx_k_raises_ABAPRuntimeError), 0, 1, 0, 0},
   {&__pyx_kp_u_raises_ExternalRuntimeError, __pyx_k_raises_ExternalRuntimeError, sizeof(__pyx_k_raises_ExternalRuntimeError), 0, 1, 0, 0},
   {&__pyx_kp_u_raises_an_invalid_exception_Exc, __pyx_k_raises_an_invalid_exception_Exc, sizeof(__pyx_k_raises_an_invalid_exception_Exc), 0, 1, 0, 0},
   {&__pyx_n_s_range, __pyx_k_range, sizeof(__pyx_k_range), 0, 0, 1, 1},
   {&__pyx_n_s_rc, __pyx_k_rc, sizeof(__pyx_k_rc), 0, 0, 1, 1},
-  {&__pyx_n_s_receivedBytes, __pyx_k_receivedBytes, sizeof(__pyx_k_receivedBytes), 0, 0, 1, 1},
+  {&__pyx_n_u_receivedBytes, __pyx_k_receivedBytes, sizeof(__pyx_k_receivedBytes), 0, 1, 0, 1},
   {&__pyx_n_s_reduce, __pyx_k_reduce, sizeof(__pyx_k_reduce), 0, 0, 1, 1},
   {&__pyx_n_s_reduce_cython, __pyx_k_reduce_cython, sizeof(__pyx_k_reduce_cython), 0, 0, 1, 1},
   {&__pyx_n_s_reduce_ex, __pyx_k_reduce_ex, sizeof(__pyx_k_reduce_ex), 0, 0, 1, 1},
-  {&__pyx_n_s_registrationCount, __pyx_k_registrationCount, sizeof(__pyx_k_registrationCount), 0, 0, 1, 1},
+  {&__pyx_n_u_registrationCount, __pyx_k_registrationCount, sizeof(__pyx_k_registrationCount), 0, 1, 0, 1},
   {&__pyx_n_s_registry, __pyx_k_registry, sizeof(__pyx_k_registry), 0, 0, 1, 1},
-  {&__pyx_n_s_rel, __pyx_k_rel, sizeof(__pyx_k_rel), 0, 0, 1, 1},
+  {&__pyx_n_u_rel, __pyx_k_rel, sizeof(__pyx_k_rel), 0, 1, 0, 1},
   {&__pyx_n_s_reload_ini_file, __pyx_k_reload_ini_file, sizeof(__pyx_k_reload_ini_file), 0, 0, 1, 1},
   {&__pyx_n_s_remove, __pyx_k_remove, sizeof(__pyx_k_remove), 0, 0, 1, 1},
   {&__pyx_n_s_repr, __pyx_k_repr, sizeof(__pyx_k_repr), 0, 0, 1, 1},
   {&__pyx_n_s_request_context, __pyx_k_request_context, sizeof(__pyx_k_request_context), 0, 0, 1, 1},
   {&__pyx_kp_u_request_context_2, __pyx_k_request_context_2, sizeof(__pyx_k_request_context_2), 0, 1, 0, 0},
-  {&__pyx_n_s_reserved, __pyx_k_reserved, sizeof(__pyx_k_reserved), 0, 0, 1, 1},
-  {&__pyx_n_s_return_import_params, __pyx_k_return_import_params, sizeof(__pyx_k_return_import_params), 0, 0, 1, 1},
-  {&__pyx_n_s_rfcRole, __pyx_k_rfcRole, sizeof(__pyx_k_rfcRole), 0, 0, 1, 1},
-  {&__pyx_n_s_rollback, __pyx_k_rollback, sizeof(__pyx_k_rollback), 0, 0, 1, 1},
+  {&__pyx_n_u_reserved, __pyx_k_reserved, sizeof(__pyx_k_reserved), 0, 1, 0, 1},
+  {&__pyx_n_u_return_import_params, __pyx_k_return_import_params, sizeof(__pyx_k_return_import_params), 0, 1, 0, 1},
+  {&__pyx_n_u_rfcRole, __pyx_k_rfcRole, sizeof(__pyx_k_rfcRole), 0, 1, 0, 1},
+  {&__pyx_n_u_rollback, __pyx_k_rollback, sizeof(__pyx_k_rollback), 0, 1, 0, 1},
   {&__pyx_n_s_rolled_back, __pyx_k_rolled_back, sizeof(__pyx_k_rolled_back), 0, 0, 1, 1},
   {&__pyx_n_s_rsplit, __pyx_k_rsplit, sizeof(__pyx_k_rsplit), 0, 0, 1, 1},
   {&__pyx_n_s_rstrip, __pyx_k_rstrip, sizeof(__pyx_k_rstrip), 0, 0, 1, 1},
-  {&__pyx_kp_s_sapnwrfc_ini, __pyx_k_sapnwrfc_ini, sizeof(__pyx_k_sapnwrfc_ini), 0, 0, 1, 0},
-  {&__pyx_kp_s_sapnwrfc_ini_not_found_in, __pyx_k_sapnwrfc_ini_not_found_in, sizeof(__pyx_k_sapnwrfc_ini_not_found_in), 0, 0, 1, 0},
-  {&__pyx_kp_s_sapnwrfc_ini_path_is_not_a_strin, __pyx_k_sapnwrfc_ini_path_is_not_a_strin, sizeof(__pyx_k_sapnwrfc_ini_path_is_not_a_strin), 0, 0, 1, 0},
-  {&__pyx_n_s_sat_trace, __pyx_k_sat_trace, sizeof(__pyx_k_sat_trace), 0, 0, 1, 1},
+  {&__pyx_n_u_rstrip, __pyx_k_rstrip, sizeof(__pyx_k_rstrip), 0, 1, 0, 1},
+  {&__pyx_kp_u_sapnwrfc_ini, __pyx_k_sapnwrfc_ini, sizeof(__pyx_k_sapnwrfc_ini), 0, 1, 0, 0},
+  {&__pyx_kp_u_sapnwrfc_ini_not_found_in, __pyx_k_sapnwrfc_ini_not_found_in, sizeof(__pyx_k_sapnwrfc_ini_not_found_in), 0, 1, 0, 0},
+  {&__pyx_kp_u_sapnwrfc_ini_path_is_not_a_strin, __pyx_k_sapnwrfc_ini_path_is_not_a_strin, sizeof(__pyx_k_sapnwrfc_ini_path_is_not_a_strin), 0, 1, 0, 0},
+  {&__pyx_n_u_sat_trace, __pyx_k_sat_trace, sizeof(__pyx_k_sat_trace), 0, 1, 0, 1},
   {&__pyx_n_s_second, __pyx_k_second, sizeof(__pyx_k_second), 0, 0, 1, 1},
   {&__pyx_n_s_self, __pyx_k_self, sizeof(__pyx_k_self), 0, 0, 1, 1},
   {&__pyx_kp_s_self__handle_cannot_be_converted, __pyx_k_self__handle_cannot_be_converted, sizeof(__pyx_k_self__handle_cannot_be_converted), 0, 0, 1, 0},
   {&__pyx_kp_s_self__handle_self__tHandle_self, __pyx_k_self__handle_self__tHandle_self, sizeof(__pyx_k_self__handle_self__tHandle_self), 0, 0, 1, 0},
   {&__pyx_kp_s_self__throughput_handle_cannot_b, __pyx_k_self__throughput_handle_cannot_b, sizeof(__pyx_k_self__throughput_handle_cannot_b), 0, 0, 1, 0},
-  {&__pyx_n_s_sending_date, __pyx_k_sending_date, sizeof(__pyx_k_sending_date), 0, 0, 1, 1},
-  {&__pyx_n_s_sending_time, __pyx_k_sending_time, sizeof(__pyx_k_sending_time), 0, 0, 1, 1},
-  {&__pyx_n_s_sentBytes, __pyx_k_sentBytes, sizeof(__pyx_k_sentBytes), 0, 0, 1, 1},
-  {&__pyx_n_s_serializationTime, __pyx_k_serializationTime, sizeof(__pyx_k_serializationTime), 0, 0, 1, 1},
+  {&__pyx_n_u_sending_date, __pyx_k_sending_date, sizeof(__pyx_k_sending_date), 0, 1, 0, 1},
+  {&__pyx_n_u_sending_time, __pyx_k_sending_time, sizeof(__pyx_k_sending_time), 0, 1, 0, 1},
+  {&__pyx_n_u_sentBytes, __pyx_k_sentBytes, sizeof(__pyx_k_sentBytes), 0, 1, 0, 1},
+  {&__pyx_n_u_serializationTime, __pyx_k_serializationTime, sizeof(__pyx_k_serializationTime), 0, 1, 0, 1},
   {&__pyx_n_s_serve, __pyx_k_serve, sizeof(__pyx_k_serve), 0, 0, 1, 1},
-  {&__pyx_n_s_server, __pyx_k_server, sizeof(__pyx_k_server), 0, 0, 1, 1},
-  {&__pyx_n_s_serverName, __pyx_k_serverName, sizeof(__pyx_k_serverName), 0, 0, 1, 1},
+  {&__pyx_n_u_server, __pyx_k_server, sizeof(__pyx_k_server), 0, 1, 0, 1},
+  {&__pyx_n_u_serverName, __pyx_k_serverName, sizeof(__pyx_k_serverName), 0, 1, 0, 1},
   {&__pyx_n_s_server_context, __pyx_k_server_context, sizeof(__pyx_k_server_context), 0, 0, 1, 1},
+  {&__pyx_n_u_server_context, __pyx_k_server_context, sizeof(__pyx_k_server_context), 0, 1, 0, 1},
   {&__pyx_n_s_server_functions, __pyx_k_server_functions, sizeof(__pyx_k_server_functions), 0, 0, 1, 1},
   {&__pyx_n_s_server_log, __pyx_k_server_log, sizeof(__pyx_k_server_log), 0, 0, 1, 1},
-  {&__pyx_n_s_server_log_2, __pyx_k_server_log_2, sizeof(__pyx_k_server_log_2), 0, 0, 1, 1},
+  {&__pyx_n_u_server_log_2, __pyx_k_server_log_2, sizeof(__pyx_k_server_log_2), 0, 1, 0, 1},
   {&__pyx_n_s_server_params, __pyx_k_server_params, sizeof(__pyx_k_server_params), 0, 0, 1, 1},
   {&__pyx_n_s_setOnConnection, __pyx_k_setOnConnection, sizeof(__pyx_k_setOnConnection), 0, 0, 1, 1},
   {&__pyx_n_s_set_cryptolib_path, __pyx_k_set_cryptolib_path, sizeof(__pyx_k_set_cryptolib_path), 0, 0, 1, 1},
   {&__pyx_n_s_set_ini_file_directory, __pyx_k_set_ini_file_directory, sizeof(__pyx_k_set_ini_file_directory), 0, 0, 1, 1},
   {&__pyx_n_s_set_locale_radix, __pyx_k_set_locale_radix, sizeof(__pyx_k_set_locale_radix), 0, 0, 1, 1},
   {&__pyx_n_s_setstate, __pyx_k_setstate, sizeof(__pyx_k_setstate), 0, 0, 1, 1},
   {&__pyx_n_s_setstate_cython, __pyx_k_setstate_cython, sizeof(__pyx_k_setstate_cython), 0, 0, 1, 1},
   {&__pyx_kp_u_should_be_from_1_30_chars, __pyx_k_should_be_from_1_30_chars, sizeof(__pyx_k_should_be_from_1_30_chars), 0, 1, 0, 0},
   {&__pyx_kp_u_should_be_from_1_30_chars_2, __pyx_k_should_be_from_1_30_chars_2, sizeof(__pyx_k_should_be_from_1_30_chars_2), 0, 1, 0, 0},
   {&__pyx_n_s_socket, __pyx_k_socket, sizeof(__pyx_k_socket), 0, 0, 1, 1},
   {&__pyx_kp_s_src_pyrfc__cyrfc_pyx, __pyx_k_src_pyrfc__cyrfc_pyx, sizeof(__pyx_k_src_pyrfc__cyrfc_pyx), 0, 0, 1, 0},
   {&__pyx_n_s_start, __pyx_k_start, sizeof(__pyx_k_start), 0, 0, 1, 1},
-  {&__pyx_n_s_state, __pyx_k_state, sizeof(__pyx_k_state), 0, 0, 1, 1},
+  {&__pyx_n_u_state, __pyx_k_state, sizeof(__pyx_k_state), 0, 1, 0, 1},
   {&__pyx_n_s_staticmethod, __pyx_k_staticmethod, sizeof(__pyx_k_staticmethod), 0, 0, 1, 1},
   {&__pyx_n_s_stop, __pyx_k_stop, sizeof(__pyx_k_stop), 0, 0, 1, 1},
   {&__pyx_kp_s_stringsource, __pyx_k_stringsource, sizeof(__pyx_k_stringsource), 0, 0, 1, 0},
   {&__pyx_n_s_strptime, __pyx_k_strptime, sizeof(__pyx_k_strptime), 0, 0, 1, 1},
   {&__pyx_n_s_synchronous, __pyx_k_synchronous, sizeof(__pyx_k_synchronous), 0, 0, 1, 1},
   {&__pyx_n_s_sys, __pyx_k_sys, sizeof(__pyx_k_sys), 0, 0, 1, 1},
   {&__pyx_n_s_sysId, __pyx_k_sysId, sizeof(__pyx_k_sysId), 0, 0, 1, 1},
-  {&__pyx_n_s_sysNumber, __pyx_k_sysNumber, sizeof(__pyx_k_sysNumber), 0, 0, 1, 1},
+  {&__pyx_n_u_sysId, __pyx_k_sysId, sizeof(__pyx_k_sysId), 0, 1, 0, 1},
+  {&__pyx_n_u_sysNumber, __pyx_k_sysNumber, sizeof(__pyx_k_sysNumber), 0, 1, 0, 1},
   {&__pyx_n_s_sysid, __pyx_k_sysid, sizeof(__pyx_k_sysid), 0, 0, 1, 1},
   {&__pyx_n_s_t, __pyx_k_t, sizeof(__pyx_k_t), 0, 0, 1, 1},
-  {&__pyx_n_s_t_code, __pyx_k_t_code, sizeof(__pyx_k_t_code), 0, 0, 1, 1},
+  {&__pyx_n_u_t_code, __pyx_k_t_code, sizeof(__pyx_k_t_code), 0, 1, 0, 1},
   {&__pyx_n_s_target, __pyx_k_target, sizeof(__pyx_k_target), 0, 0, 1, 1},
   {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
   {&__pyx_n_s_threading, __pyx_k_threading, sizeof(__pyx_k_threading), 0, 0, 1, 1},
   {&__pyx_n_s_throughput, __pyx_k_throughput, sizeof(__pyx_k_throughput), 0, 0, 1, 1},
   {&__pyx_n_s_time, __pyx_k_time, sizeof(__pyx_k_time), 0, 0, 1, 1},
-  {&__pyx_kp_s_time_value_required_received, __pyx_k_time_value_required_received, sizeof(__pyx_k_time_value_required_received), 0, 0, 1, 0},
-  {&__pyx_n_s_timeout, __pyx_k_timeout, sizeof(__pyx_k_timeout), 0, 0, 1, 1},
-  {&__pyx_n_s_totalTime, __pyx_k_totalTime, sizeof(__pyx_k_totalTime), 0, 0, 1, 1},
-  {&__pyx_n_s_trace, __pyx_k_trace, sizeof(__pyx_k_trace), 0, 0, 1, 1},
+  {&__pyx_kp_u_time_value_required_received, __pyx_k_time_value_required_received, sizeof(__pyx_k_time_value_required_received), 0, 1, 0, 0},
+  {&__pyx_n_u_timeout, __pyx_k_timeout, sizeof(__pyx_k_timeout), 0, 1, 0, 1},
+  {&__pyx_n_u_totalTime, __pyx_k_totalTime, sizeof(__pyx_k_totalTime), 0, 1, 0, 1},
+  {&__pyx_n_u_trace, __pyx_k_trace, sizeof(__pyx_k_trace), 0, 1, 0, 1},
   {&__pyx_n_s_traceback, __pyx_k_traceback, sizeof(__pyx_k_traceback), 0, 0, 1, 1},
   {&__pyx_n_s_transaction_id, __pyx_k_transaction_id, sizeof(__pyx_k_transaction_id), 0, 0, 1, 1},
   {&__pyx_n_s_transactional, __pyx_k_transactional, sizeof(__pyx_k_transactional), 0, 0, 1, 1},
   {&__pyx_n_s_type, __pyx_k_type, sizeof(__pyx_k_type), 0, 0, 1, 1},
+  {&__pyx_n_u_type, __pyx_k_type, sizeof(__pyx_k_type), 0, 1, 0, 1},
   {&__pyx_n_s_type_description, __pyx_k_type_description, sizeof(__pyx_k_type_description), 0, 0, 1, 1},
+  {&__pyx_n_u_type_description, __pyx_k_type_description, sizeof(__pyx_k_type_description), 0, 1, 0, 1},
   {&__pyx_n_s_type_name, __pyx_k_type_name, sizeof(__pyx_k_type_name), 0, 0, 1, 1},
   {&__pyx_n_s_uc_length, __pyx_k_uc_length, sizeof(__pyx_k_uc_length), 0, 0, 1, 1},
+  {&__pyx_n_u_uc_length, __pyx_k_uc_length, sizeof(__pyx_k_uc_length), 0, 1, 0, 1},
   {&__pyx_n_s_uc_offset, __pyx_k_uc_offset, sizeof(__pyx_k_uc_offset), 0, 0, 1, 1},
+  {&__pyx_n_u_uc_offset, __pyx_k_uc_offset, sizeof(__pyx_k_uc_offset), 0, 1, 0, 1},
   {&__pyx_n_s_uclang_iso, __pyx_k_uclang_iso, sizeof(__pyx_k_uclang_iso), 0, 0, 1, 1},
   {&__pyx_n_s_uclang_sap, __pyx_k_uclang_sap, sizeof(__pyx_k_uclang_sap), 0, 0, 1, 1},
   {&__pyx_n_s_unit, __pyx_k_unit, sizeof(__pyx_k_unit), 0, 0, 1, 1},
-  {&__pyx_n_s_unit_attributes, __pyx_k_unit_attributes, sizeof(__pyx_k_unit_attributes), 0, 0, 1, 1},
-  {&__pyx_n_s_unit_history, __pyx_k_unit_history, sizeof(__pyx_k_unit_history), 0, 0, 1, 1},
+  {&__pyx_n_u_unit_attributes, __pyx_k_unit_attributes, sizeof(__pyx_k_unit_attributes), 0, 1, 0, 1},
+  {&__pyx_n_u_unit_history, __pyx_k_unit_history, sizeof(__pyx_k_unit_history), 0, 1, 0, 1},
   {&__pyx_n_s_unit_id, __pyx_k_unit_id, sizeof(__pyx_k_unit_id), 0, 0, 1, 1},
-  {&__pyx_n_s_unit_identifier, __pyx_k_unit_identifier, sizeof(__pyx_k_unit_identifier), 0, 0, 1, 1},
+  {&__pyx_n_u_unit_identifier, __pyx_k_unit_identifier, sizeof(__pyx_k_unit_identifier), 0, 1, 0, 1},
   {&__pyx_n_s_update, __pyx_k_update, sizeof(__pyx_k_update), 0, 0, 1, 1},
   {&__pyx_n_s_upper, __pyx_k_upper, sizeof(__pyx_k_upper), 0, 0, 1, 1},
-  {&__pyx_n_s_user, __pyx_k_user, sizeof(__pyx_k_user), 0, 0, 1, 1},
+  {&__pyx_n_u_user, __pyx_k_user, sizeof(__pyx_k_user), 0, 1, 0, 1},
   {&__pyx_n_s_utcnow, __pyx_k_utcnow, sizeof(__pyx_k_utcnow), 0, 0, 1, 1},
   {&__pyx_n_s_utils, __pyx_k_utils, sizeof(__pyx_k_utils), 0, 0, 1, 1},
   {&__pyx_n_s_value, __pyx_k_value, sizeof(__pyx_k_value), 0, 0, 1, 1},
+  {&__pyx_kp_u_when_filling, __pyx_k_when_filling, sizeof(__pyx_k_when_filling), 0, 1, 0, 0},
   {&__pyx_kp_u_when_getting_server_context_for, __pyx_k_when_getting_server_context_for, sizeof(__pyx_k_when_getting_server_context_for), 0, 1, 0, 0},
+  {&__pyx_kp_u_when_wrapping, __pyx_k_when_wrapping, sizeof(__pyx_k_when_wrapping), 0, 1, 0, 0},
   {&__pyx_kp_u_with, __pyx_k_with, sizeof(__pyx_k_with), 0, 1, 0, 0},
   {&__pyx_n_s_wrap, __pyx_k_wrap, sizeof(__pyx_k_wrap), 0, 0, 1, 1},
-  {&__pyx_kp_s_wrapString_uclen_u_utf8_size_u, __pyx_k_wrapString_uclen_u_utf8_size_u, sizeof(__pyx_k_wrapString_uclen_u_utf8_size_u), 0, 0, 1, 0},
+  {&__pyx_kp_u_wrapString_uclen_u_utf8_size_u, __pyx_k_wrapString_uclen_u_utf8_size_u, sizeof(__pyx_k_wrapString_uclen_u_utf8_size_u), 0, 1, 0, 0},
   {&__pyx_n_s_year, __pyx_k_year, sizeof(__pyx_k_year), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_object = __Pyx_GetBuiltinName(__pyx_n_s_object); if (!__pyx_builtin_object) __PYX_ERR(0, 312, __pyx_L1_error)
   __pyx_builtin_staticmethod = __Pyx_GetBuiltinName(__pyx_n_s_staticmethod); if (!__pyx_builtin_staticmethod) __PYX_ERR(0, 2231, __pyx_L1_error)
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(0, 132, __pyx_L1_error)
   __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 301, __pyx_L1_error)
   __pyx_builtin_enumerate = __Pyx_GetBuiltinName(__pyx_n_s_enumerate); if (!__pyx_builtin_enumerate) __PYX_ERR(0, 1145, __pyx_L1_error)
+  __pyx_builtin_print = __Pyx_GetBuiltinName(__pyx_n_s_print); if (!__pyx_builtin_print) __PYX_ERR(0, 1243, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
@@ -42186,59 +42966,59 @@
   /* "pyrfc/_cyrfc.pyx":460
  *             raise TypeError(f"'default_value' (string) '{default_value}' must not exceed 30 chars.")
  *         if len(parameter_text)>79:
  *             raise TypeError("'parameter_text' (string) '{parameter_text}' must not exceed 79 chars.")             # <<<<<<<<<<<<<<
  *         self.parameters.append({
  *             'name': name,
  */
-  __pyx_tuple__7 = PyTuple_Pack(1, __pyx_kp_s_parameter_text_string_parameter); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 460, __pyx_L1_error)
+  __pyx_tuple__7 = PyTuple_Pack(1, __pyx_kp_u_parameter_text_string_parameter); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 460, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__7);
   __Pyx_GIVEREF(__pyx_tuple__7);
 
   /* "pyrfc/_cyrfc.pyx":599
  *                 raise RFCError(f"Connection configuration option '{k}' is not supported")
  *         self.__config = {}
  *         self.__config['dtime'] = config.get('dtime', False)             # <<<<<<<<<<<<<<
  *         self.__config['return_import_params'] = config.get('return_import_params', False)
  *         self.__config['rstrip'] = config.get('rstrip', True)
  */
-  __pyx_tuple__8 = PyTuple_Pack(2, __pyx_n_s_dtime, Py_False); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 599, __pyx_L1_error)
+  __pyx_tuple__8 = PyTuple_Pack(2, __pyx_n_u_dtime, Py_False); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 599, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
 
   /* "pyrfc/_cyrfc.pyx":600
  *         self.__config = {}
  *         self.__config['dtime'] = config.get('dtime', False)
  *         self.__config['return_import_params'] = config.get('return_import_params', False)             # <<<<<<<<<<<<<<
  *         self.__config['rstrip'] = config.get('rstrip', True)
  *         self.__config['timeout'] = config.get('timeout', None)
  */
-  __pyx_tuple__9 = PyTuple_Pack(2, __pyx_n_s_return_import_params, Py_False); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 600, __pyx_L1_error)
+  __pyx_tuple__9 = PyTuple_Pack(2, __pyx_n_u_return_import_params, Py_False); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 600, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
 
   /* "pyrfc/_cyrfc.pyx":601
  *         self.__config['dtime'] = config.get('dtime', False)
  *         self.__config['return_import_params'] = config.get('return_import_params', False)
  *         self.__config['rstrip'] = config.get('rstrip', True)             # <<<<<<<<<<<<<<
  *         self.__config['timeout'] = config.get('timeout', None)
  * 
  */
-  __pyx_tuple__10 = PyTuple_Pack(2, __pyx_n_s_rstrip, Py_True); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(0, 601, __pyx_L1_error)
+  __pyx_tuple__10 = PyTuple_Pack(2, __pyx_n_u_rstrip, Py_True); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(0, 601, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__10);
   __Pyx_GIVEREF(__pyx_tuple__10);
 
   /* "pyrfc/_cyrfc.pyx":602
  *         self.__config['return_import_params'] = config.get('return_import_params', False)
  *         self.__config['rstrip'] = config.get('rstrip', True)
  *         self.__config['timeout'] = config.get('timeout', None)             # <<<<<<<<<<<<<<
  * 
  *         # set internal configuration
  */
-  __pyx_tuple__11 = PyTuple_Pack(2, __pyx_n_s_timeout, Py_None); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(0, 602, __pyx_L1_error)
+  __pyx_tuple__11 = PyTuple_Pack(2, __pyx_n_u_timeout, Py_None); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(0, 602, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__11);
   __Pyx_GIVEREF(__pyx_tuple__11);
 
   /* "pyrfc/_cyrfc.pyx":1190
  *             if 'user' in attributes and attributes['user'] is not None:
  *                 # (SAP_UC[12+1]) Sender User (optional). Default is current operating system User.
  *                 sapuc = fillString(attributes['user'][0:12])             # <<<<<<<<<<<<<<
@@ -42278,507 +43058,518 @@
  *                 strncpyU(unitAttr.program, sapuc, len(attributes['program'][0:40]) + 1)
  *                 free(sapuc)
  */
   __pyx_slice__15 = PySlice_New(__pyx_int_0, __pyx_int_40, Py_None); if (unlikely(!__pyx_slice__15)) __PYX_ERR(0, 1205, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_slice__15);
   __Pyx_GIVEREF(__pyx_slice__15);
 
+  /* "pyrfc/_cyrfc.pyx":1243
+ *                     RfcDestroyFunction(funcCont, NULL)
+ *             # execute
+ *             print (" Invocation finished. submitting unit.")             # <<<<<<<<<<<<<<
+ *             with nogil:
+ *                 rc = RfcSubmitUnit(self._uHandle, &errorInfo)
+ */
+  __pyx_tuple__16 = PyTuple_Pack(1, __pyx_kp_u_Invocation_finished_submitting); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(0, 1243, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__16);
+  __Pyx_GIVEREF(__pyx_tuple__16);
+
   /* "pyrfc/_cyrfc.pyx":1388
  * 
  *         if type(unit) is not dict or 'id' not in unit or 'background' not in unit:
  *             raise TypeError("Parameter 'unit' not valid. Please use initialize_unit() to retrieve a valid unit.")             # <<<<<<<<<<<<<<
  *         if not isinstance(calls, Iterable):
  *             raise TypeError("Parameter 'calls' must be iterable.")
  */
-  __pyx_tuple__16 = PyTuple_Pack(1, __pyx_kp_s_Parameter_unit_not_valid_Please); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(0, 1388, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__16);
-  __Pyx_GIVEREF(__pyx_tuple__16);
+  __pyx_tuple__17 = PyTuple_Pack(1, __pyx_kp_u_Parameter_unit_not_valid_Please); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(0, 1388, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__17);
+  __Pyx_GIVEREF(__pyx_tuple__17);
 
   /* "pyrfc/_cyrfc.pyx":1390
  *             raise TypeError("Parameter 'unit' not valid. Please use initialize_unit() to retrieve a valid unit.")
  *         if not isinstance(calls, Iterable):
  *             raise TypeError("Parameter 'calls' must be iterable.")             # <<<<<<<<<<<<<<
  *         if len(calls)==0:
  *             raise TypeError("Parameter 'calls' must contain at least on call description (func_name, params).")
  */
-  __pyx_tuple__17 = PyTuple_Pack(1, __pyx_kp_s_Parameter_calls_must_be_iterable); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(0, 1390, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__17);
-  __Pyx_GIVEREF(__pyx_tuple__17);
+  __pyx_tuple__18 = PyTuple_Pack(1, __pyx_kp_u_Parameter_calls_must_be_iterable); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(0, 1390, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__18);
+  __Pyx_GIVEREF(__pyx_tuple__18);
 
   /* "pyrfc/_cyrfc.pyx":1392
  *             raise TypeError("Parameter 'calls' must be iterable.")
  *         if len(calls)==0:
  *             raise TypeError("Parameter 'calls' must contain at least on call description (func_name, params).")             # <<<<<<<<<<<<<<
  *         for func_name, params in calls:
  *             if type(func_name) is not str or type(params) is not dict:
  */
-  __pyx_tuple__18 = PyTuple_Pack(1, __pyx_kp_s_Parameter_calls_must_contain_at); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(0, 1392, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__18);
-  __Pyx_GIVEREF(__pyx_tuple__18);
+  __pyx_tuple__19 = PyTuple_Pack(1, __pyx_kp_u_Parameter_calls_must_contain_at); if (unlikely(!__pyx_tuple__19)) __PYX_ERR(0, 1392, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__19);
+  __Pyx_GIVEREF(__pyx_tuple__19);
 
   /* "pyrfc/_cyrfc.pyx":1395
  *         for func_name, params in calls:
  *             if type(func_name) is not str or type(params) is not dict:
  *                 raise TypeError("Parameter 'calls' must contain valid call descriptions (func_name, params dict).")             # <<<<<<<<<<<<<<
  *         if self.active_unit:
  *             raise RFCError("There is an active unit for this connection. "
  */
-  __pyx_tuple__19 = PyTuple_Pack(1, __pyx_kp_s_Parameter_calls_must_contain_val); if (unlikely(!__pyx_tuple__19)) __PYX_ERR(0, 1395, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__19);
-  __Pyx_GIVEREF(__pyx_tuple__19);
+  __pyx_tuple__20 = PyTuple_Pack(1, __pyx_kp_u_Parameter_calls_must_contain_val); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(0, 1395, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__20);
+  __Pyx_GIVEREF(__pyx_tuple__20);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("self._handle,self._tHandle,self._uHandle cannot be converted to a Python object for pickling")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("self._handle,self._tHandle,self._uHandle cannot be converted to a Python object for pickling")
  */
-  __pyx_tuple__21 = PyTuple_Pack(1, __pyx_kp_s_self__handle_self__tHandle_self); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(1, 2, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__21);
-  __Pyx_GIVEREF(__pyx_tuple__21);
+  __pyx_tuple__22 = PyTuple_Pack(1, __pyx_kp_s_self__handle_self__tHandle_self); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(1, 2, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__22);
+  __Pyx_GIVEREF(__pyx_tuple__22);
 
   /* "(tree fragment)":4
  *     raise TypeError("self._handle,self._tHandle,self._uHandle cannot be converted to a Python object for pickling")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("self._handle,self._tHandle,self._uHandle cannot be converted to a Python object for pickling")             # <<<<<<<<<<<<<<
  */
-  __pyx_tuple__22 = PyTuple_Pack(1, __pyx_kp_s_self__handle_self__tHandle_self); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(1, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__22);
-  __Pyx_GIVEREF(__pyx_tuple__22);
+  __pyx_tuple__23 = PyTuple_Pack(1, __pyx_kp_s_self__handle_self__tHandle_self); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__23);
+  __Pyx_GIVEREF(__pyx_tuple__23);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("self._handle cannot be converted to a Python object for pickling")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("self._handle cannot be converted to a Python object for pickling")
  */
-  __pyx_tuple__25 = PyTuple_Pack(1, __pyx_kp_s_self__handle_cannot_be_converted); if (unlikely(!__pyx_tuple__25)) __PYX_ERR(1, 2, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__25);
-  __Pyx_GIVEREF(__pyx_tuple__25);
+  __pyx_tuple__26 = PyTuple_Pack(1, __pyx_kp_s_self__handle_cannot_be_converted); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(1, 2, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__26);
+  __Pyx_GIVEREF(__pyx_tuple__26);
 
   /* "(tree fragment)":4
  *     raise TypeError("self._handle cannot be converted to a Python object for pickling")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("self._handle cannot be converted to a Python object for pickling")             # <<<<<<<<<<<<<<
  */
-  __pyx_tuple__26 = PyTuple_Pack(1, __pyx_kp_s_self__handle_cannot_be_converted); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(1, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__26);
-  __Pyx_GIVEREF(__pyx_tuple__26);
+  __pyx_tuple__27 = PyTuple_Pack(1, __pyx_kp_s_self__handle_cannot_be_converted); if (unlikely(!__pyx_tuple__27)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__27);
+  __Pyx_GIVEREF(__pyx_tuple__27);
 
   /* "pyrfc/_cyrfc.pyx":1705
  *         return RFC_ABAP_EXCEPTION
  *     except Exception as ex:
  *         exctype, value = exc_info()[:2]             # <<<<<<<<<<<<<<
  *         _server_log(
  *             "genericHandler",
  */
-  __pyx_slice__29 = PySlice_New(Py_None, __pyx_int_2, Py_None); if (unlikely(!__pyx_slice__29)) __PYX_ERR(0, 1705, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_slice__29);
-  __Pyx_GIVEREF(__pyx_slice__29);
+  __pyx_slice__30 = PySlice_New(Py_None, __pyx_int_2, Py_None); if (unlikely(!__pyx_slice__30)) __PYX_ERR(0, 1705, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_slice__30);
+  __Pyx_GIVEREF(__pyx_slice__30);
 
   /* "pyrfc/_cyrfc.pyx":1772
  *         # config parsing
  *         config = config or {}
  *         self.debug = config.get('debug', False)             # <<<<<<<<<<<<<<
  *         self.rstrip = config.get('rstrip', True)
  *         server_context["server_log"] = config.get("server_log", False)
  */
-  __pyx_tuple__30 = PyTuple_Pack(2, __pyx_n_s_debug, Py_False); if (unlikely(!__pyx_tuple__30)) __PYX_ERR(0, 1772, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__30);
-  __Pyx_GIVEREF(__pyx_tuple__30);
+  __pyx_tuple__31 = PyTuple_Pack(2, __pyx_n_u_debug, Py_False); if (unlikely(!__pyx_tuple__31)) __PYX_ERR(0, 1772, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__31);
+  __Pyx_GIVEREF(__pyx_tuple__31);
 
   /* "pyrfc/_cyrfc.pyx":1774
  *         self.debug = config.get('debug', False)
  *         self.rstrip = config.get('rstrip', True)
  *         server_context["server_log"] = config.get("server_log", False)             # <<<<<<<<<<<<<<
  *         server_context["auth_check"] = config.get("auth_check", default_auth_check)
  *         server_context["port"] = config.get("port", 8080)
  */
-  __pyx_tuple__31 = PyTuple_Pack(2, __pyx_n_s_server_log_2, Py_False); if (unlikely(!__pyx_tuple__31)) __PYX_ERR(0, 1774, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__31);
-  __Pyx_GIVEREF(__pyx_tuple__31);
+  __pyx_tuple__32 = PyTuple_Pack(2, __pyx_n_u_server_log_2, Py_False); if (unlikely(!__pyx_tuple__32)) __PYX_ERR(0, 1774, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__32);
+  __Pyx_GIVEREF(__pyx_tuple__32);
 
   /* "pyrfc/_cyrfc.pyx":1776
  *         server_context["server_log"] = config.get("server_log", False)
  *         server_context["auth_check"] = config.get("auth_check", default_auth_check)
  *         server_context["port"] = config.get("port", 8080)             # <<<<<<<<<<<<<<
  * 
  *         self._client_connection = Connection(**client_params)
  */
-  __pyx_tuple__32 = PyTuple_Pack(2, __pyx_n_s_port, __pyx_int_8080); if (unlikely(!__pyx_tuple__32)) __PYX_ERR(0, 1776, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__32);
-  __Pyx_GIVEREF(__pyx_tuple__32);
+  __pyx_tuple__33 = PyTuple_Pack(2, __pyx_n_u_port, __pyx_int_8080); if (unlikely(!__pyx_tuple__33)) __PYX_ERR(0, 1776, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__33);
+  __Pyx_GIVEREF(__pyx_tuple__33);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_tuple__33 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__33)) __PYX_ERR(1, 2, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__33);
-  __Pyx_GIVEREF(__pyx_tuple__33);
+  __pyx_tuple__34 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__34)) __PYX_ERR(1, 2, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__34);
+  __Pyx_GIVEREF(__pyx_tuple__34);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_tuple__34 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__34)) __PYX_ERR(1, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__34);
-  __Pyx_GIVEREF(__pyx_tuple__34);
+  __pyx_tuple__35 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__35)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__35);
+  __Pyx_GIVEREF(__pyx_tuple__35);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("self._throughput_handle cannot be converted to a Python object for pickling")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("self._throughput_handle cannot be converted to a Python object for pickling")
  */
-  __pyx_tuple__35 = PyTuple_Pack(1, __pyx_kp_s_self__throughput_handle_cannot_b); if (unlikely(!__pyx_tuple__35)) __PYX_ERR(1, 2, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__35);
-  __Pyx_GIVEREF(__pyx_tuple__35);
+  __pyx_tuple__36 = PyTuple_Pack(1, __pyx_kp_s_self__throughput_handle_cannot_b); if (unlikely(!__pyx_tuple__36)) __PYX_ERR(1, 2, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__36);
+  __Pyx_GIVEREF(__pyx_tuple__36);
 
   /* "(tree fragment)":4
  *     raise TypeError("self._throughput_handle cannot be converted to a Python object for pickling")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("self._throughput_handle cannot be converted to a Python object for pickling")             # <<<<<<<<<<<<<<
  */
-  __pyx_tuple__36 = PyTuple_Pack(1, __pyx_kp_s_self__throughput_handle_cannot_b); if (unlikely(!__pyx_tuple__36)) __PYX_ERR(1, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__36);
-  __Pyx_GIVEREF(__pyx_tuple__36);
+  __pyx_tuple__37 = PyTuple_Pack(1, __pyx_kp_s_self__throughput_handle_cannot_b); if (unlikely(!__pyx_tuple__37)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__37);
+  __Pyx_GIVEREF(__pyx_tuple__37);
 
   /* "pyrfc/_cyrfc.pyx":2512
  *                         else:
  *                             if len(value.rstrip()) > 0:
  *                                 date(int(value[:4]), int(value[4:6]), int(value[6:8]))             # <<<<<<<<<<<<<<
  *                             cValue = fillString(value)
  *                     except Exception as ex:
  */
-  __pyx_slice__37 = PySlice_New(Py_None, __pyx_int_4, Py_None); if (unlikely(!__pyx_slice__37)) __PYX_ERR(0, 2512, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_slice__37);
-  __Pyx_GIVEREF(__pyx_slice__37);
-  __pyx_slice__38 = PySlice_New(__pyx_int_4, __pyx_int_6, Py_None); if (unlikely(!__pyx_slice__38)) __PYX_ERR(0, 2512, __pyx_L1_error)
+  __pyx_slice__38 = PySlice_New(Py_None, __pyx_int_4, Py_None); if (unlikely(!__pyx_slice__38)) __PYX_ERR(0, 2512, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_slice__38);
   __Pyx_GIVEREF(__pyx_slice__38);
-  __pyx_slice__39 = PySlice_New(__pyx_int_6, __pyx_int_8, Py_None); if (unlikely(!__pyx_slice__39)) __PYX_ERR(0, 2512, __pyx_L1_error)
+  __pyx_slice__39 = PySlice_New(__pyx_int_4, __pyx_int_6, Py_None); if (unlikely(!__pyx_slice__39)) __PYX_ERR(0, 2512, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_slice__39);
   __Pyx_GIVEREF(__pyx_slice__39);
+  __pyx_slice__40 = PySlice_New(__pyx_int_6, __pyx_int_8, Py_None); if (unlikely(!__pyx_slice__40)) __PYX_ERR(0, 2512, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_slice__40);
+  __Pyx_GIVEREF(__pyx_slice__40);
 
   /* "pyrfc/_cyrfc.pyx":2533
  *                         else:
  *                             if len(value.rstrip()) > 0:
  *                                 time(int(value[:2]), int(value[2:4]), int(value[4:6]))             # <<<<<<<<<<<<<<
  *                             cValue = fillString(value)
  *                     except Exception as ex:
  */
-  __pyx_slice__40 = PySlice_New(__pyx_int_2, __pyx_int_4, Py_None); if (unlikely(!__pyx_slice__40)) __PYX_ERR(0, 2533, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_slice__40);
-  __Pyx_GIVEREF(__pyx_slice__40);
+  __pyx_slice__41 = PySlice_New(__pyx_int_2, __pyx_int_4, Py_None); if (unlikely(!__pyx_slice__41)) __PYX_ERR(0, 2533, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_slice__41);
+  __Pyx_GIVEREF(__pyx_slice__41);
 
   /* "pyrfc/_cyrfc.pyx":2578
  *     if exception.message:  # fixed length, exactly 512 chars
  *         # str = exception.message[0:512].ljust(512)
  *         str = exception.message[0:512]             # <<<<<<<<<<<<<<
  *         sapuc = fillString(str)
  *         strncpyU(errorInfo.message, sapuc, min(len(str)+1, 512))
  */
-  __pyx_slice__41 = PySlice_New(__pyx_int_0, __pyx_int_512, Py_None); if (unlikely(!__pyx_slice__41)) __PYX_ERR(0, 2578, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_slice__41);
-  __Pyx_GIVEREF(__pyx_slice__41);
+  __pyx_slice__42 = PySlice_New(__pyx_int_0, __pyx_int_512, Py_None); if (unlikely(!__pyx_slice__42)) __PYX_ERR(0, 2578, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_slice__42);
+  __Pyx_GIVEREF(__pyx_slice__42);
 
   /* "pyrfc/_cyrfc.pyx":2584
  *     errorInfo.code = exception.code if exception.code else RFC_UNKNOWN_ERROR
  *     if exception.key:  # fixed length, exactly 128 chars
  *         str = exception.key[0:128]             # <<<<<<<<<<<<<<
  *         sapuc = fillString(str)
  *         strncpyU(errorInfo.key, sapuc, min(len(str)+1, 128))
  */
-  __pyx_slice__42 = PySlice_New(__pyx_int_0, __pyx_int_128, Py_None); if (unlikely(!__pyx_slice__42)) __PYX_ERR(0, 2584, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_slice__42);
-  __Pyx_GIVEREF(__pyx_slice__42);
+  __pyx_slice__43 = PySlice_New(__pyx_int_0, __pyx_int_128, Py_None); if (unlikely(!__pyx_slice__43)) __PYX_ERR(0, 2584, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_slice__43);
+  __Pyx_GIVEREF(__pyx_slice__43);
 
   /* "pyrfc/_cyrfc.pyx":2593
  *         free(sapuc)
  *     if exception.msg_type:
  *         sapuc = fillString(exception.msg_type[0:1])             # <<<<<<<<<<<<<<
  *         strncpyU(errorInfo.abapMsgType, sapuc, len(exception.msg_type[0:1]) + 1)
  *         free(sapuc)
  */
-  __pyx_slice__43 = PySlice_New(__pyx_int_0, __pyx_int_1, Py_None); if (unlikely(!__pyx_slice__43)) __PYX_ERR(0, 2593, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_slice__43);
-  __Pyx_GIVEREF(__pyx_slice__43);
+  __pyx_slice__44 = PySlice_New(__pyx_int_0, __pyx_int_1, Py_None); if (unlikely(!__pyx_slice__44)) __PYX_ERR(0, 2593, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_slice__44);
+  __Pyx_GIVEREF(__pyx_slice__44);
 
   /* "pyrfc/_cyrfc.pyx":2601
  *         free(sapuc)
  *     if exception.msg_v1:
  *         sapuc = fillString(exception.msg_v1[0:50])             # <<<<<<<<<<<<<<
  *         strncpyU(errorInfo.abapMsgV1, sapuc, len(exception.msg_v1[0:50]) + 1)
  *         free(sapuc)
  */
-  __pyx_slice__44 = PySlice_New(__pyx_int_0, __pyx_int_50, Py_None); if (unlikely(!__pyx_slice__44)) __PYX_ERR(0, 2601, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_slice__44);
-  __Pyx_GIVEREF(__pyx_slice__44);
+  __pyx_slice__45 = PySlice_New(__pyx_int_0, __pyx_int_50, Py_None); if (unlikely(!__pyx_slice__45)) __PYX_ERR(0, 2601, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_slice__45);
+  __Pyx_GIVEREF(__pyx_slice__45);
 
   /* "pyrfc/_cyrfc.pyx":3021
  *             utcValue = wrapString(stringValue, resultLen)
  *             # replace the "," separator with "."
  *             return utcValue[:19]+'.'+utcValue[20:]             # <<<<<<<<<<<<<<
  *         finally:
  *             free(stringValue)
  */
-  __pyx_slice__46 = PySlice_New(Py_None, __pyx_int_19, Py_None); if (unlikely(!__pyx_slice__46)) __PYX_ERR(0, 3021, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_slice__46);
-  __Pyx_GIVEREF(__pyx_slice__46);
-  __pyx_slice__47 = PySlice_New(__pyx_int_20, Py_None, Py_None); if (unlikely(!__pyx_slice__47)) __PYX_ERR(0, 3021, __pyx_L1_error)
+  __pyx_slice__47 = PySlice_New(Py_None, __pyx_int_19, Py_None); if (unlikely(!__pyx_slice__47)) __PYX_ERR(0, 3021, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_slice__47);
   __Pyx_GIVEREF(__pyx_slice__47);
+  __pyx_slice__48 = PySlice_New(__pyx_int_20, Py_None, Py_None); if (unlikely(!__pyx_slice__48)) __PYX_ERR(0, 3021, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_slice__48);
+  __Pyx_GIVEREF(__pyx_slice__48);
 
   /* "cfunc.to_py":65
  * @cname("__Pyx_CFunc_object____object___to_py")
  * cdef object __Pyx_CFunc_object____object___to_py(object (*f)(object) ):
  *     def wrap(object client_connection):             # <<<<<<<<<<<<<<
  *         """wrap(client_connection)"""
  *         return f(client_connection)
  */
-  __pyx_tuple__48 = PyTuple_Pack(1, __pyx_n_s_client_connection); if (unlikely(!__pyx_tuple__48)) __PYX_ERR(1, 65, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__48);
-  __Pyx_GIVEREF(__pyx_tuple__48);
-  __pyx_codeobj__49 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__48, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_wrap, 65, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__49)) __PYX_ERR(1, 65, __pyx_L1_error)
+  __pyx_tuple__49 = PyTuple_Pack(1, __pyx_n_s_client_connection); if (unlikely(!__pyx_tuple__49)) __PYX_ERR(1, 65, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__49);
+  __Pyx_GIVEREF(__pyx_tuple__49);
+  __pyx_codeobj__50 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__49, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_wrap, 65, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__50)) __PYX_ERR(1, 65, __pyx_L1_error)
 
   /* "pyrfc/_cyrfc.pyx":112
  * 
  * 
  * def get_nwrfclib_version():             # <<<<<<<<<<<<<<
  *     """Get SAP NW RFC Lib version
  *     :returns: tuple of major, minor and patch level and OS platform
  */
-  __pyx_tuple__51 = PyTuple_Pack(3, __pyx_n_s_major, __pyx_n_s_minor, __pyx_n_s_patchlevel); if (unlikely(!__pyx_tuple__51)) __PYX_ERR(0, 112, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__51);
-  __Pyx_GIVEREF(__pyx_tuple__51);
-  __pyx_codeobj__52 = (PyObject*)__Pyx_PyCode_New(0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__51, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_pyrfc__cyrfc_pyx, __pyx_n_s_get_nwrfclib_version, 112, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__52)) __PYX_ERR(0, 112, __pyx_L1_error)
+  __pyx_tuple__52 = PyTuple_Pack(3, __pyx_n_s_major, __pyx_n_s_minor, __pyx_n_s_patchlevel); if (unlikely(!__pyx_tuple__52)) __PYX_ERR(0, 112, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__52);
+  __Pyx_GIVEREF(__pyx_tuple__52);
+  __pyx_codeobj__53 = (PyObject*)__Pyx_PyCode_New(0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__52, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_pyrfc__cyrfc_pyx, __pyx_n_s_get_nwrfclib_version, 112, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__53)) __PYX_ERR(0, 112, __pyx_L1_error)
 
   /* "pyrfc/_cyrfc.pyx":123
  * 
  * 
  * def set_ini_file_directory(path_name):             # <<<<<<<<<<<<<<
  *     """Sets the directory in which to search for the sapnwrfc.ini file
  * 
  */
-  __pyx_tuple__53 = PyTuple_Pack(4, __pyx_n_s_path_name, __pyx_n_s_errorInfo, __pyx_n_s_pathName, __pyx_n_s_rc); if (unlikely(!__pyx_tuple__53)) __PYX_ERR(0, 123, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__53);
-  __Pyx_GIVEREF(__pyx_tuple__53);
-  __pyx_codeobj__54 = (PyObject*)__Pyx_PyCode_New(1, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__53, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_pyrfc__cyrfc_pyx, __pyx_n_s_set_ini_file_directory, 123, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__54)) __PYX_ERR(0, 123, __pyx_L1_error)
+  __pyx_tuple__54 = PyTuple_Pack(4, __pyx_n_s_path_name, __pyx_n_s_errorInfo, __pyx_n_s_pathName, __pyx_n_s_rc); if (unlikely(!__pyx_tuple__54)) __PYX_ERR(0, 123, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__54);
+  __Pyx_GIVEREF(__pyx_tuple__54);
+  __pyx_codeobj__55 = (PyObject*)__Pyx_PyCode_New(1, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__54, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_pyrfc__cyrfc_pyx, __pyx_n_s_set_ini_file_directory, 123, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__55)) __PYX_ERR(0, 123, __pyx_L1_error)
 
   /* "pyrfc/_cyrfc.pyx":143
  * 
  * 
  * def reload_ini_file():             # <<<<<<<<<<<<<<
  *     """Reloads the contents of the sapnwrfc.ini file into memory.
  * 
  */
-  __pyx_tuple__55 = PyTuple_Pack(2, __pyx_n_s_errorInfo, __pyx_n_s_rc); if (unlikely(!__pyx_tuple__55)) __PYX_ERR(0, 143, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__55);
-  __Pyx_GIVEREF(__pyx_tuple__55);
-  __pyx_codeobj__56 = (PyObject*)__Pyx_PyCode_New(0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__55, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_pyrfc__cyrfc_pyx, __pyx_n_s_reload_ini_file, 143, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__56)) __PYX_ERR(0, 143, __pyx_L1_error)
+  __pyx_tuple__56 = PyTuple_Pack(2, __pyx_n_s_errorInfo, __pyx_n_s_rc); if (unlikely(!__pyx_tuple__56)) __PYX_ERR(0, 143, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__56);
+  __Pyx_GIVEREF(__pyx_tuple__56);
+  __pyx_codeobj__57 = (PyObject*)__Pyx_PyCode_New(0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__56, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_pyrfc__cyrfc_pyx, __pyx_n_s_reload_ini_file, 143, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__57)) __PYX_ERR(0, 143, __pyx_L1_error)
 
   /* "pyrfc/_cyrfc.pyx":162
  * 
  * 
  * def language_iso_to_sap(lang_iso):             # <<<<<<<<<<<<<<
  *     """Language code conversion of ISO code to SAP code.
  * 
  */
-  __pyx_tuple__57 = PyTuple_Pack(5, __pyx_n_s_lang_iso, __pyx_n_s_uclang_iso, __pyx_n_s_uclang_sap, __pyx_n_s_errorInfo, __pyx_n_s_rc); if (unlikely(!__pyx_tuple__57)) __PYX_ERR(0, 162, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__57);
-  __Pyx_GIVEREF(__pyx_tuple__57);
-  __pyx_codeobj__58 = (PyObject*)__Pyx_PyCode_New(1, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__57, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_pyrfc__cyrfc_pyx, __pyx_n_s_language_iso_to_sap, 162, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__58)) __PYX_ERR(0, 162, __pyx_L1_error)
+  __pyx_tuple__58 = PyTuple_Pack(5, __pyx_n_s_lang_iso, __pyx_n_s_uclang_iso, __pyx_n_s_uclang_sap, __pyx_n_s_errorInfo, __pyx_n_s_rc); if (unlikely(!__pyx_tuple__58)) __PYX_ERR(0, 162, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__58);
+  __Pyx_GIVEREF(__pyx_tuple__58);
+  __pyx_codeobj__59 = (PyObject*)__Pyx_PyCode_New(1, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__58, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_pyrfc__cyrfc_pyx, __pyx_n_s_language_iso_to_sap, 162, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__59)) __PYX_ERR(0, 162, __pyx_L1_error)
 
   /* "pyrfc/_cyrfc.pyx":183
  * 
  * 
  * def language_sap_to_iso(lang_sap):             # <<<<<<<<<<<<<<
  *     """Language code conversion of SAP code to ISO code.
  * 
  */
-  __pyx_tuple__59 = PyTuple_Pack(5, __pyx_n_s_lang_sap, __pyx_n_s_uclang_sap, __pyx_n_s_uclang_iso, __pyx_n_s_errorInfo, __pyx_n_s_rc); if (unlikely(!__pyx_tuple__59)) __PYX_ERR(0, 183, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__59);
-  __Pyx_GIVEREF(__pyx_tuple__59);
-  __pyx_codeobj__60 = (PyObject*)__Pyx_PyCode_New(1, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__59, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_pyrfc__cyrfc_pyx, __pyx_n_s_language_sap_to_iso, 183, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__60)) __PYX_ERR(0, 183, __pyx_L1_error)
+  __pyx_tuple__60 = PyTuple_Pack(5, __pyx_n_s_lang_sap, __pyx_n_s_uclang_sap, __pyx_n_s_uclang_iso, __pyx_n_s_errorInfo, __pyx_n_s_rc); if (unlikely(!__pyx_tuple__60)) __PYX_ERR(0, 183, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__60);
+  __Pyx_GIVEREF(__pyx_tuple__60);
+  __pyx_codeobj__61 = (PyObject*)__Pyx_PyCode_New(1, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__60, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_pyrfc__cyrfc_pyx, __pyx_n_s_language_sap_to_iso, 183, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__61)) __PYX_ERR(0, 183, __pyx_L1_error)
 
   /* "pyrfc/_cyrfc.pyx":204
  * 
  * 
  * def set_cryptolib_path(path_name):             # <<<<<<<<<<<<<<
  *     """Sets the absolute path to the sapcrypto library to enable TLS encryption via Websocket Rfc.
  * 
  */
-  __pyx_tuple__61 = PyTuple_Pack(4, __pyx_n_s_path_name, __pyx_n_s_errorInfo, __pyx_n_s_pathName, __pyx_n_s_rc); if (unlikely(!__pyx_tuple__61)) __PYX_ERR(0, 204, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__61);
-  __Pyx_GIVEREF(__pyx_tuple__61);
-  __pyx_codeobj__62 = (PyObject*)__Pyx_PyCode_New(1, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__61, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_pyrfc__cyrfc_pyx, __pyx_n_s_set_cryptolib_path, 204, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__62)) __PYX_ERR(0, 204, __pyx_L1_error)
+  __pyx_tuple__62 = PyTuple_Pack(4, __pyx_n_s_path_name, __pyx_n_s_errorInfo, __pyx_n_s_pathName, __pyx_n_s_rc); if (unlikely(!__pyx_tuple__62)) __PYX_ERR(0, 204, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__62);
+  __Pyx_GIVEREF(__pyx_tuple__62);
+  __pyx_codeobj__63 = (PyObject*)__Pyx_PyCode_New(1, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__62, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_pyrfc__cyrfc_pyx, __pyx_n_s_set_cryptolib_path, 204, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__63)) __PYX_ERR(0, 204, __pyx_L1_error)
 
   /* "pyrfc/_cyrfc.pyx":228
  * 
  * 
  * def set_locale_radix(value=None):             # <<<<<<<<<<<<<<
  *     """Sets the locale radix for decimal conversions.
  * 
  */
-  __pyx_tuple__63 = PyTuple_Pack(1, __pyx_n_s_value); if (unlikely(!__pyx_tuple__63)) __PYX_ERR(0, 228, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__63);
-  __Pyx_GIVEREF(__pyx_tuple__63);
-  __pyx_codeobj__64 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__63, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_pyrfc__cyrfc_pyx, __pyx_n_s_set_locale_radix, 228, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__64)) __PYX_ERR(0, 228, __pyx_L1_error)
+  __pyx_tuple__64 = PyTuple_Pack(1, __pyx_n_s_value); if (unlikely(!__pyx_tuple__64)) __PYX_ERR(0, 228, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__64);
+  __Pyx_GIVEREF(__pyx_tuple__64);
+  __pyx_codeobj__65 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__64, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_pyrfc__cyrfc_pyx, __pyx_n_s_set_locale_radix, 228, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__65)) __PYX_ERR(0, 228, __pyx_L1_error)
 
   /* "pyrfc/_cyrfc.pyx":252
  * 
  * 
  * def cancel_connection(client_connection):             # <<<<<<<<<<<<<<
  *     """Immediately cancels the RFC call which is currently being called over the given RFC connection
  *     and closes the connection. Can be used only on an RFC client connection.
  */
-  __pyx_tuple__65 = PyTuple_Pack(1, __pyx_n_s_client_connection); if (unlikely(!__pyx_tuple__65)) __PYX_ERR(0, 252, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__65);
-  __Pyx_GIVEREF(__pyx_tuple__65);
-  __pyx_codeobj__66 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__65, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_pyrfc__cyrfc_pyx, __pyx_n_s_cancel_connection, 252, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__66)) __PYX_ERR(0, 252, __pyx_L1_error)
+  __pyx_tuple__66 = PyTuple_Pack(1, __pyx_n_s_client_connection); if (unlikely(!__pyx_tuple__66)) __PYX_ERR(0, 252, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__66);
+  __Pyx_GIVEREF(__pyx_tuple__66);
+  __pyx_codeobj__67 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__66, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_pyrfc__cyrfc_pyx, __pyx_n_s_cancel_connection, 252, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__67)) __PYX_ERR(0, 252, __pyx_L1_error)
 
   /* "pyrfc/_cyrfc.pyx":312
  * 
  * 
  * class TypeDescription(object):             # <<<<<<<<<<<<<<
  *     """ A type description
  * 
  */
-  __pyx_tuple__67 = PyTuple_Pack(1, __pyx_builtin_object); if (unlikely(!__pyx_tuple__67)) __PYX_ERR(0, 312, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__67);
-  __Pyx_GIVEREF(__pyx_tuple__67);
+  __pyx_tuple__68 = PyTuple_Pack(1, __pyx_builtin_object); if (unlikely(!__pyx_tuple__68)) __PYX_ERR(0, 312, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__68);
+  __Pyx_GIVEREF(__pyx_tuple__68);
 
   /* "pyrfc/_cyrfc.pyx":337
  * 
  *     """
  *     def __init__(self, name, nuc_length, uc_length):             # <<<<<<<<<<<<<<
  *         self.fields = []
  *         if len(name)<1 or len(name)>30:
  */
-  __pyx_tuple__68 = PyTuple_Pack(5, __pyx_n_s_self, __pyx_n_s_name, __pyx_n_s_nuc_length, __pyx_n_s_uc_length, __pyx_n_s_int_field); if (unlikely(!__pyx_tuple__68)) __PYX_ERR(0, 337, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__68);
-  __Pyx_GIVEREF(__pyx_tuple__68);
-  __pyx_codeobj__69 = (PyObject*)__Pyx_PyCode_New(4, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__68, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_pyrfc__cyrfc_pyx, __pyx_n_s_init, 337, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__69)) __PYX_ERR(0, 337, __pyx_L1_error)
+  __pyx_tuple__69 = PyTuple_Pack(5, __pyx_n_s_self, __pyx_n_s_name, __pyx_n_s_nuc_length, __pyx_n_s_uc_length, __pyx_n_s_int_field); if (unlikely(!__pyx_tuple__69)) __PYX_ERR(0, 337, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__69);
+  __Pyx_GIVEREF(__pyx_tuple__69);
+  __pyx_codeobj__70 = (PyObject*)__Pyx_PyCode_New(4, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__69, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_pyrfc__cyrfc_pyx, __pyx_n_s_init, 337, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__70)) __PYX_ERR(0, 337, __pyx_L1_error)
 
   /* "pyrfc/_cyrfc.pyx":348
  *         self.uc_length = uc_length
  * 
  *     def add_field(self, name, field_type, nuc_length, uc_length, nuc_offset,             # <<<<<<<<<<<<<<
  *                   uc_offset, decimals=0, type_description=None):
  *         """ Adds a field to the type description.
  */
-  __pyx_tuple__70 = PyTuple_Pack(10, __pyx_n_s_self, __pyx_n_s_name, __pyx_n_s_field_type, __pyx_n_s_nuc_length, __pyx_n_s_uc_length, __pyx_n_s_nuc_offset, __pyx_n_s_uc_offset, __pyx_n_s_decimals, __pyx_n_s_type_description, __pyx_n_s_int_field); if (unlikely(!__pyx_tuple__70)) __PYX_ERR(0, 348, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__70);
-  __Pyx_GIVEREF(__pyx_tuple__70);
-  __pyx_codeobj__71 = (PyObject*)__Pyx_PyCode_New(9, 0, 10, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__70, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_pyrfc__cyrfc_pyx, __pyx_n_s_add_field, 348, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__71)) __PYX_ERR(0, 348, __pyx_L1_error)
-  __pyx_tuple__72 = PyTuple_Pack(2, ((PyObject *)__pyx_int_0), ((PyObject *)Py_None)); if (unlikely(!__pyx_tuple__72)) __PYX_ERR(0, 348, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__72);
-  __Pyx_GIVEREF(__pyx_tuple__72);
+  __pyx_tuple__71 = PyTuple_Pack(10, __pyx_n_s_self, __pyx_n_s_name, __pyx_n_s_field_type, __pyx_n_s_nuc_length, __pyx_n_s_uc_length, __pyx_n_s_nuc_offset, __pyx_n_s_uc_offset, __pyx_n_s_decimals, __pyx_n_s_type_description, __pyx_n_s_int_field); if (unlikely(!__pyx_tuple__71)) __PYX_ERR(0, 348, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__71);
+  __Pyx_GIVEREF(__pyx_tuple__71);
+  __pyx_codeobj__72 = (PyObject*)__Pyx_PyCode_New(9, 0, 10, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__71, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_pyrfc__cyrfc_pyx, __pyx_n_s_add_field, 348, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__72)) __PYX_ERR(0, 348, __pyx_L1_error)
+  __pyx_tuple__73 = PyTuple_Pack(2, ((PyObject *)__pyx_int_0), ((PyObject *)Py_None)); if (unlikely(!__pyx_tuple__73)) __PYX_ERR(0, 348, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__73);
+  __Pyx_GIVEREF(__pyx_tuple__73);
 
   /* "pyrfc/_cyrfc.pyx":389
  *         })
  * 
  *     def __repr__(self):             # <<<<<<<<<<<<<<
  *         return f"<TypeDescription '{self.name}' with {len(self.fields)} " \
  *             f"fields (n/uclength={self.nuc_length}/{self.uc_length})>"
  */
-  __pyx_tuple__73 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__73)) __PYX_ERR(0, 389, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__73);
-  __Pyx_GIVEREF(__pyx_tuple__73);
-  __pyx_codeobj__74 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__73, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_pyrfc__cyrfc_pyx, __pyx_n_s_repr, 389, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__74)) __PYX_ERR(0, 389, __pyx_L1_error)
+  __pyx_tuple__74 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__74)) __PYX_ERR(0, 389, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__74);
+  __Pyx_GIVEREF(__pyx_tuple__74);
+  __pyx_codeobj__75 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__74, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_pyrfc__cyrfc_pyx, __pyx_n_s_repr, 389, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__75)) __PYX_ERR(0, 389, __pyx_L1_error)
 
   /* "pyrfc/_cyrfc.pyx":398
  * 
  * 
  * class FunctionDescription(object):             # <<<<<<<<<<<<<<
  *     """ A function description
  * 
  */
-  __pyx_tuple__75 = PyTuple_Pack(1, __pyx_builtin_object); if (unlikely(!__pyx_tuple__75)) __PYX_ERR(0, 398, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__75);
-  __Pyx_GIVEREF(__pyx_tuple__75);
+  __pyx_tuple__76 = PyTuple_Pack(1, __pyx_builtin_object); if (unlikely(!__pyx_tuple__76)) __PYX_ERR(0, 398, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__76);
+  __Pyx_GIVEREF(__pyx_tuple__76);
 
   /* "pyrfc/_cyrfc.pyx":421
  * 
  *     """
  *     def __init__(self, name):             # <<<<<<<<<<<<<<
  *         self.name = name
  *         self.parameters = []
  */
-  __pyx_tuple__76 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_name); if (unlikely(!__pyx_tuple__76)) __PYX_ERR(0, 421, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__76);
-  __Pyx_GIVEREF(__pyx_tuple__76);
-  __pyx_codeobj__77 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__76, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_pyrfc__cyrfc_pyx, __pyx_n_s_init, 421, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__77)) __PYX_ERR(0, 421, __pyx_L1_error)
+  __pyx_tuple__77 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_name); if (unlikely(!__pyx_tuple__77)) __PYX_ERR(0, 421, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__77);
+  __Pyx_GIVEREF(__pyx_tuple__77);
+  __pyx_codeobj__78 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__77, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_pyrfc__cyrfc_pyx, __pyx_n_s_init, 421, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__78)) __PYX_ERR(0, 421, __pyx_L1_error)
 
   /* "pyrfc/_cyrfc.pyx":425
  *         self.parameters = []
  * 
  *     def add_parameter(self, name, parameter_type, direction, nuc_length,             # <<<<<<<<<<<<<<
  *                       uc_length, decimals=0, default_value="", parameter_text="",
  *                       optional=False, type_description=None):
  */
-  __pyx_tuple__78 = PyTuple_Pack(11, __pyx_n_s_self, __pyx_n_s_name, __pyx_n_s_parameter_type, __pyx_n_s_direction, __pyx_n_s_nuc_length, __pyx_n_s_uc_length, __pyx_n_s_decimals, __pyx_n_s_default_value, __pyx_n_s_parameter_text, __pyx_n_s_optional, __pyx_n_s_type_description); if (unlikely(!__pyx_tuple__78)) __PYX_ERR(0, 425, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__78);
-  __Pyx_GIVEREF(__pyx_tuple__78);
-  __pyx_codeobj__79 = (PyObject*)__Pyx_PyCode_New(11, 0, 11, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__78, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_pyrfc__cyrfc_pyx, __pyx_n_s_add_parameter, 425, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__79)) __PYX_ERR(0, 425, __pyx_L1_error)
-  __pyx_tuple__80 = PyTuple_Pack(5, ((PyObject *)__pyx_int_0), ((PyObject*)__pyx_kp_s__5), ((PyObject*)__pyx_kp_s__5), ((PyObject *)Py_False), ((PyObject *)Py_None)); if (unlikely(!__pyx_tuple__80)) __PYX_ERR(0, 425, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__80);
-  __Pyx_GIVEREF(__pyx_tuple__80);
+  __pyx_tuple__79 = PyTuple_Pack(11, __pyx_n_s_self, __pyx_n_s_name, __pyx_n_s_parameter_type, __pyx_n_s_direction, __pyx_n_s_nuc_length, __pyx_n_s_uc_length, __pyx_n_s_decimals, __pyx_n_s_default_value, __pyx_n_s_parameter_text, __pyx_n_s_optional, __pyx_n_s_type_description); if (unlikely(!__pyx_tuple__79)) __PYX_ERR(0, 425, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__79);
+  __Pyx_GIVEREF(__pyx_tuple__79);
+  __pyx_codeobj__80 = (PyObject*)__Pyx_PyCode_New(11, 0, 11, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__79, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_pyrfc__cyrfc_pyx, __pyx_n_s_add_parameter, 425, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__80)) __PYX_ERR(0, 425, __pyx_L1_error)
+  __pyx_tuple__81 = PyTuple_Pack(5, ((PyObject *)__pyx_int_0), ((PyObject*)__pyx_kp_u__5), ((PyObject*)__pyx_kp_u__5), ((PyObject *)Py_False), ((PyObject *)Py_None)); if (unlikely(!__pyx_tuple__81)) __PYX_ERR(0, 425, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__81);
+  __Pyx_GIVEREF(__pyx_tuple__81);
 
   /* "pyrfc/_cyrfc.pyx":474
  *         })
  * 
  *     def __repr__(self):             # <<<<<<<<<<<<<<
  *         return f"<FunctionDescription '{self.name}' with {len(self.parameters)} params>"
  * 
  */
-  __pyx_tuple__81 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__81)) __PYX_ERR(0, 474, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__81);
-  __Pyx_GIVEREF(__pyx_tuple__81);
-  __pyx_codeobj__82 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__81, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_pyrfc__cyrfc_pyx, __pyx_n_s_repr, 474, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__82)) __PYX_ERR(0, 474, __pyx_L1_error)
+  __pyx_tuple__82 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__82)) __PYX_ERR(0, 474, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__82);
+  __Pyx_GIVEREF(__pyx_tuple__82);
+  __pyx_codeobj__83 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__82, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_pyrfc__cyrfc_pyx, __pyx_n_s_repr, 474, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__83)) __PYX_ERR(0, 474, __pyx_L1_error)
 
   /* "pyrfc/_cyrfc.pyx":1501
  * 
  * 
  * def default_auth_check(func_name=False, request_context = None):             # <<<<<<<<<<<<<<
  *     request_context = request_context or {}
  *     _server_log(f"authorization check for '{func_name}'", request_context['server_context'])
  */
-  __pyx_tuple__83 = PyTuple_Pack(2, __pyx_n_s_func_name, __pyx_n_s_request_context); if (unlikely(!__pyx_tuple__83)) __PYX_ERR(0, 1501, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__83);
-  __Pyx_GIVEREF(__pyx_tuple__83);
-  __pyx_codeobj__84 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__83, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_pyrfc__cyrfc_pyx, __pyx_n_s_default_auth_check, 1501, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__84)) __PYX_ERR(0, 1501, __pyx_L1_error)
+  __pyx_tuple__84 = PyTuple_Pack(2, __pyx_n_s_func_name, __pyx_n_s_request_context); if (unlikely(!__pyx_tuple__84)) __PYX_ERR(0, 1501, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__84);
+  __Pyx_GIVEREF(__pyx_tuple__84);
+  __pyx_codeobj__85 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__84, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_pyrfc__cyrfc_pyx, __pyx_n_s_default_auth_check, 1501, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__85)) __PYX_ERR(0, 1501, __pyx_L1_error)
 
   /* "pyrfc/_cyrfc.pyx":1507
  * 
  * 
  * def _server_log(origin, log_message):             # <<<<<<<<<<<<<<
  *     if server_context["server_log"]:
  *         print (f"[{datetime.utcnow()} UTC] {origin} '{log_message}'")
  */
-  __pyx_tuple__85 = PyTuple_Pack(2, __pyx_n_s_origin, __pyx_n_s_log_message); if (unlikely(!__pyx_tuple__85)) __PYX_ERR(0, 1507, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__85);
-  __Pyx_GIVEREF(__pyx_tuple__85);
-  __pyx_codeobj__86 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__85, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_pyrfc__cyrfc_pyx, __pyx_n_s_server_log, 1507, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__86)) __PYX_ERR(0, 1507, __pyx_L1_error)
+  __pyx_tuple__86 = PyTuple_Pack(2, __pyx_n_s_origin, __pyx_n_s_log_message); if (unlikely(!__pyx_tuple__86)) __PYX_ERR(0, 1507, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__86);
+  __Pyx_GIVEREF(__pyx_tuple__86);
+  __pyx_codeobj__87 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__86, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_pyrfc__cyrfc_pyx, __pyx_n_s_server_log, 1507, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__87)) __PYX_ERR(0, 1507, __pyx_L1_error)
 
   /* "pyrfc/_cyrfc.pyx":2232
  * 
  *     @staticmethod
  *     def getFromConnection(Connection connection):             # <<<<<<<<<<<<<<
  *         """Returns the currently attached throughput object from a connection, if any.
  * 
  */
-  __pyx_tuple__87 = PyTuple_Pack(4, __pyx_n_s_connection, __pyx_n_s_errorInfo, __pyx_n_s_throughput, __pyx_n_s_t); if (unlikely(!__pyx_tuple__87)) __PYX_ERR(0, 2232, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__87);
-  __Pyx_GIVEREF(__pyx_tuple__87);
-  __pyx_codeobj__88 = (PyObject*)__Pyx_PyCode_New(1, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__87, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_pyrfc__cyrfc_pyx, __pyx_n_s_getFromConnection, 2232, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__88)) __PYX_ERR(0, 2232, __pyx_L1_error)
+  __pyx_tuple__88 = PyTuple_Pack(4, __pyx_n_s_connection, __pyx_n_s_errorInfo, __pyx_n_s_throughput, __pyx_n_s_t); if (unlikely(!__pyx_tuple__88)) __PYX_ERR(0, 2232, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__88);
+  __Pyx_GIVEREF(__pyx_tuple__88);
+  __pyx_codeobj__89 = (PyObject*)__Pyx_PyCode_New(1, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__88, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_pyrfc__cyrfc_pyx, __pyx_n_s_getFromConnection, 2232, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__89)) __PYX_ERR(0, 2232, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
@@ -43173,15 +43964,15 @@
  * from decimal import Decimal
  */
   __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_n_s_Iterable);
   __Pyx_GIVEREF(__pyx_n_s_Iterable);
   PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_Iterable);
-  __pyx_t_2 = __Pyx_Import(__pyx_n_s_collections_abc, __pyx_t_1, -1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 9, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_Import(__pyx_n_s_collections_abc, __pyx_t_1, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_Iterable); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_Iterable, __pyx_t_1) < 0) __PYX_ERR(0, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
@@ -43200,15 +43991,15 @@
   PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_date);
   __Pyx_INCREF(__pyx_n_s_time);
   __Pyx_GIVEREF(__pyx_n_s_time);
   PyList_SET_ITEM(__pyx_t_2, 1, __pyx_n_s_time);
   __Pyx_INCREF(__pyx_n_s_datetime);
   __Pyx_GIVEREF(__pyx_n_s_datetime);
   PyList_SET_ITEM(__pyx_t_2, 2, __pyx_n_s_datetime);
-  __pyx_t_1 = __Pyx_Import(__pyx_n_s_datetime, __pyx_t_2, -1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 10, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_Import(__pyx_n_s_datetime, __pyx_t_2, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 10, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_1, __pyx_n_s_date); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 10, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_date, __pyx_t_2) < 0) __PYX_ERR(0, 10, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_1, __pyx_n_s_time); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 10, __pyx_L1_error)
@@ -43229,15 +44020,15 @@
  * from locale import localeconv
  */
   __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 11, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_n_s_Decimal);
   __Pyx_GIVEREF(__pyx_n_s_Decimal);
   PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_Decimal);
-  __pyx_t_2 = __Pyx_Import(__pyx_n_s_decimal, __pyx_t_1, -1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 11, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_Import(__pyx_n_s_decimal, __pyx_t_1, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 11, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_Decimal); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 11, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_Decimal, __pyx_t_1) < 0) __PYX_ERR(0, 11, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
@@ -43253,15 +44044,15 @@
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_n_s_Enum);
   __Pyx_GIVEREF(__pyx_n_s_Enum);
   PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_Enum);
   __Pyx_INCREF(__pyx_n_s_auto);
   __Pyx_GIVEREF(__pyx_n_s_auto);
   PyList_SET_ITEM(__pyx_t_2, 1, __pyx_n_s_auto);
-  __pyx_t_1 = __Pyx_Import(__pyx_n_s_enum, __pyx_t_2, -1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 12, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_Import(__pyx_n_s_enum, __pyx_t_2, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 12, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_1, __pyx_n_s_Enum); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 12, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_Enum, __pyx_t_2) < 0) __PYX_ERR(0, 12, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_1, __pyx_n_s_auto); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 12, __pyx_L1_error)
@@ -43278,15 +44069,15 @@
  * from sys import exc_info, platform
  */
   __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 13, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_n_s_localeconv);
   __Pyx_GIVEREF(__pyx_n_s_localeconv);
   PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_localeconv);
-  __pyx_t_2 = __Pyx_Import(__pyx_n_s_locale, __pyx_t_1, -1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 13, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_Import(__pyx_n_s_locale, __pyx_t_1, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 13, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_localeconv); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 13, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_localeconv, __pyx_t_1) < 0) __PYX_ERR(0, 13, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
@@ -43302,15 +44093,15 @@
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_n_s_isfile);
   __Pyx_GIVEREF(__pyx_n_s_isfile);
   PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_isfile);
   __Pyx_INCREF(__pyx_n_s_join);
   __Pyx_GIVEREF(__pyx_n_s_join);
   PyList_SET_ITEM(__pyx_t_2, 1, __pyx_n_s_join);
-  __pyx_t_1 = __Pyx_Import(__pyx_n_s_os_path, __pyx_t_2, -1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 14, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_Import(__pyx_n_s_os_path, __pyx_t_2, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 14, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_1, __pyx_n_s_isfile); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 14, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_isfile, __pyx_t_2) < 0) __PYX_ERR(0, 14, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_1, __pyx_n_s_join); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 14, __pyx_L1_error)
@@ -43330,15 +44121,15 @@
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_n_s_exc_info);
   __Pyx_GIVEREF(__pyx_n_s_exc_info);
   PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_exc_info);
   __Pyx_INCREF(__pyx_n_s_platform);
   __Pyx_GIVEREF(__pyx_n_s_platform);
   PyList_SET_ITEM(__pyx_t_1, 1, __pyx_n_s_platform);
-  __pyx_t_2 = __Pyx_Import(__pyx_n_s_sys, __pyx_t_1, -1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 15, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_Import(__pyx_n_s_sys, __pyx_t_1, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_exc_info); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_exc_info, __pyx_t_1) < 0) __PYX_ERR(0, 15, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_platform); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 15, __pyx_L1_error)
@@ -43350,15 +44141,15 @@
   /* "pyrfc/_cyrfc.pyx":16
  * from os.path import isfile, join
  * from sys import exc_info, platform
  * import socket             # <<<<<<<<<<<<<<
  * from threading import Thread, Timer
  * 
  */
-  __pyx_t_2 = __Pyx_Import(__pyx_n_s_socket, 0, -1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 16, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_Import(__pyx_n_s_socket, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_socket, __pyx_t_2) < 0) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "pyrfc/_cyrfc.pyx":17
  * from sys import exc_info, platform
  * import socket
@@ -43370,15 +44161,15 @@
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_n_s_Thread);
   __Pyx_GIVEREF(__pyx_n_s_Thread);
   PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_Thread);
   __Pyx_INCREF(__pyx_n_s_Timer);
   __Pyx_GIVEREF(__pyx_n_s_Timer);
   PyList_SET_ITEM(__pyx_t_2, 1, __pyx_n_s_Timer);
-  __pyx_t_1 = __Pyx_Import(__pyx_n_s_threading, __pyx_t_2, -1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 17, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_Import(__pyx_n_s_threading, __pyx_t_2, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_1, __pyx_n_s_Thread); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_Thread, __pyx_t_2) < 0) __PYX_ERR(0, 17, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_1, __pyx_n_s_Timer); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 17, __pyx_L1_error)
@@ -43392,17 +44183,17 @@
  * from . csapnwrfc cimport *
  * from . _exception import *             # <<<<<<<<<<<<<<
  * from . _utils import enum_names, enum_values
  * 
  */
   __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 20, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_INCREF(__pyx_n_s__50);
-  __Pyx_GIVEREF(__pyx_n_s__50);
-  PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s__50);
+  __Pyx_INCREF(__pyx_n_s__51);
+  __Pyx_GIVEREF(__pyx_n_s__51);
+  PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s__51);
   __pyx_t_2 = __Pyx_Import(__pyx_n_s_exception, __pyx_t_1, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 20, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (__pyx_import_star(__pyx_t_2) < 0) __PYX_ERR(0, 20, __pyx_L1_error);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "pyrfc/_cyrfc.pyx":21
@@ -43468,15 +44259,15 @@
  * ################################################################################
  */
   __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_localeconv); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 33, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_2 = __Pyx_PyObject_CallNoArg(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 33, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_t_2, __pyx_n_s_decimal_point); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 33, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_t_2, __pyx_n_u_decimal_point); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 33, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_LOCALE_RADIX, __pyx_t_1) < 0) __PYX_ERR(0, 33, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "pyrfc/_cyrfc.pyx":41
  * 
@@ -43548,15 +44339,15 @@
   /* "pyrfc/_cyrfc.pyx":41
  * 
  * # RFC parameter direction
  * class RfcParameterDirection(Enum):             # <<<<<<<<<<<<<<
  *     RFC_IMPORT = RFC_DIRECTION.RFC_IMPORT
  *     RFC_EXPORT = RFC_DIRECTION.RFC_EXPORT
  */
-  __pyx_t_4 = __Pyx_Py3ClassCreate(__pyx_t_1, __pyx_n_s_RfcParameterDirection, __pyx_t_2, __pyx_t_3, NULL, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 41, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_Py3ClassCreate(__pyx_t_1, __pyx_n_s_RfcParameterDirection, __pyx_t_2, __pyx_t_3, NULL, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 41, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_RfcParameterDirection, __pyx_t_4) < 0) __PYX_ERR(0, 41, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
@@ -43930,15 +44721,15 @@
   /* "pyrfc/_cyrfc.pyx":49
  * 
  * # RFC field type
  * class RfcFieldType(Enum):             # <<<<<<<<<<<<<<
  *     RFCTYPE_CHAR = RFCTYPE.RFCTYPE_CHAR
  *     RFCTYPE_DATE = RFCTYPE.RFCTYPE_DATE
  */
-  __pyx_t_4 = __Pyx_Py3ClassCreate(__pyx_t_2, __pyx_n_s_RfcFieldType, __pyx_t_1, __pyx_t_3, NULL, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 49, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_Py3ClassCreate(__pyx_t_2, __pyx_n_s_RfcFieldType, __pyx_t_1, __pyx_t_3, NULL, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 49, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_RfcFieldType, __pyx_t_4) < 0) __PYX_ERR(0, 49, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
@@ -44078,15 +44869,15 @@
   /* "pyrfc/_cyrfc.pyx":82
  * 
  * # bgRFC unit state
  * class UnitState(Enum):             # <<<<<<<<<<<<<<
  *     not_found = RFC_UNIT_STATE.RFC_UNIT_NOT_FOUND
  *     in_process = RFC_UNIT_STATE.RFC_UNIT_IN_PROCESS
  */
-  __pyx_t_4 = __Pyx_Py3ClassCreate(__pyx_t_1, __pyx_n_s_UnitState, __pyx_t_2, __pyx_t_3, NULL, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 82, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_Py3ClassCreate(__pyx_t_1, __pyx_n_s_UnitState, __pyx_t_2, __pyx_t_3, NULL, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 82, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_UnitState, __pyx_t_4) < 0) __PYX_ERR(0, 82, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
@@ -44160,15 +44951,15 @@
   /* "pyrfc/_cyrfc.pyx":93
  * 
  * # bgRFC status
  * class RCStatus(Enum):             # <<<<<<<<<<<<<<
  *     OK = RFC_RC.RFC_OK
  *     RFC_NOT_FOUND = RFC_RC.RFC_NOT_FOUND
  */
-  __pyx_t_4 = __Pyx_Py3ClassCreate(__pyx_t_2, __pyx_n_s_RCStatus, __pyx_t_1, __pyx_t_3, NULL, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 93, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_Py3ClassCreate(__pyx_t_2, __pyx_n_s_RCStatus, __pyx_t_1, __pyx_t_3, NULL, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 93, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_RCStatus, __pyx_t_4) < 0) __PYX_ERR(0, 93, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
@@ -44242,15 +45033,15 @@
   /* "pyrfc/_cyrfc.pyx":101
  * 
  * # bgRFCunit call type
  * class UnitCallType(Enum):             # <<<<<<<<<<<<<<
  *     synchronous = RFC_CALL_TYPE.RFC_SYNCHRONOUS
  *     transactional = RFC_CALL_TYPE.RFC_TRANSACTIONAL
  */
-  __pyx_t_4 = __Pyx_Py3ClassCreate(__pyx_t_1, __pyx_n_s_UnitCallType, __pyx_t_2, __pyx_t_3, NULL, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 101, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_Py3ClassCreate(__pyx_t_1, __pyx_n_s_UnitCallType, __pyx_t_2, __pyx_t_3, NULL, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 101, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_UnitCallType, __pyx_t_4) < 0) __PYX_ERR(0, 101, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
@@ -44353,127 +45144,127 @@
   /* "pyrfc/_cyrfc.pyx":312
  * 
  * 
  * class TypeDescription(object):             # <<<<<<<<<<<<<<
  *     """ A type description
  * 
  */
-  __pyx_t_2 = __Pyx_CalculateMetaclass(NULL, __pyx_tuple__67); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 312, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CalculateMetaclass(NULL, __pyx_tuple__68); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 312, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = __Pyx_Py3MetaclassPrepare(__pyx_t_2, __pyx_tuple__67, __pyx_n_s_TypeDescription_2, __pyx_n_s_TypeDescription_2, (PyObject *) NULL, __pyx_n_s_pyrfc__cyrfc, __pyx_kp_s_A_type_description_This_class_w); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 312, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_Py3MetaclassPrepare(__pyx_t_2, __pyx_tuple__68, __pyx_n_s_TypeDescription_2, __pyx_n_s_TypeDescription_2, (PyObject *) NULL, __pyx_n_s_pyrfc__cyrfc, __pyx_kp_s_A_type_description_This_class_w); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 312, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
 
   /* "pyrfc/_cyrfc.pyx":337
  * 
  *     """
  *     def __init__(self, name, nuc_length, uc_length):             # <<<<<<<<<<<<<<
  *         self.fields = []
  *         if len(name)<1 or len(name)>30:
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_5pyrfc_6_cyrfc_15TypeDescription_1__init__, 0, __pyx_n_s_TypeDescription___init, NULL, __pyx_n_s_pyrfc__cyrfc, __pyx_d, ((PyObject *)__pyx_codeobj__69)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 337, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_5pyrfc_6_cyrfc_15TypeDescription_1__init__, 0, __pyx_n_s_TypeDescription___init, NULL, __pyx_n_s_pyrfc__cyrfc, __pyx_d, ((PyObject *)__pyx_codeobj__70)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 337, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_init, __pyx_t_3) < 0) __PYX_ERR(0, 337, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "pyrfc/_cyrfc.pyx":348
  *         self.uc_length = uc_length
  * 
  *     def add_field(self, name, field_type, nuc_length, uc_length, nuc_offset,             # <<<<<<<<<<<<<<
  *                   uc_offset, decimals=0, type_description=None):
  *         """ Adds a field to the type description.
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_5pyrfc_6_cyrfc_15TypeDescription_3add_field, 0, __pyx_n_s_TypeDescription_add_field, NULL, __pyx_n_s_pyrfc__cyrfc, __pyx_d, ((PyObject *)__pyx_codeobj__71)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 348, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_5pyrfc_6_cyrfc_15TypeDescription_3add_field, 0, __pyx_n_s_TypeDescription_add_field, NULL, __pyx_n_s_pyrfc__cyrfc, __pyx_d, ((PyObject *)__pyx_codeobj__72)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 348, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_tuple__72);
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_tuple__73);
   if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_add_field, __pyx_t_3) < 0) __PYX_ERR(0, 348, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "pyrfc/_cyrfc.pyx":389
  *         })
  * 
  *     def __repr__(self):             # <<<<<<<<<<<<<<
  *         return f"<TypeDescription '{self.name}' with {len(self.fields)} " \
  *             f"fields (n/uclength={self.nuc_length}/{self.uc_length})>"
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_5pyrfc_6_cyrfc_15TypeDescription_5__repr__, 0, __pyx_n_s_TypeDescription___repr, NULL, __pyx_n_s_pyrfc__cyrfc, __pyx_d, ((PyObject *)__pyx_codeobj__74)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 389, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_5pyrfc_6_cyrfc_15TypeDescription_5__repr__, 0, __pyx_n_s_TypeDescription___repr, NULL, __pyx_n_s_pyrfc__cyrfc, __pyx_d, ((PyObject *)__pyx_codeobj__75)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 389, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_repr, __pyx_t_3) < 0) __PYX_ERR(0, 389, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "pyrfc/_cyrfc.pyx":312
  * 
  * 
  * class TypeDescription(object):             # <<<<<<<<<<<<<<
  *     """ A type description
  * 
  */
-  __pyx_t_3 = __Pyx_Py3ClassCreate(__pyx_t_2, __pyx_n_s_TypeDescription_2, __pyx_tuple__67, __pyx_t_1, NULL, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 312, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_Py3ClassCreate(__pyx_t_2, __pyx_n_s_TypeDescription_2, __pyx_tuple__68, __pyx_t_1, NULL, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 312, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_TypeDescription_2, __pyx_t_3) < 0) __PYX_ERR(0, 312, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "pyrfc/_cyrfc.pyx":398
  * 
  * 
  * class FunctionDescription(object):             # <<<<<<<<<<<<<<
  *     """ A function description
  * 
  */
-  __pyx_t_2 = __Pyx_CalculateMetaclass(NULL, __pyx_tuple__75); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 398, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CalculateMetaclass(NULL, __pyx_tuple__76); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 398, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = __Pyx_Py3MetaclassPrepare(__pyx_t_2, __pyx_tuple__75, __pyx_n_s_FunctionDescription_2, __pyx_n_s_FunctionDescription_2, (PyObject *) NULL, __pyx_n_s_pyrfc__cyrfc, __pyx_kp_s_A_function_description_This_cla); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 398, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_Py3MetaclassPrepare(__pyx_t_2, __pyx_tuple__76, __pyx_n_s_FunctionDescription_2, __pyx_n_s_FunctionDescription_2, (PyObject *) NULL, __pyx_n_s_pyrfc__cyrfc, __pyx_kp_s_A_function_description_This_cla); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 398, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
 
   /* "pyrfc/_cyrfc.pyx":421
  * 
  *     """
  *     def __init__(self, name):             # <<<<<<<<<<<<<<
  *         self.name = name
  *         self.parameters = []
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_5pyrfc_6_cyrfc_19FunctionDescription_1__init__, 0, __pyx_n_s_FunctionDescription___init, NULL, __pyx_n_s_pyrfc__cyrfc, __pyx_d, ((PyObject *)__pyx_codeobj__77)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 421, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_5pyrfc_6_cyrfc_19FunctionDescription_1__init__, 0, __pyx_n_s_FunctionDescription___init, NULL, __pyx_n_s_pyrfc__cyrfc, __pyx_d, ((PyObject *)__pyx_codeobj__78)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 421, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_init, __pyx_t_3) < 0) __PYX_ERR(0, 421, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "pyrfc/_cyrfc.pyx":425
  *         self.parameters = []
  * 
  *     def add_parameter(self, name, parameter_type, direction, nuc_length,             # <<<<<<<<<<<<<<
  *                       uc_length, decimals=0, default_value="", parameter_text="",
  *                       optional=False, type_description=None):
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_5pyrfc_6_cyrfc_19FunctionDescription_3add_parameter, 0, __pyx_n_s_FunctionDescription_add_paramete, NULL, __pyx_n_s_pyrfc__cyrfc, __pyx_d, ((PyObject *)__pyx_codeobj__79)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 425, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_5pyrfc_6_cyrfc_19FunctionDescription_3add_parameter, 0, __pyx_n_s_FunctionDescription_add_paramete, NULL, __pyx_n_s_pyrfc__cyrfc, __pyx_d, ((PyObject *)__pyx_codeobj__80)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 425, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_tuple__80);
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_tuple__81);
   if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_add_parameter, __pyx_t_3) < 0) __PYX_ERR(0, 425, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "pyrfc/_cyrfc.pyx":474
  *         })
  * 
  *     def __repr__(self):             # <<<<<<<<<<<<<<
  *         return f"<FunctionDescription '{self.name}' with {len(self.parameters)} params>"
  * 
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_5pyrfc_6_cyrfc_19FunctionDescription_5__repr__, 0, __pyx_n_s_FunctionDescription___repr, NULL, __pyx_n_s_pyrfc__cyrfc, __pyx_d, ((PyObject *)__pyx_codeobj__82)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 474, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_5pyrfc_6_cyrfc_19FunctionDescription_5__repr__, 0, __pyx_n_s_FunctionDescription___repr, NULL, __pyx_n_s_pyrfc__cyrfc, __pyx_d, ((PyObject *)__pyx_codeobj__83)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 474, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_repr, __pyx_t_3) < 0) __PYX_ERR(0, 474, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "pyrfc/_cyrfc.pyx":398
  * 
  * 
  * class FunctionDescription(object):             # <<<<<<<<<<<<<<
  *     """ A function description
  * 
  */
-  __pyx_t_3 = __Pyx_Py3ClassCreate(__pyx_t_2, __pyx_n_s_FunctionDescription_2, __pyx_tuple__75, __pyx_t_1, NULL, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 398, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_Py3ClassCreate(__pyx_t_2, __pyx_n_s_FunctionDescription_2, __pyx_tuple__76, __pyx_t_1, NULL, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 398, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_FunctionDescription_2, __pyx_t_3) < 0) __PYX_ERR(0, 398, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "pyrfc/_cyrfc.pyx":1493
@@ -44529,51 +45320,51 @@
  *     __bgRfcFunction = {
  *         "check": None,             # <<<<<<<<<<<<<<
  *         "commit": None,
  *         "rollback": None,
  */
   __pyx_t_2 = __Pyx_PyDict_NewPresized(5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1762, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_check, Py_None) < 0) __PYX_ERR(0, 1762, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_check, Py_None) < 0) __PYX_ERR(0, 1762, __pyx_L1_error)
 
   /* "pyrfc/_cyrfc.pyx":1763
  *     __bgRfcFunction = {
  *         "check": None,
  *         "commit": None,             # <<<<<<<<<<<<<<
  *         "rollback": None,
  *         "confirm": None,
  */
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_commit, Py_None) < 0) __PYX_ERR(0, 1762, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_commit, Py_None) < 0) __PYX_ERR(0, 1762, __pyx_L1_error)
 
   /* "pyrfc/_cyrfc.pyx":1764
  *         "check": None,
  *         "commit": None,
  *         "rollback": None,             # <<<<<<<<<<<<<<
  *         "confirm": None,
  *         "getState": None
  */
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_rollback, Py_None) < 0) __PYX_ERR(0, 1762, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_rollback, Py_None) < 0) __PYX_ERR(0, 1762, __pyx_L1_error)
 
   /* "pyrfc/_cyrfc.pyx":1765
  *         "commit": None,
  *         "rollback": None,
  *         "confirm": None,             # <<<<<<<<<<<<<<
  *         "getState": None
  *     }
  */
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_confirm, Py_None) < 0) __PYX_ERR(0, 1762, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_confirm, Py_None) < 0) __PYX_ERR(0, 1762, __pyx_L1_error)
 
   /* "pyrfc/_cyrfc.pyx":1766
  *         "rollback": None,
  *         "confirm": None,
  *         "getState": None             # <<<<<<<<<<<<<<
  *     }
  * 
  */
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_getState, Py_None) < 0) __PYX_ERR(0, 1762, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_getState, Py_None) < 0) __PYX_ERR(0, 1762, __pyx_L1_error)
   if (PyDict_SetItem((PyObject *)__pyx_ptype_5pyrfc_6_cyrfc_Server->tp_dict, __pyx_n_s_bgRfcFunction, __pyx_t_2) < 0) __PYX_ERR(0, 1761, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_5pyrfc_6_cyrfc_Server);
 
   /* "pyrfc/_cyrfc.pyx":2173
  * 
  * cdef class Throughput:
@@ -47257,21 +48048,14 @@
         Py_XINCREF(value);
         Py_XINCREF(tb);
 #endif
         PyErr_Restore(type, value, tb);
     }
 }
 
-/* StringJoin */
-#if !CYTHON_COMPILING_IN_CPYTHON
-static CYTHON_INLINE PyObject* __Pyx_PyBytes_Join(PyObject* sep, PyObject* values) {
-    return PyObject_CallMethodObjArgs(sep, __pyx_n_s_join, values, NULL);
-}
-#endif
-
 /* PyObjectFormat */
 #if CYTHON_USE_UNICODE_WRITER
 static PyObject* __Pyx_PyObject_Format(PyObject* obj, PyObject* format_spec) {
     int ret;
     _PyUnicodeWriter writer;
     if (likely(PyFloat_CheckExact(obj))) {
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x03040000
@@ -47300,14 +48084,108 @@
         _PyUnicodeWriter_Dealloc(&writer);
         return NULL;
     }
     return _PyUnicodeWriter_Finish(&writer);
 }
 #endif
 
+/* CIntToPyUnicode */
+static CYTHON_INLINE PyObject* __Pyx_PyUnicode_From_RFCTYPE(RFCTYPE value, Py_ssize_t width, char padding_char, char format_char) {
+    char digits[sizeof(RFCTYPE)*3+2];
+    char *dpos, *end = digits + sizeof(RFCTYPE)*3+2;
+    const char *hex_digits = DIGITS_HEX;
+    Py_ssize_t length, ulength;
+    int prepend_sign, last_one_off;
+    RFCTYPE remaining;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
+    const RFCTYPE neg_one = (RFCTYPE) -1, const_zero = (RFCTYPE) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
+#endif
+    const int is_unsigned = neg_one > const_zero;
+    if (format_char == 'X') {
+        hex_digits += 16;
+        format_char = 'x';
+    }
+    remaining = value;
+    last_one_off = 0;
+    dpos = end;
+    do {
+        int digit_pos;
+        switch (format_char) {
+        case 'o':
+            digit_pos = abs((int)(remaining % (8*8)));
+            remaining = (RFCTYPE) (remaining / (8*8));
+            dpos -= 2;
+            memcpy(dpos, DIGIT_PAIRS_8 + digit_pos * 2, 2);
+            last_one_off = (digit_pos < 8);
+            break;
+        case 'd':
+            digit_pos = abs((int)(remaining % (10*10)));
+            remaining = (RFCTYPE) (remaining / (10*10));
+            dpos -= 2;
+            memcpy(dpos, DIGIT_PAIRS_10 + digit_pos * 2, 2);
+            last_one_off = (digit_pos < 10);
+            break;
+        case 'x':
+            *(--dpos) = hex_digits[abs((int)(remaining % 16))];
+            remaining = (RFCTYPE) (remaining / 16);
+            break;
+        default:
+            assert(0);
+            break;
+        }
+    } while (unlikely(remaining != 0));
+    if (last_one_off) {
+        assert(*dpos == '0');
+        dpos++;
+    }
+    length = end - dpos;
+    ulength = length;
+    prepend_sign = 0;
+    if (!is_unsigned && value <= neg_one) {
+        if (padding_char == ' ' || width <= length + 1) {
+            *(--dpos) = '-';
+            ++length;
+        } else {
+            prepend_sign = 1;
+        }
+        ++ulength;
+    }
+    if (width > ulength) {
+        ulength = width;
+    }
+    if (ulength == 1) {
+        return PyUnicode_FromOrdinal(*dpos);
+    }
+    return __Pyx_PyUnicode_BuildFromAscii(ulength, dpos, (int) length, prepend_sign, padding_char);
+}
+
+/* PyObjectFormatAndDecref */
+static CYTHON_INLINE PyObject* __Pyx_PyObject_FormatSimpleAndDecref(PyObject* s, PyObject* f) {
+    if (unlikely(!s)) return NULL;
+    if (likely(PyUnicode_CheckExact(s))) return s;
+    #if PY_MAJOR_VERSION < 3
+    if (likely(PyString_CheckExact(s))) {
+        PyObject *result = PyUnicode_FromEncodedObject(s, NULL, "strict");
+        Py_DECREF(s);
+        return result;
+    }
+    #endif
+    return __Pyx_PyObject_FormatAndDecref(s, f);
+}
+static CYTHON_INLINE PyObject* __Pyx_PyObject_FormatAndDecref(PyObject* s, PyObject* f) {
+    PyObject *result = PyObject_Format(s, f);
+    Py_DECREF(s);
+    return result;
+}
+
 /* UnpackUnboundCMethod */
 static int __Pyx_TryUnpackUnboundCMethod(__Pyx_CachedCFunction* target) {
     PyObject *method;
     method = __Pyx_PyObject_GetAttrStr(target->type, *target->method_name);
     if (unlikely(!method))
         return -1;
     target->method = method;
@@ -48876,120 +49754,14 @@
                 else\
                     goto raise_overflow;\
             }\
         }\
         return (target_type) value;\
     }
 
-/* Print */
-#if !CYTHON_COMPILING_IN_PYPY && PY_MAJOR_VERSION < 3
-static PyObject *__Pyx_GetStdout(void) {
-    PyObject *f = PySys_GetObject((char *)"stdout");
-    if (!f) {
-        PyErr_SetString(PyExc_RuntimeError, "lost sys.stdout");
-    }
-    return f;
-}
-static int __Pyx_Print(PyObject* f, PyObject *arg_tuple, int newline) {
-    int i;
-    if (!f) {
-        if (!(f = __Pyx_GetStdout()))
-            return -1;
-    }
-    Py_INCREF(f);
-    for (i=0; i < PyTuple_GET_SIZE(arg_tuple); i++) {
-        PyObject* v;
-        if (PyFile_SoftSpace(f, 1)) {
-            if (PyFile_WriteString(" ", f) < 0)
-                goto error;
-        }
-        v = PyTuple_GET_ITEM(arg_tuple, i);
-        if (PyFile_WriteObject(v, f, Py_PRINT_RAW) < 0)
-            goto error;
-        if (PyString_Check(v)) {
-            char *s = PyString_AsString(v);
-            Py_ssize_t len = PyString_Size(v);
-            if (len > 0) {
-                switch (s[len-1]) {
-                    case ' ': break;
-                    case '\f': case '\r': case '\n': case '\t': case '\v':
-                        PyFile_SoftSpace(f, 0);
-                        break;
-                    default:  break;
-                }
-            }
-        }
-    }
-    if (newline) {
-        if (PyFile_WriteString("\n", f) < 0)
-            goto error;
-        PyFile_SoftSpace(f, 0);
-    }
-    Py_DECREF(f);
-    return 0;
-error:
-    Py_DECREF(f);
-    return -1;
-}
-#else
-static int __Pyx_Print(PyObject* stream, PyObject *arg_tuple, int newline) {
-    PyObject* kwargs = 0;
-    PyObject* result = 0;
-    PyObject* end_string;
-    if (unlikely(!__pyx_print)) {
-        __pyx_print = PyObject_GetAttr(__pyx_b, __pyx_n_s_print);
-        if (!__pyx_print)
-            return -1;
-    }
-    if (stream) {
-        kwargs = PyDict_New();
-        if (unlikely(!kwargs))
-            return -1;
-        if (unlikely(PyDict_SetItem(kwargs, __pyx_n_s_file, stream) < 0))
-            goto bad;
-        if (!newline) {
-            end_string = PyUnicode_FromStringAndSize(" ", 1);
-            if (unlikely(!end_string))
-                goto bad;
-            if (PyDict_SetItem(kwargs, __pyx_n_s_end, end_string) < 0) {
-                Py_DECREF(end_string);
-                goto bad;
-            }
-            Py_DECREF(end_string);
-        }
-    } else if (!newline) {
-        if (unlikely(!__pyx_print_kwargs)) {
-            __pyx_print_kwargs = PyDict_New();
-            if (unlikely(!__pyx_print_kwargs))
-                return -1;
-            end_string = PyUnicode_FromStringAndSize(" ", 1);
-            if (unlikely(!end_string))
-                return -1;
-            if (PyDict_SetItem(__pyx_print_kwargs, __pyx_n_s_end, end_string) < 0) {
-                Py_DECREF(end_string);
-                return -1;
-            }
-            Py_DECREF(end_string);
-        }
-        kwargs = __pyx_print_kwargs;
-    }
-    result = PyObject_Call(__pyx_print, arg_tuple, kwargs);
-    if (unlikely(kwargs) && (kwargs != __pyx_print_kwargs))
-        Py_DECREF(kwargs);
-    if (!result)
-        return -1;
-    Py_DECREF(result);
-    return 0;
-bad:
-    if (kwargs != __pyx_print_kwargs)
-        Py_XDECREF(kwargs);
-    return -1;
-}
-#endif
-
 /* CIntToPy */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_RFC_DIRECTION(RFC_DIRECTION value) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const RFC_DIRECTION neg_one = (RFC_DIRECTION) -1, const_zero = (RFC_DIRECTION) 0;
@@ -51474,51 +52246,14 @@
         int one = 1; int little = (int)*(unsigned char *)&one;
         unsigned char *bytes = (unsigned char *)&value;
         return _PyLong_FromByteArray(bytes, sizeof(RFC_INT8),
                                      little, !is_unsigned);
     }
 }
 
-/* PrintOne */
-#if !CYTHON_COMPILING_IN_PYPY && PY_MAJOR_VERSION < 3
-static int __Pyx_PrintOne(PyObject* f, PyObject *o) {
-    if (!f) {
-        if (!(f = __Pyx_GetStdout()))
-            return -1;
-    }
-    Py_INCREF(f);
-    if (PyFile_SoftSpace(f, 0)) {
-        if (PyFile_WriteString(" ", f) < 0)
-            goto error;
-    }
-    if (PyFile_WriteObject(o, f, Py_PRINT_RAW) < 0)
-        goto error;
-    if (PyFile_WriteString("\n", f) < 0)
-        goto error;
-    Py_DECREF(f);
-    return 0;
-error:
-    Py_DECREF(f);
-    return -1;
-    /* the line below is just to avoid C compiler
-     * warnings about unused functions */
-    return __Pyx_Print(f, NULL, 0);
-}
-#else
-static int __Pyx_PrintOne(PyObject* stream, PyObject *o) {
-    int res;
-    PyObject* arg_tuple = PyTuple_Pack(1, o);
-    if (unlikely(!arg_tuple))
-        return -1;
-    res = __Pyx_Print(stream, arg_tuple, 1);
-    Py_DECREF(arg_tuple);
-    return res;
-}
-#endif
-
 /* CIntFromPy */
 static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const long neg_one = (long) -1, const_zero = (long) 0;
```

### Comparing `pyrfc-2.8.2/src/pyrfc/_cyrfc.pyx` & `pyrfc-2.8.3/src/pyrfc/_cyrfc.pyx`

 * *Files identical despite different names*

### Comparing `pyrfc-2.8.2/src/pyrfc/_exception.py` & `pyrfc-2.8.3/src/pyrfc/_exception.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,14 +54,15 @@
         rc_text = RcCodeText(code).value if code in enum_values(RcCodeText) else "??"
         return (
             f"{rc_text} (rc={self.code}): key={self.key}, message={self.message}"
             f" [MSG: class={self.msg_class}, type={self.msg_type}, number={self.msg_number},"
             f" v1-4:={self.msg_v1};{self.msg_v2};{self.msg_v3};{self.msg_v4}]"
         )
 
+
 class ABAPApplicationError(RFCLibError):
     """ABAP application error
 
     This exception is raised if a RFC call returns an RC code greater than 0
     and the error object has an RFC_ERROR_GROUP value of
     ABAP_APPLICATION_FAILURE.
     """
```

### Comparing `pyrfc-2.8.2/src/pyrfc/csapnwrfc.pxd` & `pyrfc-2.8.3/src/pyrfc/csapnwrfc.pxd`

 * *Files identical despite different names*

