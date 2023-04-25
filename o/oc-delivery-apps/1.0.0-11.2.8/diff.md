# Comparing `tmp/oc_delivery_apps-1.0.0-py3-none-any.whl.zip` & `tmp/oc_delivery_apps-11.2.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,117 @@
-Zip file size: 39648 bytes, number of entries: 16
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 13:16 oc_delivery_apps/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 13:16 oc_delivery_apps/checksums/__init__.py
--rw-r--r--  2.0 unx      171 b- defN 23-Apr-14 13:16 oc_delivery_apps/checksums/apps.py
--rw-r--r--  2.0 unx     4756 b- defN 23-Apr-14 13:16 oc_delivery_apps/checksums/archive_object.py
--rw-r--r--  2.0 unx    60493 b- defN 23-Apr-14 13:16 oc_delivery_apps/checksums/controllers.py
--rw-r--r--  2.0 unx    11104 b- defN 23-Apr-14 13:16 oc_delivery_apps/checksums/models.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 13:16 oc_delivery_apps/dlcontents/__init__.py
--rw-r--r--  2.0 unx      172 b- defN 23-Apr-14 13:16 oc_delivery_apps/dlcontents/apps.py
--rw-r--r--  2.0 unx     4756 b- defN 23-Apr-14 13:16 oc_delivery_apps/dlcontents/archive_object.py
--rw-r--r--  2.0 unx    58734 b- defN 23-Apr-14 13:16 oc_delivery_apps/dlcontents/controllers.py
--rw-r--r--  2.0 unx     9313 b- defN 23-Apr-14 13:16 oc_delivery_apps/dlcontents/models.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Apr-14 13:16 oc_delivery_apps-1.0.0.dist-info/LICENSE
--rw-r--r--  2.0 unx      346 b- defN 23-Apr-14 13:16 oc_delivery_apps-1.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-14 13:16 oc_delivery_apps-1.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       17 b- defN 23-Apr-14 13:16 oc_delivery_apps-1.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1469 b- defN 23-Apr-14 13:16 oc_delivery_apps-1.0.0.dist-info/RECORD
-16 files, 162780 bytes uncompressed, 37164 bytes compressed:  77.2%
+Zip file size: 95256 bytes, number of entries: 115
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-25 12:39 oc_delivery_apps/__init__.py
+-rw-r--r--  2.0 unx     1851 b- defN 23-Apr-25 12:39 oc_delivery_apps/checksums/Component.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-25 12:39 oc_delivery_apps/checksums/__init__.py
+-rw-r--r--  2.0 unx      171 b- defN 23-Apr-25 12:39 oc_delivery_apps/checksums/apps.py
+-rw-r--r--  2.0 unx     4756 b- defN 23-Apr-25 12:39 oc_delivery_apps/checksums/archive_object.py
+-rw-r--r--  2.0 unx    60493 b- defN 23-Apr-25 12:39 oc_delivery_apps/checksums/controllers.py
+-rw-r--r--  2.0 unx    11096 b- defN 23-Apr-25 12:39 oc_delivery_apps/checksums/models.py
+-rw-r--r--  2.0 unx     3501 b- defN 23-Apr-25 12:39 oc_delivery_apps/checksums/migrations/0001_initial.py
+-rw-r--r--  2.0 unx     1144 b- defN 23-Apr-25 12:39 oc_delivery_apps/checksums/migrations/0002_auto_20170424_0902.py
+-rw-r--r--  2.0 unx     1223 b- defN 23-Apr-25 12:39 oc_delivery_apps/checksums/migrations/0003_auto_20170424_1235.py
+-rw-r--r--  2.0 unx      182 b- defN 23-Apr-25 12:39 oc_delivery_apps/checksums/migrations/0005_fileinfo.py
+-rw-r--r--  2.0 unx      404 b- defN 23-Apr-25 12:39 oc_delivery_apps/checksums/migrations/0006_citypes_is_deliverable.py
+-rw-r--r--  2.0 unx      434 b- defN 23-Apr-25 12:39 oc_delivery_apps/checksums/migrations/0007_locations_revision.py
+-rw-r--r--  2.0 unx      412 b- defN 23-Apr-25 12:39 oc_delivery_apps/checksums/migrations/0008_locations_is_deleted.py
+-rw-r--r--  2.0 unx     1966 b- defN 23-Apr-25 12:39 oc_delivery_apps/checksums/migrations/0009_auto_20171204_0100.py
+-rw-r--r--  2.0 unx     1260 b- defN 23-Apr-25 12:39 oc_delivery_apps/checksums/migrations/0010_citypegroups_citypeincs.py
+-rw-r--r--  2.0 unx      365 b- defN 23-Apr-25 12:39 oc_delivery_apps/checksums/migrations/0011_remove_citypegroups_rn_gav.py
+-rw-r--r--  2.0 unx      447 b- defN 23-Apr-25 12:39 oc_delivery_apps/checksums/migrations/0012_citypegroups_rn_artifactid.py
+-rw-r--r--  2.0 unx      816 b- defN 23-Apr-25 12:39 oc_delivery_apps/checksums/migrations/0013_auto_20180109_0127.py
+-rw-r--r--  2.0 unx      181 b- defN 23-Apr-25 12:39 oc_delivery_apps/checksums/migrations/0014_migrate_file_incs_data.py
+-rw-r--r--  2.0 unx      186 b- defN 23-Apr-25 12:39 oc_delivery_apps/checksums/migrations/0015_auto_20180126_0332.py
+-rw-r--r--  2.0 unx      182 b- defN 23-Apr-25 12:39 oc_delivery_apps/checksums/migrations/0016_citypeparms.py
+-rw-r--r--  2.0 unx      435 b- defN 23-Apr-25 12:39 oc_delivery_apps/checksums/migrations/0017_historicallocations_history_change_reason.py
+-rw-r--r--  2.0 unx      413 b- defN 23-Apr-25 12:39 oc_delivery_apps/checksums/migrations/0018_auto_20180312_0116.py
+-rw-r--r--  2.0 unx     2485 b- defN 23-Apr-25 12:39 oc_delivery_apps/checksums/migrations/0019_auto_20180326_0439.py
+-rw-r--r--  2.0 unx      181 b- defN 23-Apr-25 12:39 oc_delivery_apps/checksums/migrations/0020_cs_prov_migration.py
+-rw-r--r--  2.0 unx      866 b- defN 23-Apr-25 12:39 oc_delivery_apps/checksums/migrations/0021_auto_20180329_0242.py
+-rw-r--r--  2.0 unx      438 b- defN 23-Apr-25 12:39 oc_delivery_apps/checksums/migrations/0022_files_depth_level.py
+-rw-r--r--  2.0 unx      584 b- defN 23-Apr-25 12:39 oc_delivery_apps/checksums/migrations/0023_loc_db_index.py
+-rw-r--r--  2.0 unx      175 b- defN 23-Apr-25 12:39 oc_delivery_apps/checksums/migrations/0024_locations_dup_remove.py
+-rw-r--r--  2.0 unx      532 b- defN 23-Apr-25 12:39 oc_delivery_apps/checksums/migrations/0025_auto_20180412_0740.py
+-rw-r--r--  2.0 unx      180 b- defN 23-Apr-25 12:39 oc_delivery_apps/checksums/migrations/0026_auto_20180416_0413.py
+-rw-r--r--  2.0 unx      192 b- defN 23-Apr-25 12:39 oc_delivery_apps/checksums/migrations/0027_notnull_loc_rev.py
+-rw-r--r--  2.0 unx      177 b- defN 23-Apr-25 12:39 oc_delivery_apps/checksums/migrations/0028_auto_20180419_0719.py
+-rw-r--r--  2.0 unx      182 b- defN 23-Apr-25 12:39 oc_delivery_apps/checksums/migrations/0029_fake_id_reverse.py
+-rw-r--r--  2.0 unx      630 b- defN 23-Apr-25 12:39 oc_delivery_apps/checksums/migrations/0030_auto_20180514_2311.py
+-rw-r--r--  2.0 unx      182 b- defN 23-Apr-25 12:39 oc_delivery_apps/checksums/migrations/0031_auto_20180528_2344.py
+-rw-r--r--  2.0 unx      700 b- defN 23-Apr-25 12:39 oc_delivery_apps/checksums/migrations/0032_auto_20180703_0023.py
+-rw-r--r--  2.0 unx      806 b- defN 23-Apr-25 12:39 oc_delivery_apps/checksums/migrations/0033_auto_20200117_0810.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-25 12:39 oc_delivery_apps/checksums/migrations/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-25 12:39 oc_delivery_apps/dlcontents/__init__.py
+-rw-r--r--  2.0 unx      172 b- defN 23-Apr-25 12:39 oc_delivery_apps/dlcontents/apps.py
+-rw-r--r--  2.0 unx     4756 b- defN 23-Apr-25 12:39 oc_delivery_apps/dlcontents/archive_object.py
+-rw-r--r--  2.0 unx    58734 b- defN 23-Apr-25 12:39 oc_delivery_apps/dlcontents/controllers.py
+-rw-r--r--  2.0 unx     9313 b- defN 23-Apr-25 12:39 oc_delivery_apps/dlcontents/models.py
+-rw-r--r--  2.0 unx     3506 b- defN 23-Apr-25 12:39 oc_delivery_apps/dlcontents/migrations/0001_initial.py
+-rw-r--r--  2.0 unx     1148 b- defN 23-Apr-25 12:39 oc_delivery_apps/dlcontents/migrations/0002_auto_20170424_0902.py
+-rw-r--r--  2.0 unx     1226 b- defN 23-Apr-25 12:39 oc_delivery_apps/dlcontents/migrations/0003_auto_20170424_1235.py
+-rw-r--r--  2.0 unx      182 b- defN 23-Apr-25 12:39 oc_delivery_apps/dlcontents/migrations/0005_fileinfo.py
+-rw-r--r--  2.0 unx      405 b- defN 23-Apr-25 12:39 oc_delivery_apps/dlcontents/migrations/0006_citypes_is_deliverable.py
+-rw-r--r--  2.0 unx      435 b- defN 23-Apr-25 12:39 oc_delivery_apps/dlcontents/migrations/0007_locations_revision.py
+-rw-r--r--  2.0 unx      413 b- defN 23-Apr-25 12:39 oc_delivery_apps/dlcontents/migrations/0008_locations_is_deleted.py
+-rw-r--r--  2.0 unx     1969 b- defN 23-Apr-25 12:39 oc_delivery_apps/dlcontents/migrations/0009_auto_20171204_0100.py
+-rw-r--r--  2.0 unx     1263 b- defN 23-Apr-25 12:39 oc_delivery_apps/dlcontents/migrations/0010_citypegroups_citypeincs.py
+-rw-r--r--  2.0 unx      366 b- defN 23-Apr-25 12:39 oc_delivery_apps/dlcontents/migrations/0011_remove_citypegroups_rn_gav.py
+-rw-r--r--  2.0 unx      448 b- defN 23-Apr-25 12:39 oc_delivery_apps/dlcontents/migrations/0012_citypegroups_rn_artifactid.py
+-rw-r--r--  2.0 unx      819 b- defN 23-Apr-25 12:39 oc_delivery_apps/dlcontents/migrations/0013_auto_20180109_0127.py
+-rw-r--r--  2.0 unx      182 b- defN 23-Apr-25 12:39 oc_delivery_apps/dlcontents/migrations/0014_migrate_file_incs_data.py
+-rw-r--r--  2.0 unx      186 b- defN 23-Apr-25 12:39 oc_delivery_apps/dlcontents/migrations/0015_auto_20180126_0332.py
+-rw-r--r--  2.0 unx      182 b- defN 23-Apr-25 12:39 oc_delivery_apps/dlcontents/migrations/0016_citypeparms.py
+-rw-r--r--  2.0 unx      436 b- defN 23-Apr-25 12:39 oc_delivery_apps/dlcontents/migrations/0017_historicallocations_history_change_reason.py
+-rw-r--r--  2.0 unx      414 b- defN 23-Apr-25 12:39 oc_delivery_apps/dlcontents/migrations/0018_auto_20180312_0116.py
+-rw-r--r--  2.0 unx     2491 b- defN 23-Apr-25 12:39 oc_delivery_apps/dlcontents/migrations/0019_auto_20180326_0439.py
+-rw-r--r--  2.0 unx      182 b- defN 23-Apr-25 12:39 oc_delivery_apps/dlcontents/migrations/0020_cs_prov_migration.py
+-rw-r--r--  2.0 unx      867 b- defN 23-Apr-25 12:39 oc_delivery_apps/dlcontents/migrations/0021_auto_20180329_0242.py
+-rw-r--r--  2.0 unx      439 b- defN 23-Apr-25 12:39 oc_delivery_apps/dlcontents/migrations/0022_files_depth_level.py
+-rw-r--r--  2.0 unx      585 b- defN 23-Apr-25 12:39 oc_delivery_apps/dlcontents/migrations/0023_loc_db_index.py
+-rw-r--r--  2.0 unx      176 b- defN 23-Apr-25 12:39 oc_delivery_apps/dlcontents/migrations/0024_locations_dup_remove.py
+-rw-r--r--  2.0 unx      533 b- defN 23-Apr-25 12:39 oc_delivery_apps/dlcontents/migrations/0025_auto_20180412_0740.py
+-rw-r--r--  2.0 unx      181 b- defN 23-Apr-25 12:39 oc_delivery_apps/dlcontents/migrations/0026_auto_20180416_0413.py
+-rw-r--r--  2.0 unx      182 b- defN 23-Apr-25 12:39 oc_delivery_apps/dlcontents/migrations/0027_notnull_loc_rev.py
+-rw-r--r--  2.0 unx      178 b- defN 23-Apr-25 12:39 oc_delivery_apps/dlcontents/migrations/0028_auto_20180419_0719.py
+-rw-r--r--  2.0 unx      182 b- defN 23-Apr-25 12:39 oc_delivery_apps/dlcontents/migrations/0029_fake_id_reverse.py
+-rw-r--r--  2.0 unx      179 b- defN 23-Apr-25 12:39 oc_delivery_apps/dlcontents/migrations/0030_remove_dup_locations.py
+-rw-r--r--  2.0 unx     1269 b- defN 23-Apr-25 12:39 oc_delivery_apps/dlcontents/migrations/0031_loc_unique_idx.py
+-rw-r--r--  2.0 unx      178 b- defN 23-Apr-25 12:39 oc_delivery_apps/dlcontents/migrations/0032_auto_20180529_0123.py
+-rw-r--r--  2.0 unx      702 b- defN 23-Apr-25 12:39 oc_delivery_apps/dlcontents/migrations/0033_auto_20180703_0008.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-25 12:39 oc_delivery_apps/dlcontents/migrations/__init__.py
+-rw-r--r--  2.0 unx     5076 b- defN 23-Apr-25 12:39 oc_delivery_apps/dlmanager/DLModels.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-25 12:39 oc_delivery_apps/dlmanager/__init__.py
+-rw-r--r--  2.0 unx      169 b- defN 23-Apr-25 12:39 oc_delivery_apps/dlmanager/apps.py
+-rw-r--r--  2.0 unx     8572 b- defN 23-Apr-25 12:39 oc_delivery_apps/dlmanager/models.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-25 12:39 oc_delivery_apps/dlmanager/management/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-25 12:39 oc_delivery_apps/dlmanager/management/commands/__init__.py
+-rw-r--r--  2.0 unx     1905 b- defN 23-Apr-25 12:39 oc_delivery_apps/dlmanager/management/commands/fix_shifted_dates.py
+-rw-r--r--  2.0 unx     3923 b- defN 23-Apr-25 12:39 oc_delivery_apps/dlmanager/management/commands/init_delivery_history.py
+-rw-r--r--  2.0 unx     4060 b- defN 23-Apr-25 12:39 oc_delivery_apps/dlmanager/migrations/0001_initial.py
+-rw-r--r--  2.0 unx      310 b- defN 23-Apr-25 12:39 oc_delivery_apps/dlmanager/migrations/0002_remove_delivery_build_status.py
+-rw-r--r--  2.0 unx      403 b- defN 23-Apr-25 12:39 oc_delivery_apps/dlmanager/migrations/0003_delivery_build_status.py
+-rw-r--r--  2.0 unx      418 b- defN 23-Apr-25 12:39 oc_delivery_apps/dlmanager/migrations/0004_client_country.py
+-rw-r--r--  2.0 unx      378 b- defN 23-Apr-25 12:39 oc_delivery_apps/dlmanager/migrations/0005_delivery_creation_date.py
+-rw-r--r--  2.0 unx     4886 b- defN 23-Apr-25 12:39 oc_delivery_apps/dlmanager/migrations/0006_auto_20170113_1749.py
+-rw-r--r--  2.0 unx      666 b- defN 23-Apr-25 12:39 oc_delivery_apps/dlmanager/migrations/0007_clientemailaddress.py
+-rw-r--r--  2.0 unx      366 b- defN 23-Apr-25 12:39 oc_delivery_apps/dlmanager/migrations/0008_client_is_active.py
+-rw-r--r--  2.0 unx      367 b- defN 23-Apr-25 12:39 oc_delivery_apps/dlmanager/migrations/0009_auto_20170901_1032.py
+-rw-r--r--  2.0 unx      607 b- defN 23-Apr-25 12:39 oc_delivery_apps/dlmanager/migrations/0010_clientlanguage.py
+-rw-r--r--  2.0 unx      430 b- defN 23-Apr-25 12:39 oc_delivery_apps/dlmanager/migrations/0011_client_language.py
+-rw-r--r--  2.0 unx      634 b- defN 23-Apr-25 12:39 oc_delivery_apps/dlmanager/migrations/0012_ftpuploadextendedclient.py
+-rw-r--r--  2.0 unx      871 b- defN 23-Apr-25 12:39 oc_delivery_apps/dlmanager/migrations/0013_auto_20180125_0105.py
+-rw-r--r--  2.0 unx      596 b- defN 23-Apr-25 12:39 oc_delivery_apps/dlmanager/migrations/0014_auto_20180221_0312.py
+-rw-r--r--  2.0 unx      195 b- defN 23-Apr-25 12:39 oc_delivery_apps/dlmanager/migrations/0015_delete_dl_status_rollback.py
+-rw-r--r--  2.0 unx      391 b- defN 23-Apr-25 12:39 oc_delivery_apps/dlmanager/migrations/0016_ftpuploadclientoptions_can_receive.py
+-rw-r--r--  2.0 unx      532 b- defN 23-Apr-25 12:39 oc_delivery_apps/dlmanager/migrations/0017_privatefile.py
+-rw-r--r--  2.0 unx      770 b- defN 23-Apr-25 12:39 oc_delivery_apps/dlmanager/migrations/0018_jiraprojects.py
+-rw-r--r--  2.0 unx     1218 b- defN 23-Apr-25 12:39 oc_delivery_apps/dlmanager/migrations/0019_auto_20190219_0909.py
+-rw-r--r--  2.0 unx     1386 b- defN 23-Apr-25 12:39 oc_delivery_apps/dlmanager/migrations/0020_JiraInstances_Table_Addition.py
+-rw-r--r--  2.0 unx      618 b- defN 23-Apr-25 12:39 oc_delivery_apps/dlmanager/migrations/0021_AddedUniqueFields.py
+-rw-r--r--  2.0 unx      744 b- defN 23-Apr-25 12:39 oc_delivery_apps/dlmanager/migrations/0022_auto_20190319_0653.py
+-rw-r--r--  2.0 unx      369 b- defN 23-Apr-25 12:39 oc_delivery_apps/dlmanager/migrations/0023_jirainstances_priority.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-25 12:39 oc_delivery_apps/dlmanager/migrations/__init__.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Apr-25 12:39 oc_delivery_apps-11.2.8.dist-info/LICENSE
+-rw-r--r--  2.0 unx      435 b- defN 23-Apr-25 12:39 oc_delivery_apps-11.2.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-25 12:39 oc_delivery_apps-11.2.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 23-Apr-25 12:39 oc_delivery_apps-11.2.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    13253 b- defN 23-Apr-25 12:39 oc_delivery_apps-11.2.8.dist-info/RECORD
+115 files, 261121 bytes uncompressed, 72788 bytes compressed:  72.1%
```

## zipnote {}

```diff
@@ -1,10 +1,13 @@
 Filename: oc_delivery_apps/__init__.py
 Comment: 
 
+Filename: oc_delivery_apps/checksums/Component.py
+Comment: 
+
 Filename: oc_delivery_apps/checksums/__init__.py
 Comment: 
 
 Filename: oc_delivery_apps/checksums/apps.py
 Comment: 
 
 Filename: oc_delivery_apps/checksums/archive_object.py
@@ -12,14 +15,113 @@
 
 Filename: oc_delivery_apps/checksums/controllers.py
 Comment: 
 
 Filename: oc_delivery_apps/checksums/models.py
 Comment: 
 
+Filename: oc_delivery_apps/checksums/migrations/0001_initial.py
+Comment: 
+
+Filename: oc_delivery_apps/checksums/migrations/0002_auto_20170424_0902.py
+Comment: 
+
+Filename: oc_delivery_apps/checksums/migrations/0003_auto_20170424_1235.py
+Comment: 
+
+Filename: oc_delivery_apps/checksums/migrations/0005_fileinfo.py
+Comment: 
+
+Filename: oc_delivery_apps/checksums/migrations/0006_citypes_is_deliverable.py
+Comment: 
+
+Filename: oc_delivery_apps/checksums/migrations/0007_locations_revision.py
+Comment: 
+
+Filename: oc_delivery_apps/checksums/migrations/0008_locations_is_deleted.py
+Comment: 
+
+Filename: oc_delivery_apps/checksums/migrations/0009_auto_20171204_0100.py
+Comment: 
+
+Filename: oc_delivery_apps/checksums/migrations/0010_citypegroups_citypeincs.py
+Comment: 
+
+Filename: oc_delivery_apps/checksums/migrations/0011_remove_citypegroups_rn_gav.py
+Comment: 
+
+Filename: oc_delivery_apps/checksums/migrations/0012_citypegroups_rn_artifactid.py
+Comment: 
+
+Filename: oc_delivery_apps/checksums/migrations/0013_auto_20180109_0127.py
+Comment: 
+
+Filename: oc_delivery_apps/checksums/migrations/0014_migrate_file_incs_data.py
+Comment: 
+
+Filename: oc_delivery_apps/checksums/migrations/0015_auto_20180126_0332.py
+Comment: 
+
+Filename: oc_delivery_apps/checksums/migrations/0016_citypeparms.py
+Comment: 
+
+Filename: oc_delivery_apps/checksums/migrations/0017_historicallocations_history_change_reason.py
+Comment: 
+
+Filename: oc_delivery_apps/checksums/migrations/0018_auto_20180312_0116.py
+Comment: 
+
+Filename: oc_delivery_apps/checksums/migrations/0019_auto_20180326_0439.py
+Comment: 
+
+Filename: oc_delivery_apps/checksums/migrations/0020_cs_prov_migration.py
+Comment: 
+
+Filename: oc_delivery_apps/checksums/migrations/0021_auto_20180329_0242.py
+Comment: 
+
+Filename: oc_delivery_apps/checksums/migrations/0022_files_depth_level.py
+Comment: 
+
+Filename: oc_delivery_apps/checksums/migrations/0023_loc_db_index.py
+Comment: 
+
+Filename: oc_delivery_apps/checksums/migrations/0024_locations_dup_remove.py
+Comment: 
+
+Filename: oc_delivery_apps/checksums/migrations/0025_auto_20180412_0740.py
+Comment: 
+
+Filename: oc_delivery_apps/checksums/migrations/0026_auto_20180416_0413.py
+Comment: 
+
+Filename: oc_delivery_apps/checksums/migrations/0027_notnull_loc_rev.py
+Comment: 
+
+Filename: oc_delivery_apps/checksums/migrations/0028_auto_20180419_0719.py
+Comment: 
+
+Filename: oc_delivery_apps/checksums/migrations/0029_fake_id_reverse.py
+Comment: 
+
+Filename: oc_delivery_apps/checksums/migrations/0030_auto_20180514_2311.py
+Comment: 
+
+Filename: oc_delivery_apps/checksums/migrations/0031_auto_20180528_2344.py
+Comment: 
+
+Filename: oc_delivery_apps/checksums/migrations/0032_auto_20180703_0023.py
+Comment: 
+
+Filename: oc_delivery_apps/checksums/migrations/0033_auto_20200117_0810.py
+Comment: 
+
+Filename: oc_delivery_apps/checksums/migrations/__init__.py
+Comment: 
+
 Filename: oc_delivery_apps/dlcontents/__init__.py
 Comment: 
 
 Filename: oc_delivery_apps/dlcontents/apps.py
 Comment: 
 
 Filename: oc_delivery_apps/dlcontents/archive_object.py
@@ -27,23 +129,218 @@
 
 Filename: oc_delivery_apps/dlcontents/controllers.py
 Comment: 
 
 Filename: oc_delivery_apps/dlcontents/models.py
 Comment: 
 
-Filename: oc_delivery_apps-1.0.0.dist-info/LICENSE
+Filename: oc_delivery_apps/dlcontents/migrations/0001_initial.py
+Comment: 
+
+Filename: oc_delivery_apps/dlcontents/migrations/0002_auto_20170424_0902.py
+Comment: 
+
+Filename: oc_delivery_apps/dlcontents/migrations/0003_auto_20170424_1235.py
+Comment: 
+
+Filename: oc_delivery_apps/dlcontents/migrations/0005_fileinfo.py
+Comment: 
+
+Filename: oc_delivery_apps/dlcontents/migrations/0006_citypes_is_deliverable.py
+Comment: 
+
+Filename: oc_delivery_apps/dlcontents/migrations/0007_locations_revision.py
+Comment: 
+
+Filename: oc_delivery_apps/dlcontents/migrations/0008_locations_is_deleted.py
+Comment: 
+
+Filename: oc_delivery_apps/dlcontents/migrations/0009_auto_20171204_0100.py
+Comment: 
+
+Filename: oc_delivery_apps/dlcontents/migrations/0010_citypegroups_citypeincs.py
+Comment: 
+
+Filename: oc_delivery_apps/dlcontents/migrations/0011_remove_citypegroups_rn_gav.py
+Comment: 
+
+Filename: oc_delivery_apps/dlcontents/migrations/0012_citypegroups_rn_artifactid.py
+Comment: 
+
+Filename: oc_delivery_apps/dlcontents/migrations/0013_auto_20180109_0127.py
+Comment: 
+
+Filename: oc_delivery_apps/dlcontents/migrations/0014_migrate_file_incs_data.py
+Comment: 
+
+Filename: oc_delivery_apps/dlcontents/migrations/0015_auto_20180126_0332.py
+Comment: 
+
+Filename: oc_delivery_apps/dlcontents/migrations/0016_citypeparms.py
+Comment: 
+
+Filename: oc_delivery_apps/dlcontents/migrations/0017_historicallocations_history_change_reason.py
+Comment: 
+
+Filename: oc_delivery_apps/dlcontents/migrations/0018_auto_20180312_0116.py
+Comment: 
+
+Filename: oc_delivery_apps/dlcontents/migrations/0019_auto_20180326_0439.py
+Comment: 
+
+Filename: oc_delivery_apps/dlcontents/migrations/0020_cs_prov_migration.py
+Comment: 
+
+Filename: oc_delivery_apps/dlcontents/migrations/0021_auto_20180329_0242.py
+Comment: 
+
+Filename: oc_delivery_apps/dlcontents/migrations/0022_files_depth_level.py
+Comment: 
+
+Filename: oc_delivery_apps/dlcontents/migrations/0023_loc_db_index.py
+Comment: 
+
+Filename: oc_delivery_apps/dlcontents/migrations/0024_locations_dup_remove.py
+Comment: 
+
+Filename: oc_delivery_apps/dlcontents/migrations/0025_auto_20180412_0740.py
+Comment: 
+
+Filename: oc_delivery_apps/dlcontents/migrations/0026_auto_20180416_0413.py
+Comment: 
+
+Filename: oc_delivery_apps/dlcontents/migrations/0027_notnull_loc_rev.py
+Comment: 
+
+Filename: oc_delivery_apps/dlcontents/migrations/0028_auto_20180419_0719.py
+Comment: 
+
+Filename: oc_delivery_apps/dlcontents/migrations/0029_fake_id_reverse.py
+Comment: 
+
+Filename: oc_delivery_apps/dlcontents/migrations/0030_remove_dup_locations.py
+Comment: 
+
+Filename: oc_delivery_apps/dlcontents/migrations/0031_loc_unique_idx.py
+Comment: 
+
+Filename: oc_delivery_apps/dlcontents/migrations/0032_auto_20180529_0123.py
+Comment: 
+
+Filename: oc_delivery_apps/dlcontents/migrations/0033_auto_20180703_0008.py
+Comment: 
+
+Filename: oc_delivery_apps/dlcontents/migrations/__init__.py
+Comment: 
+
+Filename: oc_delivery_apps/dlmanager/DLModels.py
+Comment: 
+
+Filename: oc_delivery_apps/dlmanager/__init__.py
+Comment: 
+
+Filename: oc_delivery_apps/dlmanager/apps.py
+Comment: 
+
+Filename: oc_delivery_apps/dlmanager/models.py
+Comment: 
+
+Filename: oc_delivery_apps/dlmanager/management/__init__.py
+Comment: 
+
+Filename: oc_delivery_apps/dlmanager/management/commands/__init__.py
+Comment: 
+
+Filename: oc_delivery_apps/dlmanager/management/commands/fix_shifted_dates.py
+Comment: 
+
+Filename: oc_delivery_apps/dlmanager/management/commands/init_delivery_history.py
+Comment: 
+
+Filename: oc_delivery_apps/dlmanager/migrations/0001_initial.py
+Comment: 
+
+Filename: oc_delivery_apps/dlmanager/migrations/0002_remove_delivery_build_status.py
+Comment: 
+
+Filename: oc_delivery_apps/dlmanager/migrations/0003_delivery_build_status.py
+Comment: 
+
+Filename: oc_delivery_apps/dlmanager/migrations/0004_client_country.py
+Comment: 
+
+Filename: oc_delivery_apps/dlmanager/migrations/0005_delivery_creation_date.py
+Comment: 
+
+Filename: oc_delivery_apps/dlmanager/migrations/0006_auto_20170113_1749.py
+Comment: 
+
+Filename: oc_delivery_apps/dlmanager/migrations/0007_clientemailaddress.py
+Comment: 
+
+Filename: oc_delivery_apps/dlmanager/migrations/0008_client_is_active.py
+Comment: 
+
+Filename: oc_delivery_apps/dlmanager/migrations/0009_auto_20170901_1032.py
+Comment: 
+
+Filename: oc_delivery_apps/dlmanager/migrations/0010_clientlanguage.py
+Comment: 
+
+Filename: oc_delivery_apps/dlmanager/migrations/0011_client_language.py
+Comment: 
+
+Filename: oc_delivery_apps/dlmanager/migrations/0012_ftpuploadextendedclient.py
+Comment: 
+
+Filename: oc_delivery_apps/dlmanager/migrations/0013_auto_20180125_0105.py
+Comment: 
+
+Filename: oc_delivery_apps/dlmanager/migrations/0014_auto_20180221_0312.py
+Comment: 
+
+Filename: oc_delivery_apps/dlmanager/migrations/0015_delete_dl_status_rollback.py
+Comment: 
+
+Filename: oc_delivery_apps/dlmanager/migrations/0016_ftpuploadclientoptions_can_receive.py
+Comment: 
+
+Filename: oc_delivery_apps/dlmanager/migrations/0017_privatefile.py
+Comment: 
+
+Filename: oc_delivery_apps/dlmanager/migrations/0018_jiraprojects.py
+Comment: 
+
+Filename: oc_delivery_apps/dlmanager/migrations/0019_auto_20190219_0909.py
+Comment: 
+
+Filename: oc_delivery_apps/dlmanager/migrations/0020_JiraInstances_Table_Addition.py
+Comment: 
+
+Filename: oc_delivery_apps/dlmanager/migrations/0021_AddedUniqueFields.py
+Comment: 
+
+Filename: oc_delivery_apps/dlmanager/migrations/0022_auto_20190319_0653.py
+Comment: 
+
+Filename: oc_delivery_apps/dlmanager/migrations/0023_jirainstances_priority.py
+Comment: 
+
+Filename: oc_delivery_apps/dlmanager/migrations/__init__.py
+Comment: 
+
+Filename: oc_delivery_apps-11.2.8.dist-info/LICENSE
 Comment: 
 
-Filename: oc_delivery_apps-1.0.0.dist-info/METADATA
+Filename: oc_delivery_apps-11.2.8.dist-info/METADATA
 Comment: 
 
-Filename: oc_delivery_apps-1.0.0.dist-info/WHEEL
+Filename: oc_delivery_apps-11.2.8.dist-info/WHEEL
 Comment: 
 
-Filename: oc_delivery_apps-1.0.0.dist-info/top_level.txt
+Filename: oc_delivery_apps-11.2.8.dist-info/top_level.txt
 Comment: 
 
-Filename: oc_delivery_apps-1.0.0.dist-info/RECORD
+Filename: oc_delivery_apps-11.2.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## oc_delivery_apps/checksums/models.py

```diff
@@ -21,15 +21,15 @@
     # artifactid needed for documentation appending
     doc_artifactid = models.CharField(max_length=255, blank=True, null=True)
 
     def get_rn_gav(self, version):
         """
         Returns GAV of release notes of given version if artifactid is known, None otherwise
         """
-        
+
         if any([not self.rn_artifactid, not version]):
             return None
 
         _group_id = '.'.join([
             os.getenv("MVN_PREFIX") or "com.example",
             os.getenv("MVN_RN_SUFFIX") or "rn.sfx",
             "release_notes"])
```

## Comparing `oc_delivery_apps-1.0.0.dist-info/LICENSE` & `oc_delivery_apps-11.2.8.dist-info/LICENSE`

 * *Files identical despite different names*

