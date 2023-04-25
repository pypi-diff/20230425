# Comparing `tmp/odoo13_addon_partner_exception-13.0.1.0.1-py3-none-any.whl.zip` & `tmp/odoo13_addon_partner_exception-13.0.1.0.1.dev2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 14069 bytes, number of entries: 11
--rw-r--r--  2.0 unx      123 b- defN 23-Apr-25 13:02 odoo/addons/partner_exception/__init__.py
--rw-r--r--  2.0 unx      497 b- defN 23-Apr-25 13:02 odoo/addons/partner_exception/__manifest__.py
--rw-r--r--  2.0 unx     1240 b- defN 23-Apr-25 13:02 odoo/addons/partner_exception/i18n/partner_exception.pot
--rw-r--r--  2.0 unx       26 b- defN 23-Apr-25 13:02 odoo/addons/partner_exception/models/__init__.py
--rw-r--r--  2.0 unx     1373 b- defN 23-Apr-25 13:02 odoo/addons/partner_exception/models/res_partner.py
--rw-r--r--  2.0 unx     9455 b- defN 23-Apr-25 13:02 odoo/addons/partner_exception/static/description/icon.png
--rw-r--r--  2.0 unx      734 b- defN 23-Apr-25 13:02 odoo/addons/partner_exception/views/contact_views.xml
--rw-r--r--  2.0 unx      604 b- defN 23-Apr-25 13:02 odoo13_addon_partner_exception-13.0.1.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-25 13:02 odoo13_addon_partner_exception-13.0.1.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-Apr-25 13:02 odoo13_addon_partner_exception-13.0.1.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1153 b- defN 23-Apr-25 13:02 odoo13_addon_partner_exception-13.0.1.0.1.dist-info/RECORD
-11 files, 15302 bytes uncompressed, 12029 bytes compressed:  21.4%
+Zip file size: 14108 bytes, number of entries: 11
+-rw-r--r--  2.0 unx      123 b- defN 23-Mar-02 18:28 odoo/addons/partner_exception/__init__.py
+-rw-r--r--  2.0 unx      497 b- defN 23-Mar-02 18:28 odoo/addons/partner_exception/__manifest__.py
+-rw-r--r--  2.0 unx     1240 b- defN 23-Mar-02 18:28 odoo/addons/partner_exception/i18n/partner_exception.pot
+-rw-r--r--  2.0 unx       26 b- defN 23-Mar-02 18:28 odoo/addons/partner_exception/models/__init__.py
+-rw-r--r--  2.0 unx     1370 b- defN 23-Mar-02 18:28 odoo/addons/partner_exception/models/res_partner.py
+-rw-r--r--  2.0 unx     9455 b- defN 23-Mar-02 18:28 odoo/addons/partner_exception/static/description/icon.png
+-rw-r--r--  2.0 unx      734 b- defN 23-Mar-02 18:28 odoo/addons/partner_exception/views/contact_views.xml
+-rw-r--r--  2.0 unx      609 b- defN 23-Mar-02 18:28 odoo13_addon_partner_exception-13.0.1.0.1.dev2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Mar-02 18:28 odoo13_addon_partner_exception-13.0.1.0.1.dev2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 23-Mar-02 18:28 odoo13_addon_partner_exception-13.0.1.0.1.dev2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1173 b- defN 23-Mar-02 18:28 odoo13_addon_partner_exception-13.0.1.0.1.dev2.dist-info/RECORD
+11 files, 15324 bytes uncompressed, 12028 bytes compressed:  21.5%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: odoo/addons/partner_exception/static/description/icon.png
 Comment: 
 
 Filename: odoo/addons/partner_exception/views/contact_views.xml
 Comment: 
 
-Filename: odoo13_addon_partner_exception-13.0.1.0.1.dist-info/METADATA
+Filename: odoo13_addon_partner_exception-13.0.1.0.1.dev2.dist-info/METADATA
 Comment: 
 
-Filename: odoo13_addon_partner_exception-13.0.1.0.1.dist-info/WHEEL
+Filename: odoo13_addon_partner_exception-13.0.1.0.1.dev2.dist-info/WHEEL
 Comment: 
 
-Filename: odoo13_addon_partner_exception-13.0.1.0.1.dist-info/top_level.txt
+Filename: odoo13_addon_partner_exception-13.0.1.0.1.dev2.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo13_addon_partner_exception-13.0.1.0.1.dist-info/RECORD
+Filename: odoo13_addon_partner_exception-13.0.1.0.1.dev2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## odoo/addons/partner_exception/__manifest__.py

```diff
@@ -1,13 +1,13 @@
 # Copyright 2022 ForgeFlow, S.L.
 # License AGPL-3.0 or later (http://www.gnu.org/licenses/agpl.html).
 {
     "name": "Partner Exception",
     "summary": "Custom exceptions on partner contact",
-    "version": "13.0.1.0.1",
+    "version": "13.0.1.0.0",
     "category": "Generic Modules/Sale",
     "author": "Forgeflow, " "Odoo Community Association (OCA)",
     "website": "https://github.com/OCA/partner-contact",
     "depends": ["contacts", "base_exception"],
     "license": "AGPL-3",
     "data": ["views/contact_views.xml"],
 }
```

## odoo/addons/partner_exception/models/res_partner.py

```diff
@@ -10,15 +10,15 @@
     model = fields.Selection(selection_add=[("res.partner", "Contact")])
     partner_ids = fields.Many2many("res.partner", string="Contacts")
 
 
 class ResPartner(models.Model):
     _inherit = ["res.partner", "base.exception"]
     _name = "res.partner"
-    _order = "main_exception_id asc, display_name"
+    _order = "main_exception_id asc, name desc"
 
     @api.model
     def _reverse_field(self):
         return "partner_ids"
 
     def _fields_trigger_check_exception(self):
         return ["ignore_exception"]
```

## Comparing `odoo13_addon_partner_exception-13.0.1.0.1.dist-info/METADATA` & `odoo13_addon_partner_exception-13.0.1.0.1.dev2.dist-info/METADATA`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo13-addon-partner-exception
-Version: 13.0.1.0.1
+Version: 13.0.1.0.1.dev2
 Summary: Custom exceptions on partner contact
 Home-page: https://github.com/OCA/partner-contact
 Author: Forgeflow, Odoo Community Association (OCA)
 Author-email: support@odoo-community.org
 License: AGPL-3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

## Comparing `odoo13_addon_partner_exception-13.0.1.0.1.dist-info/RECORD` & `odoo13_addon_partner_exception-13.0.1.0.1.dev2.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 odoo/addons/partner_exception/__init__.py,sha256=15AqmlWgKJSJG8__DYEopR3m8aiwBx6RESKP8BOQIQU,123
-odoo/addons/partner_exception/__manifest__.py,sha256=gxxxRuayA00MuFXnnA9MOdJdurcJQv7izGVmnq4gjA8,497
+odoo/addons/partner_exception/__manifest__.py,sha256=9DGZ6MkcJXX7qpO65wjT79x38SpMSz3TWRfaygB5S-c,497
 odoo/addons/partner_exception/i18n/partner_exception.pot,sha256=VGeiWveni-ndDOKKOJcnh4ja_zFwNq9b9l8mCynBn_E,1240
 odoo/addons/partner_exception/models/__init__.py,sha256=g-Dp2ZwN6oB4CqdQfgRInNSzdMWAVQg1vjWL7S-ZODM,26
-odoo/addons/partner_exception/models/res_partner.py,sha256=fd76q5dx6ZNzvKK4Wj8x0khcdFJ62cXaj5UGu_f0hb0,1373
+odoo/addons/partner_exception/models/res_partner.py,sha256=9Qrcj8rywiUTyHSFDpo3rdHpQidt3odDyfMQE6psNxw,1370
 odoo/addons/partner_exception/static/description/icon.png,sha256=6xBPJauaFOF0KDHfHgQopSc28kKvxMaeoQFQWZtfZDo,9455
 odoo/addons/partner_exception/views/contact_views.xml,sha256=8nTKTXvWxRzPilZvSXW2aOzMHK3iUrYK9LQ-UXlRSz8,734
-odoo13_addon_partner_exception-13.0.1.0.1.dist-info/METADATA,sha256=zX1c7D98KK24K5sYc5_iZqlKqeyJYP_uSBkgJYtD-s8,604
-odoo13_addon_partner_exception-13.0.1.0.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-odoo13_addon_partner_exception-13.0.1.0.1.dist-info/top_level.txt,sha256=qBj40grFkGOfDZ2WDSw3y1RnDlgG0u8rP8pvGNdbz4w,5
-odoo13_addon_partner_exception-13.0.1.0.1.dist-info/RECORD,,
+odoo13_addon_partner_exception-13.0.1.0.1.dev2.dist-info/METADATA,sha256=yYhud5e8_1swnbtfNIlkVWAPpm6s8vAeVGgh2hcOHf8,609
+odoo13_addon_partner_exception-13.0.1.0.1.dev2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+odoo13_addon_partner_exception-13.0.1.0.1.dev2.dist-info/top_level.txt,sha256=qBj40grFkGOfDZ2WDSw3y1RnDlgG0u8rP8pvGNdbz4w,5
+odoo13_addon_partner_exception-13.0.1.0.1.dev2.dist-info/RECORD,,
```

