# Comparing `tmp/realnet-0.0.97.tar.gz` & `tmp/realnet-0.0.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "realnet-0.0.97.tar", last modified: Mon Apr 24 03:26:18 2023, max compression
+gzip compressed data, was "realnet-0.0.98.tar", last modified: Tue Apr 25 01:39:21 2023, max compression
```

## Comparing `realnet-0.0.97.tar` & `realnet-0.0.98.tar`

### file list

```diff
@@ -1,186 +1,186 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 03:26:18.457203 realnet-0.0.97/
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-04-24 03:23:26.000000 realnet-0.0.97/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7492 2023-04-24 03:26:18.457203 realnet-0.0.97/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7060 2023-04-24 03:23:26.000000 realnet-0.0.97/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 03:26:18.441203 realnet-0.0.97/realnet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 03:26:18.445203 realnet-0.0.97/realnet/cmd/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/cmd/create.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/cmd/get.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/cmd/info.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/cmd/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     6976 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/cmd/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 03:26:18.445203 realnet-0.0.97/realnet/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/core/acl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8432 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/core/hierarchy.py
--rw-r--r--   0 runner    (1001) docker     (123)    21596 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/core/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     9290 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/core/type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 03:26:18.445203 realnet-0.0.97/realnet/provider/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/provider/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 03:26:18.445203 realnet-0.0.97/realnet/provider/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/provider/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/provider/aws/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 03:26:18.445203 realnet-0.0.97/realnet/provider/generic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/provider/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/provider/generic/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/provider/generic/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/provider/generic/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 03:26:18.445203 realnet-0.0.97/realnet/provider/json/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/provider/json/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 03:26:18.445203 realnet-0.0.97/realnet/provider/sql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/provider/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/provider/sql/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/provider/sql/init.py
--rw-r--r--   0 runner    (1001) docker     (123)    17851 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/provider/sql/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    12486 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/provider/sql/org.py
--rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/provider/sql/orgs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 03:26:18.445203 realnet-0.0.97/realnet/provider/sql/postgres/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/provider/sql/postgres/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11838 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/provider/sql/postgres/item.py
--rw-r--r--   0 runner    (1001) docker     (123)     5206 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/provider/sql/roles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 03:26:18.445203 realnet-0.0.97/realnet/provider/sql/sqlite/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/provider/sql/sqlite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6589 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/provider/sql/type.py
--rw-r--r--   0 runner    (1001) docker     (123)    15084 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/provider/sql/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 03:26:18.445203 realnet-0.0.97/realnet/provider/xml/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/provider/xml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 03:26:18.445203 realnet-0.0.97/realnet/provider/yaml/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/provider/yaml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/realnet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 03:26:18.445203 realnet-0.0.97/realnet/resource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/resource/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 03:26:18.445203 realnet-0.0.97/realnet/resource/accounts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/resource/accounts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/resource/accounts/accounts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 03:26:18.445203 realnet-0.0.97/realnet/resource/apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/resource/apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/resource/apps/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 03:26:18.445203 realnet-0.0.97/realnet/resource/attributes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/resource/attributes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/resource/attributes/attributes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 03:26:18.445203 realnet-0.0.97/realnet/resource/auths/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/resource/auths/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/resource/auths/auths.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 03:26:18.445203 realnet-0.0.97/realnet/resource/chatgpt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/resource/chatgpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/resource/chatgpt/chatgpt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 03:26:18.445203 realnet-0.0.97/realnet/resource/clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/resource/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/resource/clients/clients.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 03:26:18.449203 realnet-0.0.97/realnet/resource/ctrls/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/resource/ctrls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/resource/ctrls/ctrls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 03:26:18.449203 realnet-0.0.97/realnet/resource/endpoints/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/resource/endpoints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/resource/endpoints/endpoints.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 03:26:18.449203 realnet-0.0.97/realnet/resource/files/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/resource/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/resource/files/files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 03:26:18.449203 realnet-0.0.97/realnet/resource/forms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/resource/forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/resource/forms/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 03:26:18.449203 realnet-0.0.97/realnet/resource/gltf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/resource/gltf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6723 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/resource/gltf/export.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/resource/gltf/gltf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 03:26:18.449203 realnet-0.0.97/realnet/resource/groups/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/resource/groups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/resource/groups/groups.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 03:26:18.449203 realnet-0.0.97/realnet/resource/items/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/resource/items/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35333 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/resource/items/items.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 03:26:18.449203 realnet-0.0.97/realnet/resource/login/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/resource/login/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/resource/login/login.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 03:26:18.449203 realnet-0.0.97/realnet/resource/public/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/resource/public/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/resource/public/public.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 03:26:18.449203 realnet-0.0.97/realnet/resource/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/resource/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/resource/resources/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 03:26:18.449203 realnet-0.0.97/realnet/resource/roles/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/resource/roles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/resource/roles/roles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 03:26:18.449203 realnet-0.0.97/realnet/resource/types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/resource/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21652 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/resource/types/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 03:26:18.449203 realnet-0.0.97/realnet/resource/views/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/resource/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/resource/views/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 03:26:18.449203 realnet-0.0.97/realnet/runner/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/runner/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 03:26:18.449203 realnet-0.0.97/realnet/runner/http/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/runner/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/runner/http/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     7670 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/runner/http/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    21472 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/runner/http/router.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/runner/http/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 03:26:18.449203 realnet-0.0.97/realnet/runner/http/static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/runner/http/static/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 03:26:18.441203 realnet-0.0.97/realnet/runner/http/static/font-awesome/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 03:26:18.449203 realnet-0.0.97/realnet/runner/http/static/font-awesome/css/
--rw-r--r--   0 runner    (1001) docker     (123)    37414 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/runner/http/static/font-awesome/css/font-awesome.css
--rw-r--r--   0 runner    (1001) docker     (123)    31000 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/runner/http/static/font-awesome/css/font-awesome.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 03:26:18.453203 realnet-0.0.97/realnet/runner/http/static/font-awesome/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)   134808 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/runner/http/static/font-awesome/fonts/FontAwesome.otf
--rw-r--r--   0 runner    (1001) docker     (123)   165742 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/runner/http/static/font-awesome/fonts/fontawesome-webfont.eot
--rw-r--r--   0 runner    (1001) docker     (123)   444379 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/runner/http/static/font-awesome/fonts/fontawesome-webfont.svg
--rw-r--r--   0 runner    (1001) docker     (123)   165548 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/runner/http/static/font-awesome/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    98024 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/runner/http/static/font-awesome/fonts/fontawesome-webfont.woff
--rw-r--r--   0 runner    (1001) docker     (123)    77160 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/runner/http/static/font-awesome/fonts/fontawesome-webfont.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 03:26:18.441203 realnet-0.0.97/realnet/runner/http/static/scripts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 03:26:18.453203 realnet-0.0.97/realnet/runner/http/static/scripts/ace/
--rw-r--r--   0 runner    (1001) docker     (123)   373401 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/runner/http/static/scripts/ace/ace.js
--rw-r--r--   0 runner    (1001) docker     (123)    13008 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/runner/http/static/scripts/ace/ext-beautify.js
--rw-r--r--   0 runner    (1001) docker     (123)    39778 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/runner/http/static/scripts/ace/ext-language_tools.js
--rw-r--r--   0 runner    (1001) docker     (123)    31853 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/runner/http/static/scripts/ace/mode-css.js
--rw-r--r--   0 runner    (1001) docker     (123)   101769 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/runner/http/static/scripts/ace/mode-html.js
--rw-r--r--   0 runner    (1001) docker     (123)    18573 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/runner/http/static/scripts/ace/mode-javascript.js
--rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/runner/http/static/scripts/ace/mode-json.js
--rw-r--r--   0 runner    (1001) docker     (123)     8244 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/runner/http/static/scripts/ace/mode-python.js
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/runner/http/static/scripts/ace/theme-monokai.js
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/runner/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 03:26:18.453203 realnet-0.0.97/realnet/runner/sqs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/runner/sqs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/runner/sqs/sqs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 03:26:18.453203 realnet-0.0.97/realnet/shell/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/shell/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/shell/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/shell/cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/shell/proto.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/shell/shell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 03:26:18.453203 realnet-0.0.97/realnet/static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/static/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 03:26:18.457203 realnet-0.0.97/realnet/static/initialization/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/static/initialization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/static/initialization/access.json
--rw-r--r--   0 runner    (1001) docker     (123)    24153 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/static/initialization/apps.json
--rw-r--r--   0 runner    (1001) docker     (123)    13136 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/static/initialization/controls.json
--rw-r--r--   0 runner    (1001) docker     (123)    38721 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/static/initialization/core.json
--rw-r--r--   0 runner    (1001) docker     (123)   115082 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/static/initialization/forms.json
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/static/initialization/geometry.json
--rw-r--r--   0 runner    (1001) docker     (123)     4783 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/static/initialization/views.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 03:26:18.457203 realnet-0.0.97/realnet/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10742 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/templates/control.html
--rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/templates/form.html
--rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/templates/item.html
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/templates/login.html
--rw-r--r--   0 runner    (1001) docker     (123)    16417 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/templates/main.html
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/templates/nav.html
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/templates/register.html
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/templates/register_org.html
--rw-r--r--   0 runner    (1001) docker     (123)    26169 2023-04-24 03:23:26.000000 realnet-0.0.97/realnet/templates/view.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 03:26:18.445203 realnet-0.0.97/realnet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7492 2023-04-24 03:26:18.000000 realnet-0.0.97/realnet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-04-24 03:26:18.000000 realnet-0.0.97/realnet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 03:26:18.000000 realnet-0.0.97/realnet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-24 03:26:18.000000 realnet-0.0.97/realnet.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-24 03:26:18.000000 realnet-0.0.97/realnet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-24 03:26:18.000000 realnet-0.0.97/realnet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 03:26:18.457203 realnet-0.0.97/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-04-24 03:23:29.000000 realnet-0.0.97/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.771448 realnet-0.0.98/
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-04-25 01:36:27.000000 realnet-0.0.98/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7492 2023-04-25 01:39:21.771448 realnet-0.0.98/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7060 2023-04-25 01:36:27.000000 realnet-0.0.98/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.751448 realnet-0.0.98/realnet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.755448 realnet-0.0.98/realnet/cmd/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/cmd/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/cmd/get.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/cmd/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/cmd/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6976 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/cmd/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.755448 realnet-0.0.98/realnet/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/core/acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8432 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/core/hierarchy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21596 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/core/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9290 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/core/type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.755448 realnet-0.0.98/realnet/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/provider/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.755448 realnet-0.0.98/realnet/provider/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/provider/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/provider/aws/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.759448 realnet-0.0.98/realnet/provider/generic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/provider/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/provider/generic/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/provider/generic/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/provider/generic/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.759448 realnet-0.0.98/realnet/provider/json/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/provider/json/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.759448 realnet-0.0.98/realnet/provider/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/provider/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/provider/sql/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/provider/sql/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17851 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/provider/sql/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12486 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/provider/sql/org.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/provider/sql/orgs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.759448 realnet-0.0.98/realnet/provider/sql/postgres/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/provider/sql/postgres/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11838 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/provider/sql/postgres/item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5206 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/provider/sql/roles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.759448 realnet-0.0.98/realnet/provider/sql/sqlite/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/provider/sql/sqlite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6589 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/provider/sql/type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15084 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/provider/sql/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.759448 realnet-0.0.98/realnet/provider/xml/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/provider/xml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.759448 realnet-0.0.98/realnet/provider/yaml/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/provider/yaml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/realnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.759448 realnet-0.0.98/realnet/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/resource/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.759448 realnet-0.0.98/realnet/resource/accounts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/resource/accounts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/resource/accounts/accounts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.759448 realnet-0.0.98/realnet/resource/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/resource/apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/resource/apps/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.759448 realnet-0.0.98/realnet/resource/attributes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/resource/attributes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/resource/attributes/attributes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.759448 realnet-0.0.98/realnet/resource/auths/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/resource/auths/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/resource/auths/auths.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.759448 realnet-0.0.98/realnet/resource/chatgpt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/resource/chatgpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/resource/chatgpt/chatgpt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.759448 realnet-0.0.98/realnet/resource/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/resource/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/resource/clients/clients.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.759448 realnet-0.0.98/realnet/resource/ctrls/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/resource/ctrls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/resource/ctrls/ctrls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.759448 realnet-0.0.98/realnet/resource/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/resource/endpoints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/resource/endpoints/endpoints.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.759448 realnet-0.0.98/realnet/resource/files/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/resource/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/resource/files/files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.759448 realnet-0.0.98/realnet/resource/forms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/resource/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/resource/forms/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.759448 realnet-0.0.98/realnet/resource/gltf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/resource/gltf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6723 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/resource/gltf/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/resource/gltf/gltf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.763448 realnet-0.0.98/realnet/resource/groups/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/resource/groups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/resource/groups/groups.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.763448 realnet-0.0.98/realnet/resource/items/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/resource/items/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35333 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/resource/items/items.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.763448 realnet-0.0.98/realnet/resource/login/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/resource/login/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/resource/login/login.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.763448 realnet-0.0.98/realnet/resource/public/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/resource/public/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/resource/public/public.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.763448 realnet-0.0.98/realnet/resource/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/resource/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/resource/resources/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.763448 realnet-0.0.98/realnet/resource/roles/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/resource/roles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/resource/roles/roles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.763448 realnet-0.0.98/realnet/resource/types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/resource/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21652 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/resource/types/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.763448 realnet-0.0.98/realnet/resource/views/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/resource/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/resource/views/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.763448 realnet-0.0.98/realnet/runner/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/runner/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.763448 realnet-0.0.98/realnet/runner/http/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/runner/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/runner/http/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7670 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/runner/http/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21472 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/runner/http/router.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/runner/http/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.763448 realnet-0.0.98/realnet/runner/http/static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/runner/http/static/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.747448 realnet-0.0.98/realnet/runner/http/static/font-awesome/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.763448 realnet-0.0.98/realnet/runner/http/static/font-awesome/css/
+-rw-r--r--   0 runner    (1001) docker     (123)    37414 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/runner/http/static/font-awesome/css/font-awesome.css
+-rw-r--r--   0 runner    (1001) docker     (123)    31000 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/runner/http/static/font-awesome/css/font-awesome.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.767448 realnet-0.0.98/realnet/runner/http/static/font-awesome/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   134808 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/runner/http/static/font-awesome/fonts/FontAwesome.otf
+-rw-r--r--   0 runner    (1001) docker     (123)   165742 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/runner/http/static/font-awesome/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   444379 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/runner/http/static/font-awesome/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   165548 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/runner/http/static/font-awesome/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    98024 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/runner/http/static/font-awesome/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    77160 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/runner/http/static/font-awesome/fonts/fontawesome-webfont.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.747448 realnet-0.0.98/realnet/runner/http/static/scripts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.767448 realnet-0.0.98/realnet/runner/http/static/scripts/ace/
+-rw-r--r--   0 runner    (1001) docker     (123)   373401 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/runner/http/static/scripts/ace/ace.js
+-rw-r--r--   0 runner    (1001) docker     (123)    13008 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/runner/http/static/scripts/ace/ext-beautify.js
+-rw-r--r--   0 runner    (1001) docker     (123)    39778 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/runner/http/static/scripts/ace/ext-language_tools.js
+-rw-r--r--   0 runner    (1001) docker     (123)    31853 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/runner/http/static/scripts/ace/mode-css.js
+-rw-r--r--   0 runner    (1001) docker     (123)   101769 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/runner/http/static/scripts/ace/mode-html.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18573 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/runner/http/static/scripts/ace/mode-javascript.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/runner/http/static/scripts/ace/mode-json.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8244 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/runner/http/static/scripts/ace/mode-python.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/runner/http/static/scripts/ace/theme-monokai.js
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/runner/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.767448 realnet-0.0.98/realnet/runner/sqs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/runner/sqs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/runner/sqs/sqs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.767448 realnet-0.0.98/realnet/shell/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/shell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/shell/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/shell/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/shell/proto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/shell/shell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.767448 realnet-0.0.98/realnet/static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/static/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.767448 realnet-0.0.98/realnet/static/initialization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/static/initialization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/static/initialization/access.json
+-rw-r--r--   0 runner    (1001) docker     (123)    24153 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/static/initialization/apps.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13136 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/static/initialization/controls.json
+-rw-r--r--   0 runner    (1001) docker     (123)    38721 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/static/initialization/core.json
+-rw-r--r--   0 runner    (1001) docker     (123)   114896 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/static/initialization/forms.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/static/initialization/geometry.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4783 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/static/initialization/views.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.771448 realnet-0.0.98/realnet/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10742 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/templates/control.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/templates/form.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/templates/item.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/templates/login.html
+-rw-r--r--   0 runner    (1001) docker     (123)    16417 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/templates/main.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/templates/nav.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/templates/register.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/templates/register_org.html
+-rw-r--r--   0 runner    (1001) docker     (123)    26169 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/templates/view.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.755448 realnet-0.0.98/realnet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7492 2023-04-25 01:39:21.000000 realnet-0.0.98/realnet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-04-25 01:39:21.000000 realnet-0.0.98/realnet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 01:39:21.000000 realnet-0.0.98/realnet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-25 01:39:21.000000 realnet-0.0.98/realnet.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-25 01:39:21.000000 realnet-0.0.98/realnet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-25 01:39:21.000000 realnet-0.0.98/realnet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 01:39:21.771448 realnet-0.0.98/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-04-25 01:36:33.000000 realnet-0.0.98/setup.py
```

### Comparing `realnet-0.0.97/LICENSE` & `realnet-0.0.98/LICENSE`

 * *Files identical despite different names*

### Comparing `realnet-0.0.97/PKG-INFO` & `realnet-0.0.98/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: realnet
-Version: 0.0.97
+Version: 0.0.98
 Summary: Realnet command line interface
 Home-page: https://github.com/virtual-space/realnet
 Author: Marko Laban
 Author-email: marko.laban@l33tsystems.com
 License: BSD
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `realnet-0.0.97/README.md` & `realnet-0.0.98/README.md`

 * *Files identical despite different names*

### Comparing `realnet-0.0.97/realnet/cmd/server.py` & `realnet-0.0.98/realnet/cmd/server.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.97/realnet/core/config.py` & `realnet-0.0.98/realnet/core/config.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.97/realnet/core/hierarchy.py` & `realnet-0.0.98/realnet/core/hierarchy.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.97/realnet/core/provider.py` & `realnet-0.0.98/realnet/core/provider.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.97/realnet/core/type.py` & `realnet-0.0.98/realnet/core/type.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.97/realnet/provider/aws/data.py` & `realnet-0.0.98/realnet/provider/aws/data.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.97/realnet/provider/generic/endpoint.py` & `realnet-0.0.98/realnet/provider/generic/endpoint.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.97/realnet/provider/generic/resource.py` & `realnet-0.0.98/realnet/provider/generic/resource.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.97/realnet/provider/sql/client.py` & `realnet-0.0.98/realnet/provider/sql/client.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.97/realnet/provider/sql/init.py` & `realnet-0.0.98/realnet/provider/sql/init.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.97/realnet/provider/sql/models.py` & `realnet-0.0.98/realnet/provider/sql/models.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.97/realnet/provider/sql/org.py` & `realnet-0.0.98/realnet/provider/sql/org.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.97/realnet/provider/sql/orgs.py` & `realnet-0.0.98/realnet/provider/sql/orgs.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.97/realnet/provider/sql/postgres/item.py` & `realnet-0.0.98/realnet/provider/sql/postgres/item.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.97/realnet/provider/sql/roles.py` & `realnet-0.0.98/realnet/provider/sql/roles.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.97/realnet/provider/sql/type.py` & `realnet-0.0.98/realnet/provider/sql/type.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.97/realnet/provider/sql/utility.py` & `realnet-0.0.98/realnet/provider/sql/utility.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.97/realnet/resource/accounts/accounts.py` & `realnet-0.0.98/realnet/resource/accounts/accounts.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.97/realnet/resource/apps/apps.py` & `realnet-0.0.98/realnet/resource/apps/apps.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.97/realnet/resource/auths/auths.py` & `realnet-0.0.98/realnet/resource/auths/auths.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.97/realnet/resource/chatgpt/chatgpt.py` & `realnet-0.0.98/realnet/resource/chatgpt/chatgpt.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.97/realnet/resource/clients/clients.py` & `realnet-0.0.98/realnet/resource/clients/clients.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.97/realnet/resource/ctrls/ctrls.py` & `realnet-0.0.98/realnet/resource/ctrls/ctrls.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.97/realnet/resource/files/files.py` & `realnet-0.0.98/realnet/resource/files/files.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.97/realnet/resource/gltf/export.py` & `realnet-0.0.98/realnet/resource/gltf/export.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.97/realnet/resource/gltf/gltf.py` & `realnet-0.0.98/realnet/resource/gltf/gltf.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.97/realnet/resource/groups/groups.py` & `realnet-0.0.98/realnet/resource/groups/groups.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.97/realnet/resource/items/items.py` & `realnet-0.0.98/realnet/resource/items/items.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.97/realnet/resource/login/login.py` & `realnet-0.0.98/realnet/resource/login/login.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.97/realnet/resource/roles/roles.py` & `realnet-0.0.98/realnet/resource/roles/roles.py`

 * *Files 6% similar despite different names*

```diff
@@ -75,9 +75,14 @@
         account = module.get_account()
         if account.is_superuser() or account.is_admin():
             if 'parent_id' in args and 'id' in args:
                 module.remove_role_app(args['parent_id'], args['id'])
                 return redirect('/roles/{}'.format(args['parent_id']))
             elif 'id' in args:
                 module.delete_role(args['id'])
+            elif path:
+                parts = path.split('/')
+                if len(parts) == 3 and parts[1] == 'apps':
+                    module.remove_role_app(parts[0], parts[2])
+                    return redirect('/roles/{}'.format(parts[0]))
 
         return self.render_item(module, endpoint, args, path, content_type)
```

### Comparing `realnet-0.0.97/realnet/resource/types/types.py` & `realnet-0.0.98/realnet/resource/types/types.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.97/realnet/resource/views/views.py` & `realnet-0.0.98/realnet/resource/views/views.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.97/realnet/runner/http/app.py` & `realnet-0.0.98/realnet/runner/http/app.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.97/realnet/runner/http/auth.py` & `realnet-0.0.98/realnet/runner/http/auth.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.97/realnet/runner/http/router.py` & `realnet-0.0.98/realnet/runner/http/router.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.97/realnet/runner/http/static/font-awesome/css/font-awesome.css` & `realnet-0.0.98/realnet/runner/http/static/font-awesome/css/font-awesome.css`

 * *Files identical despite different names*

### Comparing `realnet-0.0.97/realnet/runner/http/static/font-awesome/css/font-awesome.min.css` & `realnet-0.0.98/realnet/runner/http/static/font-awesome/css/font-awesome.min.css`

 * *Files identical despite different names*

### Comparing `realnet-0.0.97/realnet/runner/http/static/font-awesome/fonts/FontAwesome.otf` & `realnet-0.0.98/realnet/runner/http/static/font-awesome/fonts/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `realnet-0.0.97/realnet/runner/http/static/font-awesome/fonts/fontawesome-webfont.eot` & `realnet-0.0.98/realnet/runner/http/static/font-awesome/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `realnet-0.0.97/realnet/runner/http/static/font-awesome/fonts/fontawesome-webfont.svg` & `realnet-0.0.98/realnet/runner/http/static/font-awesome/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `realnet-0.0.97/realnet/runner/http/static/font-awesome/fonts/fontawesome-webfont.ttf` & `realnet-0.0.98/realnet/runner/http/static/font-awesome/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `realnet-0.0.97/realnet/runner/http/static/font-awesome/fonts/fontawesome-webfont.woff` & `realnet-0.0.98/realnet/runner/http/static/font-awesome/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `realnet-0.0.97/realnet/runner/http/static/font-awesome/fonts/fontawesome-webfont.woff2` & `realnet-0.0.98/realnet/runner/http/static/font-awesome/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `realnet-0.0.97/realnet/runner/http/static/scripts/ace/ace.js` & `realnet-0.0.98/realnet/runner/http/static/scripts/ace/ace.js`

 * *Files identical despite different names*

### Comparing `realnet-0.0.97/realnet/runner/http/static/scripts/ace/ext-beautify.js` & `realnet-0.0.98/realnet/runner/http/static/scripts/ace/ext-beautify.js`

 * *Files identical despite different names*

### Comparing `realnet-0.0.97/realnet/runner/http/static/scripts/ace/ext-language_tools.js` & `realnet-0.0.98/realnet/runner/http/static/scripts/ace/ext-language_tools.js`

 * *Files identical despite different names*

### Comparing `realnet-0.0.97/realnet/runner/http/static/scripts/ace/mode-css.js` & `realnet-0.0.98/realnet/runner/http/static/scripts/ace/mode-css.js`

 * *Files identical despite different names*

### Comparing `realnet-0.0.97/realnet/runner/http/static/scripts/ace/mode-html.js` & `realnet-0.0.98/realnet/runner/http/static/scripts/ace/mode-html.js`

 * *Files identical despite different names*

### Comparing `realnet-0.0.97/realnet/runner/http/static/scripts/ace/mode-javascript.js` & `realnet-0.0.98/realnet/runner/http/static/scripts/ace/mode-javascript.js`

 * *Files identical despite different names*

### Comparing `realnet-0.0.97/realnet/runner/http/static/scripts/ace/mode-json.js` & `realnet-0.0.98/realnet/runner/http/static/scripts/ace/mode-json.js`

 * *Files identical despite different names*

### Comparing `realnet-0.0.97/realnet/runner/http/static/scripts/ace/mode-python.js` & `realnet-0.0.98/realnet/runner/http/static/scripts/ace/mode-python.js`

 * *Files identical despite different names*

### Comparing `realnet-0.0.97/realnet/runner/http/static/scripts/ace/theme-monokai.js` & `realnet-0.0.98/realnet/runner/http/static/scripts/ace/theme-monokai.js`

 * *Files identical despite different names*

### Comparing `realnet-0.0.97/realnet/shell/cmd.py` & `realnet-0.0.98/realnet/shell/cmd.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.97/realnet/shell/proto.py` & `realnet-0.0.98/realnet/shell/proto.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.97/realnet/shell/shell.py` & `realnet-0.0.98/realnet/shell/shell.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.97/realnet/static/initialization/access.json` & `realnet-0.0.98/realnet/static/initialization/access.json`

 * *Files identical despite different names*

### Comparing `realnet-0.0.97/realnet/static/initialization/apps.json` & `realnet-0.0.98/realnet/static/initialization/apps.json`

 * *Files identical despite different names*

### Comparing `realnet-0.0.97/realnet/static/initialization/controls.json` & `realnet-0.0.98/realnet/static/initialization/controls.json`

 * *Files identical despite different names*

### Comparing `realnet-0.0.97/realnet/static/initialization/core.json` & `realnet-0.0.98/realnet/static/initialization/core.json`

 * *Files identical despite different names*

### Comparing `realnet-0.0.97/realnet/static/initialization/forms.json` & `realnet-0.0.98/realnet/static/initialization/forms.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9993371212121211%*

 * *Differences: {"'types'": "{49: {'attributes': {'type': 'Item', 'controls': {delete: [1]}, 'path': 'items'}}, "*

 * *            "52: {'attributes': {'type': 'Query'}}}"}*

```diff
@@ -3063,21 +3063,14 @@
                             "target": "name"
                         },
                         "name": "Name",
                         "type": "EditCtrl"
                     },
                     {
                         "attributes": {
-                            "target": "attributes"
-                        },
-                        "name": "Attributes",
-                        "type": "EditCtrl"
-                    },
-                    {
-                        "attributes": {
                             "close": "true",
                             "is_cancel_button": "true",
                             "order": "8"
                         },
                         "name": "Cancel",
                         "type": "ButtonCtrl"
                     },
@@ -3088,15 +3081,16 @@
                             "default": "true",
                             "order": "9"
                         },
                         "name": "Save",
                         "type": "ButtonCtrl"
                     }
                 ],
-                "type": "Form"
+                "path": "items",
+                "type": "Item"
             },
             "base": "EditForm",
             "name": "SettingsForm"
         },
         {
             "attributes": {
                 "controls": [
@@ -3329,15 +3323,16 @@
                             "default": "true",
                             "order": "9"
                         },
                         "name": "Save",
                         "type": "ButtonCtrl"
                     }
                 ],
-                "path": "queries"
+                "path": "queries",
+                "type": "Query"
             },
             "base": "EditForm",
             "name": "QueryForm"
         },
         {
             "base": "Form",
             "name": "SharingForm"
```

### Comparing `realnet-0.0.97/realnet/static/initialization/geometry.json` & `realnet-0.0.98/realnet/static/initialization/geometry.json`

 * *Files identical despite different names*

### Comparing `realnet-0.0.97/realnet/static/initialization/views.json` & `realnet-0.0.98/realnet/static/initialization/views.json`

 * *Files identical despite different names*

### Comparing `realnet-0.0.97/realnet/templates/control.html` & `realnet-0.0.98/realnet/templates/control.html`

 * *Files identical despite different names*

### Comparing `realnet-0.0.97/realnet/templates/form.html` & `realnet-0.0.98/realnet/templates/form.html`

 * *Files identical despite different names*

### Comparing `realnet-0.0.97/realnet/templates/item.html` & `realnet-0.0.98/realnet/templates/item.html`

 * *Files identical despite different names*

### Comparing `realnet-0.0.97/realnet/templates/login.html` & `realnet-0.0.98/realnet/templates/login.html`

 * *Files identical despite different names*

### Comparing `realnet-0.0.97/realnet/templates/main.html` & `realnet-0.0.98/realnet/templates/main.html`

 * *Files identical despite different names*

### Comparing `realnet-0.0.97/realnet/templates/nav.html` & `realnet-0.0.98/realnet/templates/nav.html`

 * *Files identical despite different names*

### Comparing `realnet-0.0.97/realnet/templates/register.html` & `realnet-0.0.98/realnet/templates/register.html`

 * *Files identical despite different names*

### Comparing `realnet-0.0.97/realnet/templates/register_org.html` & `realnet-0.0.98/realnet/templates/register_org.html`

 * *Files identical despite different names*

### Comparing `realnet-0.0.97/realnet/templates/view.html` & `realnet-0.0.98/realnet/templates/view.html`

 * *Files identical despite different names*

### Comparing `realnet-0.0.97/realnet.egg-info/PKG-INFO` & `realnet-0.0.98/realnet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: realnet
-Version: 0.0.97
+Version: 0.0.98
 Summary: Realnet command line interface
 Home-page: https://github.com/virtual-space/realnet
 Author: Marko Laban
 Author-email: marko.laban@l33tsystems.com
 License: BSD
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `realnet-0.0.97/realnet.egg-info/SOURCES.txt` & `realnet-0.0.98/realnet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `realnet-0.0.97/setup.py` & `realnet-0.0.98/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="realnet",
-    version="0.0.97",
+    version="0.0.98",
     description="Realnet command line interface",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/virtual-space/realnet",
     author="Marko Laban",
     author_email="marko.laban@l33tsystems.com",
     license="BSD",
```

