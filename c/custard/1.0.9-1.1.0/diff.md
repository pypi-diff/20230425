# Comparing `tmp/custard-1.0.9.tar.gz` & `tmp/custard-1.1.0.tar.gz`

## Comparing `custard-1.0.9.tar` & `custard-1.1.0.tar`

### file list

```diff
@@ -1,127 +1,174 @@
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 custard-1.0.9/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 custard-1.0.9/custard/__init__.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 custard-1.0.9/custard/cache/__init__.py
--rw-r--r--   0        0        0     4936 2020-02-02 00:00:00.000000 custard-1.0.9/custard/cache/async_lru.py
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 custard-1.0.9/custard/cache/async_lur.md
--rw-r--r--   0        0        0    11971 2020-02-02 00:00:00.000000 custard-1.0.9/custard/cache/redis.py
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 custard-1.0.9/custard/core/__init__.py
--rw-r--r--   0        0        0   770279 2020-02-02 00:00:00.000000 custard-1.0.9/custard/core/decode.py
--rw-r--r--   0        0        0    31269 2020-02-02 00:00:00.000000 custard-1.0.9/custard/core/factory.py
--rw-r--r--   0        0        0     2978 2020-02-02 00:00:00.000000 custard-1.0.9/custard/core/kerberos.py
--rw-r--r--   0        0        0    30562 2020-02-02 00:00:00.000000 custard-1.0.9/custard/core/processor.py
--rw-r--r--   0        0        0    23875 2020-02-02 00:00:00.000000 custard-1.0.9/custard/core/regular.py
--rw-r--r--   0        0        0     1959 2020-02-02 00:00:00.000000 custard-1.0.9/custard/core/snowflake.py
--rw-r--r--   0        0        0     4542 2020-02-02 00:00:00.000000 custard-1.0.9/custard/core/system.py
--rw-r--r--   0        0        0    22331 2020-02-02 00:00:00.000000 custard-1.0.9/custard/core/useragent.py
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 custard-1.0.9/custard/core/xml2dict.py
--rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 custard-1.0.9/custard/core/xprint.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 custard-1.0.9/custard/cron/__init__.py
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 custard-1.0.9/custard/cron/batch_task.py
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 custard-1.0.9/custard/crypto/__init__.py
--rw-r--r--   0        0        0    15727 2020-02-02 00:00:00.000000 custard-1.0.9/custard/crypto/crypto.py
--rw-r--r--   0        0        0     3226 2020-02-02 00:00:00.000000 custard-1.0.9/custard/crypto/streambody.py
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 custard-1.0.9/custard/db/__init__.py
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 custard-1.0.9/custard/db/exc.py
--rw-r--r--   0        0        0     4810 2020-02-02 00:00:00.000000 custard-1.0.9/custard/db/inspect.py
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 custard-1.0.9/custard/db/logger.py
--rw-r--r--   0        0        0     4769 2020-02-02 00:00:00.000000 custard-1.0.9/custard/db/utils.py
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 custard-1.0.9/custard/expect/__init__.py
--rw-r--r--   0        0        0     1287 2020-02-02 00:00:00.000000 custard-1.0.9/custard/expect/context.py
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 custard-1.0.9/custard/expect/exceptions.py
--rw-r--r--   0        0        0     3424 2020-02-02 00:00:00.000000 custard-1.0.9/custard/expect/record.py
--rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 custard-1.0.9/custard/expect/spacer.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 custard-1.0.9/custard/extra/__init__.py
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 custard-1.0.9/custard/function/__init__.py
--rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 custard-1.0.9/custard/function/callsource.py
--rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 custard-1.0.9/custard/function/traverse.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 custard-1.0.9/custard/hitfilter/__init__.py
--rw-r--r--   0        0        0     2948 2020-02-02 00:00:00.000000 custard-1.0.9/custard/hitfilter/hitfilter.py
--rw-r--r--   0        0        0   761348 2020-02-02 00:00:00.000000 custard-1.0.9/custard/hitfilter/keywords
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 custard-1.0.9/custard/json/__init__.py
--rw-r--r--   0        0        0     9316 2020-02-02 00:00:00.000000 custard-1.0.9/custard/json/jsonlogger.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 custard-1.0.9/custard/kaptcha/__init__.py
--rw-r--r--   0        0        0     9495 2020-02-02 00:00:00.000000 custard-1.0.9/custard/kaptcha/captcha.py
--rw-r--r--   0        0        0   171508 2020-02-02 00:00:00.000000 custard-1.0.9/custard/kaptcha/font1.ttf
--rw-r--r--   0        0        0    42452 2020-02-02 00:00:00.000000 custard-1.0.9/custard/kaptcha/font2.ttf
--rw-r--r--   0        0        0    92956 2020-02-02 00:00:00.000000 custard-1.0.9/custard/kaptcha/font3.ttf
--rw-r--r--   0        0        0   314452 2020-02-02 00:00:00.000000 custard-1.0.9/custard/kaptcha/font4.ttf
--rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 custard-1.0.9/custard/limiter/__init__.py
--rw-r--r--   0        0        0     2106 2020-02-02 00:00:00.000000 custard-1.0.9/custard/limiter/depends.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 custard-1.0.9/custard/limiter/enums.py
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 custard-1.0.9/custard/limiter/execres.py
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 custard-1.0.9/custard/lock/__init__.py
--rw-r--r--   0        0        0     3070 2020-02-02 00:00:00.000000 custard-1.0.9/custard/lock/redis_lock.py
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 custard-1.0.9/custard/lock/thread_lock.py
--rw-r--r--   0        0        0    12051 2020-02-02 00:00:00.000000 custard-1.0.9/custard/lodash/README.md
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 custard-1.0.9/custard/lodash/__init__.py
--rw-r--r--   0        0        0     5417 2020-02-02 00:00:00.000000 custard-1.0.9/custard/lodash/arrays.py
--rw-r--r--   0        0        0     4307 2020-02-02 00:00:00.000000 custard-1.0.9/custard/lodash/maths.py
--rw-r--r--   0        0        0     3474 2020-02-02 00:00:00.000000 custard-1.0.9/custard/lodash/number.py
--rw-r--r--   0        0        0     7238 2020-02-02 00:00:00.000000 custard-1.0.9/custard/lodash/string.py
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 custard-1.0.9/custard/lodash/utilities.py
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 custard-1.0.9/custard/minioss/__init__.py
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 custard-1.0.9/custard/minioss/aliyun.py
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 custard-1.0.9/custard/minioss/enums.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 custard-1.0.9/custard/minioss/gitee.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 custard-1.0.9/custard/minioss/minio.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 custard-1.0.9/custard/minioss/qiniu.py
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 custard-1.0.9/custard/minioss/tencent.py
--rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 custard-1.0.9/custard/mock/__init__.py
--rw-r--r--   0        0        0    14510 2020-02-02 00:00:00.000000 custard-1.0.9/custard/mock/mini_racer.py
--rw-r--r--   0        0        0   366292 2020-02-02 00:00:00.000000 custard-1.0.9/custard/mock/mock.min.js
--rw-r--r--   0        0        0   292581 2020-02-02 00:00:00.000000 custard-1.0.9/custard/mock/mock.old.min.js
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 custard-1.0.9/custard/network/asynchttp.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 custard-1.0.9/custard/network/enums.py
--rw-r--r--   0        0        0     3426 2020-02-02 00:00:00.000000 custard-1.0.9/custard/network/httpclient.py
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 custard-1.0.9/custard/pagination/__init__.py
--rw-r--r--   0        0        0     4269 2020-02-02 00:00:00.000000 custard-1.0.9/custard/pagination/api.py
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 custard-1.0.9/custard/pagination/async_sqlalchemy.py
--rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 custard-1.0.9/custard/pagination/bases.py
--rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 custard-1.0.9/custard/pagination/default.py
--rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 custard-1.0.9/custard/pagination/iterables.py
--rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 custard-1.0.9/custard/pagination/limit_offset.py
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 custard-1.0.9/custard/pagination/pagination.py
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 custard-1.0.9/custard/pagination/paginator.py
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 custard-1.0.9/custard/pagination/sync_sqlalchemy.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 custard-1.0.9/custard/pio/__init__.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 custard-1.0.9/custard/script/__init__.py
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 custard-1.0.9/custard/script/compat.py
--rw-r--r--   0        0        0    16449 2020-02-02 00:00:00.000000 custard-1.0.9/custard/script/parser.py
--rw-r--r--   0        0        0     2589 2020-02-02 00:00:00.000000 custard-1.0.9/custard/script/schema.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 custard-1.0.9/custard/socket/__init__.py
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 custard-1.0.9/custard/swagger/__init__.py
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 custard-1.0.9/custard/swagger/exception.py
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 custard-1.0.9/custard/swagger/loader.py
--rw-r--r--   0        0        0     6766 2020-02-02 00:00:00.000000 custard-1.0.9/custard/swagger/swagger.py
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 custard-1.0.9/custard/swagger/utils.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 custard-1.0.9/custard/system/__init__.py
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 custard-1.0.9/custard/time/__init__.py
--rw-r--r--   0        0        0     6215 2020-02-02 00:00:00.000000 custard-1.0.9/custard/time/dafunc.py
--rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 custard-1.0.9/custard/time/exceptions.py
--rw-r--r--   0        0        0     5964 2020-02-02 00:00:00.000000 custard-1.0.9/custard/time/moment.py
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 custard-1.0.9/custard/time/stoppable_thread.py
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 custard-1.0.9/custard/utils/__init__.py
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 custard-1.0.9/custard/utils/datasets.py
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 custard-1.0.9/custard/utils/decorators.py
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 custard-1.0.9/custard/utils/text.py
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 custard-1.0.9/examples/async_lur.py
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 custard-1.0.9/examples/crypto.py
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 custard-1.0.9/examples/datum.py
--rw-r--r--   0        0        0     3650 2020-02-02 00:00:00.000000 custard-1.0.9/examples/decorator.py
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 custard-1.0.9/examples/dts.py
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 custard-1.0.9/examples/hitfilter.py
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 custard-1.0.9/examples/hitfilter_keyword
--rw-r--r--   0        0        0     8968 2020-02-02 00:00:00.000000 custard-1.0.9/examples/json_logger.py
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 custard-1.0.9/examples/kaptcha.py
--rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 custard-1.0.9/examples/kaptcha_execution_time.py
--rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 custard-1.0.9/examples/limiter.py
--rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 custard-1.0.9/examples/mock.py
--rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 custard-1.0.9/examples/pagination_async_sqlalchemy.py
--rw-r--r--   0        0        0     2170 2020-02-02 00:00:00.000000 custard-1.0.9/examples/pagination_sqlalchemy.py
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 custard-1.0.9/examples/swagger_online_change.py
--rw-r--r--   0        0        0     6447 2020-02-02 00:00:00.000000 custard-1.0.9/examples/swagger_usabletest.py
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 custard-1.0.9/examples/useragent.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 custard-1.0.9/.gitignore
--rw-r--r--   0        0        0     6988 2020-02-02 00:00:00.000000 custard-1.0.9/README.md
--rw-r--r--   0        0        0     4215 2020-02-02 00:00:00.000000 custard-1.0.9/pyproject.toml
--rw-r--r--   0        0        0    10024 2020-02-02 00:00:00.000000 custard-1.0.9/PKG-INFO
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 custard-1.1.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 custard-1.1.0/.vscode/launch.json
+-rw-r--r--   0        0        0     3993 2020-02-02 00:00:00.000000 custard-1.1.0/.vscode/settings.json
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 custard-1.1.0/custard/__init__.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 custard-1.1.0/custard/cache/__init__.py
+-rw-r--r--   0        0        0     4936 2020-02-02 00:00:00.000000 custard-1.1.0/custard/cache/async_lru.py
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 custard-1.1.0/custard/cache/async_lur.md
+-rw-r--r--   0        0        0    11971 2020-02-02 00:00:00.000000 custard-1.1.0/custard/cache/redis.py
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 custard-1.1.0/custard/core/__init__.py
+-rw-r--r--   0        0        0   770279 2020-02-02 00:00:00.000000 custard-1.1.0/custard/core/decode.py
+-rw-r--r--   0        0        0    28578 2020-02-02 00:00:00.000000 custard-1.1.0/custard/core/factory.py
+-rw-r--r--   0        0        0     2978 2020-02-02 00:00:00.000000 custard-1.1.0/custard/core/kerberos.py
+-rw-r--r--   0        0        0    30562 2020-02-02 00:00:00.000000 custard-1.1.0/custard/core/processor.py
+-rw-r--r--   0        0        0    23875 2020-02-02 00:00:00.000000 custard-1.1.0/custard/core/regular.py
+-rw-r--r--   0        0        0     1959 2020-02-02 00:00:00.000000 custard-1.1.0/custard/core/snowflake.py
+-rw-r--r--   0        0        0     5196 2020-02-02 00:00:00.000000 custard-1.1.0/custard/core/system.py
+-rw-r--r--   0        0        0    22331 2020-02-02 00:00:00.000000 custard-1.1.0/custard/core/useragent.py
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 custard-1.1.0/custard/core/xml2dict.py
+-rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 custard-1.1.0/custard/core/xprint.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 custard-1.1.0/custard/cron/__init__.py
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 custard-1.1.0/custard/cron/batch_task.py
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 custard-1.1.0/custard/crypto/__init__.py
+-rw-r--r--   0        0        0    15727 2020-02-02 00:00:00.000000 custard-1.1.0/custard/crypto/crypto.py
+-rw-r--r--   0        0        0     3226 2020-02-02 00:00:00.000000 custard-1.1.0/custard/crypto/streambody.py
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 custard-1.1.0/custard/curl/__init__.py
+-rw-r--r--   0        0        0     5883 2020-02-02 00:00:00.000000 custard-1.1.0/custard/curl/parse.py
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 custard-1.1.0/custard/db/__init__.py
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 custard-1.1.0/custard/db/exc.py
+-rw-r--r--   0        0        0     4810 2020-02-02 00:00:00.000000 custard-1.1.0/custard/db/inspect.py
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 custard-1.1.0/custard/db/logger.py
+-rw-r--r--   0        0        0     4769 2020-02-02 00:00:00.000000 custard-1.1.0/custard/db/utils.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 custard-1.1.0/custard/expect/__init__.py
+-rw-r--r--   0        0        0     1287 2020-02-02 00:00:00.000000 custard-1.1.0/custard/expect/context.py
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 custard-1.1.0/custard/expect/exceptions.py
+-rw-r--r--   0        0        0     3424 2020-02-02 00:00:00.000000 custard-1.1.0/custard/expect/record.py
+-rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 custard-1.1.0/custard/expect/spacer.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 custard-1.1.0/custard/extra/__init__.py
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 custard-1.1.0/custard/function/__init__.py
+-rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 custard-1.1.0/custard/function/callsource.py
+-rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 custard-1.1.0/custard/function/traverse.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 custard-1.1.0/custard/hitfilter/__init__.py
+-rw-r--r--   0        0        0     2948 2020-02-02 00:00:00.000000 custard-1.1.0/custard/hitfilter/hitfilter.py
+-rw-r--r--   0        0        0   761348 2020-02-02 00:00:00.000000 custard-1.1.0/custard/hitfilter/keywords
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 custard-1.1.0/custard/json/__init__.py
+-rw-r--r--   0        0        0     9316 2020-02-02 00:00:00.000000 custard-1.1.0/custard/json/jsonlogger.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 custard-1.1.0/custard/kaptcha/__init__.py
+-rw-r--r--   0        0        0     9495 2020-02-02 00:00:00.000000 custard-1.1.0/custard/kaptcha/captcha.py
+-rw-r--r--   0        0        0   171508 2020-02-02 00:00:00.000000 custard-1.1.0/custard/kaptcha/font1.ttf
+-rw-r--r--   0        0        0    42452 2020-02-02 00:00:00.000000 custard-1.1.0/custard/kaptcha/font2.ttf
+-rw-r--r--   0        0        0    92956 2020-02-02 00:00:00.000000 custard-1.1.0/custard/kaptcha/font3.ttf
+-rw-r--r--   0        0        0   314452 2020-02-02 00:00:00.000000 custard-1.1.0/custard/kaptcha/font4.ttf
+-rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 custard-1.1.0/custard/limiter/__init__.py
+-rw-r--r--   0        0        0     2106 2020-02-02 00:00:00.000000 custard-1.1.0/custard/limiter/depends.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 custard-1.1.0/custard/limiter/enums.py
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 custard-1.1.0/custard/limiter/execres.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 custard-1.1.0/custard/lock/__init__.py
+-rw-r--r--   0        0        0     3070 2020-02-02 00:00:00.000000 custard-1.1.0/custard/lock/redis_lock.py
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 custard-1.1.0/custard/lock/thread_lock.py
+-rw-r--r--   0        0        0    12051 2020-02-02 00:00:00.000000 custard-1.1.0/custard/lodash/README.md
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 custard-1.1.0/custard/lodash/__init__.py
+-rw-r--r--   0        0        0     5417 2020-02-02 00:00:00.000000 custard-1.1.0/custard/lodash/arrays.py
+-rw-r--r--   0        0        0     4307 2020-02-02 00:00:00.000000 custard-1.1.0/custard/lodash/maths.py
+-rw-r--r--   0        0        0     3474 2020-02-02 00:00:00.000000 custard-1.1.0/custard/lodash/number.py
+-rw-r--r--   0        0        0     7238 2020-02-02 00:00:00.000000 custard-1.1.0/custard/lodash/string.py
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 custard-1.1.0/custard/lodash/utilities.py
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 custard-1.1.0/custard/minioss/__init__.py
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 custard-1.1.0/custard/minioss/aliyun.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 custard-1.1.0/custard/minioss/enums.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 custard-1.1.0/custard/minioss/gitee.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 custard-1.1.0/custard/minioss/minio.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 custard-1.1.0/custard/minioss/qiniu.py
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 custard-1.1.0/custard/minioss/tencent.py
+-rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 custard-1.1.0/custard/mock/__init__.py
+-rw-r--r--   0        0        0    14510 2020-02-02 00:00:00.000000 custard-1.1.0/custard/mock/mini_racer.py
+-rw-r--r--   0        0        0   366292 2020-02-02 00:00:00.000000 custard-1.1.0/custard/mock/mock.min.js
+-rw-r--r--   0        0        0   292581 2020-02-02 00:00:00.000000 custard-1.1.0/custard/mock/mock.old.min.js
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 custard-1.1.0/custard/network/asynchttp.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 custard-1.1.0/custard/network/enums.py
+-rw-r--r--   0        0        0     3426 2020-02-02 00:00:00.000000 custard-1.1.0/custard/network/httpclient.py
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 custard-1.1.0/custard/pagination/__init__.py
+-rw-r--r--   0        0        0     4269 2020-02-02 00:00:00.000000 custard-1.1.0/custard/pagination/api.py
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 custard-1.1.0/custard/pagination/async_sqlalchemy.py
+-rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 custard-1.1.0/custard/pagination/bases.py
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 custard-1.1.0/custard/pagination/default.py
+-rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 custard-1.1.0/custard/pagination/iterables.py
+-rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 custard-1.1.0/custard/pagination/limit_offset.py
+-rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 custard-1.1.0/custard/pagination/pagination.py
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 custard-1.1.0/custard/pagination/paginator.py
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 custard-1.1.0/custard/pagination/sync_sqlalchemy.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 custard-1.1.0/custard/pio/__init__.py
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 custard-1.1.0/custard/rediscluster/__init__.py
+-rw-r--r--   0        0        0    49431 2020-02-02 00:00:00.000000 custard-1.1.0/custard/rediscluster/client.py
+-rw-r--r--   0        0        0    23993 2020-02-02 00:00:00.000000 custard-1.1.0/custard/rediscluster/connection.py
+-rw-r--r--   0        0        0     2722 2020-02-02 00:00:00.000000 custard-1.1.0/custard/rediscluster/crc.py
+-rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 custard-1.1.0/custard/rediscluster/exceptions.py
+-rw-r--r--   0        0        0    17930 2020-02-02 00:00:00.000000 custard-1.1.0/custard/rediscluster/nodemanager.py
+-rw-r--r--   0        0        0    19857 2020-02-02 00:00:00.000000 custard-1.1.0/custard/rediscluster/pipeline.py
+-rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 custard-1.1.0/custard/rediscluster/pubsub.py
+-rw-r--r--   0        0        0     6161 2020-02-02 00:00:00.000000 custard-1.1.0/custard/rediscluster/utils.py
+-rw-r--r--   0        0        0     3730 2020-02-02 00:00:00.000000 custard-1.1.0/custard/rediscluster/benchmarks/simple.py
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 custard-1.1.0/custard/rediscluster/docs/authors.md
+-rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 custard-1.1.0/custard/rediscluster/docs/benchmarks.md
+-rw-r--r--   0        0        0     5039 2020-02-02 00:00:00.000000 custard-1.1.0/custard/rediscluster/docs/client.md
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 custard-1.1.0/custard/rediscluster/docs/logging.md
+-rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 custard-1.1.0/custard/rediscluster/docs/readonly-mode.md
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 custard-1.1.0/custard/rediscluster/docs/scripting.md
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 custard-1.1.0/custard/rediscluster/examples/basic.py
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 custard-1.1.0/custard/rediscluster/examples/basic_elasticache_password_protected.py
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 custard-1.1.0/custard/rediscluster/examples/basic_password_protected.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 custard-1.1.0/custard/rediscluster/examples/from_url_password_protected.py
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 custard-1.1.0/custard/rediscluster/examples/generate_slot_keys.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 custard-1.1.0/custard/rediscluster/examples/incr-test-writer.py
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 custard-1.1.0/custard/rediscluster/examples/pipeline-incrby.py
+-rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 custard-1.1.0/custard/rediscluster/examples/pipeline-readonly-replicas.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 custard-1.1.0/custard/rediscluster/tests/__init__.py
+-rw-r--r--   0        0        0     8789 2020-02-02 00:00:00.000000 custard-1.1.0/custard/rediscluster/tests/conftest.py
+-rw-r--r--   0        0        0    49667 2020-02-02 00:00:00.000000 custard-1.1.0/custard/rediscluster/tests/redis-trib.rb
+-rw-r--r--   0        0        0    36527 2020-02-02 00:00:00.000000 custard-1.1.0/custard/rediscluster/tests/test_cluster_connection_pool.py
+-rw-r--r--   0        0        0    21628 2020-02-02 00:00:00.000000 custard-1.1.0/custard/rediscluster/tests/test_cluster_node_manager.py
+-rw-r--r--   0        0        0    20803 2020-02-02 00:00:00.000000 custard-1.1.0/custard/rediscluster/tests/test_cluster_obj.py
+-rw-r--r--   0        0        0   103248 2020-02-02 00:00:00.000000 custard-1.1.0/custard/rediscluster/tests/test_commands.py
+-rw-r--r--   0        0        0    17579 2020-02-02 00:00:00.000000 custard-1.1.0/custard/rediscluster/tests/test_commands_cluster.py
+-rw-r--r--   0        0        0     4355 2020-02-02 00:00:00.000000 custard-1.1.0/custard/rediscluster/tests/test_encoding.py
+-rw-r--r--   0        0        0     3155 2020-02-02 00:00:00.000000 custard-1.1.0/custard/rediscluster/tests/test_encoding_cluster.py
+-rw-r--r--   0        0        0     8016 2020-02-02 00:00:00.000000 custard-1.1.0/custard/rediscluster/tests/test_lock.py
+-rw-r--r--   0        0        0     2402 2020-02-02 00:00:00.000000 custard-1.1.0/custard/rediscluster/tests/test_monitor.py
+-rw-r--r--   0        0        0     5774 2020-02-02 00:00:00.000000 custard-1.1.0/custard/rediscluster/tests/test_multiprocessing.py
+-rw-r--r--   0        0        0     5386 2020-02-02 00:00:00.000000 custard-1.1.0/custard/rediscluster/tests/test_multiprocessing_cluster.py
+-rw-r--r--   0        0        0    12150 2020-02-02 00:00:00.000000 custard-1.1.0/custard/rediscluster/tests/test_pipeline.py
+-rw-r--r--   0        0        0    12665 2020-02-02 00:00:00.000000 custard-1.1.0/custard/rediscluster/tests/test_pipeline_cluster.py
+-rw-r--r--   0        0        0    21944 2020-02-02 00:00:00.000000 custard-1.1.0/custard/rediscluster/tests/test_pubsub.py
+-rw-r--r--   0        0        0     5375 2020-02-02 00:00:00.000000 custard-1.1.0/custard/rediscluster/tests/test_scripting.py
+-rw-r--r--   0        0        0     4899 2020-02-02 00:00:00.000000 custard-1.1.0/custard/rediscluster/tests/test_utils.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 custard-1.1.0/custard/script/__init__.py
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 custard-1.1.0/custard/script/compat.py
+-rw-r--r--   0        0        0    16449 2020-02-02 00:00:00.000000 custard-1.1.0/custard/script/parser.py
+-rw-r--r--   0        0        0     2589 2020-02-02 00:00:00.000000 custard-1.1.0/custard/script/schema.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 custard-1.1.0/custard/socket/__init__.py
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 custard-1.1.0/custard/swagger/__init__.py
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 custard-1.1.0/custard/swagger/exception.py
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 custard-1.1.0/custard/swagger/loader.py
+-rw-r--r--   0        0        0     6766 2020-02-02 00:00:00.000000 custard-1.1.0/custard/swagger/swagger.py
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 custard-1.1.0/custard/swagger/utils.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 custard-1.1.0/custard/system/__init__.py
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 custard-1.1.0/custard/time/__init__.py
+-rw-r--r--   0        0        0     6215 2020-02-02 00:00:00.000000 custard-1.1.0/custard/time/dafunc.py
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 custard-1.1.0/custard/time/exceptions.py
+-rw-r--r--   0        0        0     5964 2020-02-02 00:00:00.000000 custard-1.1.0/custard/time/moment.py
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 custard-1.1.0/custard/time/stoppable_thread.py
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 custard-1.1.0/custard/utils/__init__.py
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 custard-1.1.0/custard/utils/datasets.py
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 custard-1.1.0/custard/utils/decorators.py
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 custard-1.1.0/custard/utils/text.py
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 custard-1.1.0/examples/async_lur.py
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 custard-1.1.0/examples/crypto.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 custard-1.1.0/examples/datum.py
+-rw-r--r--   0        0        0     3650 2020-02-02 00:00:00.000000 custard-1.1.0/examples/decorator.py
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 custard-1.1.0/examples/dts.py
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 custard-1.1.0/examples/hitfilter.py
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 custard-1.1.0/examples/hitfilter_keyword
+-rw-r--r--   0        0        0     8968 2020-02-02 00:00:00.000000 custard-1.1.0/examples/json_logger.py
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 custard-1.1.0/examples/kaptcha.py
+-rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 custard-1.1.0/examples/kaptcha_execution_time.py
+-rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 custard-1.1.0/examples/limiter.py
+-rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 custard-1.1.0/examples/mock.py
+-rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 custard-1.1.0/examples/pagination_async_sqlalchemy.py
+-rw-r--r--   0        0        0     2170 2020-02-02 00:00:00.000000 custard-1.1.0/examples/pagination_sqlalchemy.py
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 custard-1.1.0/examples/swagger_online_change.py
+-rw-r--r--   0        0        0     6431 2020-02-02 00:00:00.000000 custard-1.1.0/examples/swagger_usabletest.py
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 custard-1.1.0/examples/useragent.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 custard-1.1.0/.gitignore
+-rw-r--r--   0        0        0     6988 2020-02-02 00:00:00.000000 custard-1.1.0/README.md
+-rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 custard-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0    10068 2020-02-02 00:00:00.000000 custard-1.1.0/PKG-INFO
```

### Comparing `custard-1.0.9/.github/workflows/python-publish.yml` & `custard-1.1.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `custard-1.0.9/custard/cache/async_lru.py` & `custard-1.1.0/custard/cache/async_lru.py`

 * *Files identical despite different names*

### Comparing `custard-1.0.9/custard/cache/async_lur.md` & `custard-1.1.0/custard/cache/async_lur.md`

 * *Files identical despite different names*

### Comparing `custard-1.0.9/custard/cache/redis.py` & `custard-1.1.0/custard/cache/redis.py`

 * *Files identical despite different names*

### Comparing `custard-1.0.9/custard/core/__init__.py` & `custard-1.1.0/custard/core/__init__.py`

 * *Files identical despite different names*

### Comparing `custard-1.0.9/custard/core/decode.py` & `custard-1.1.0/custard/core/decode.py`

 * *Files identical despite different names*

### Comparing `custard-1.0.9/custard/core/factory.py` & `custard-1.1.0/custard/core/factory.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,35 +20,37 @@
 import pypinyin
 from faker import Faker
 from requests.exceptions import InvalidURL
 from urllib3.exceptions import LocationParseError
 from urllib3.util import parse_url
 from custard.time.moment import Moment
 
-fake = Faker(['zh_CN'])
+fake = Faker(["zh_CN"])
 
 
 class MockHelper:
     @staticmethod
-    def hans2pinyin(hans, style='A'):
+    def hans2pinyin(hans, style="A"):
         """
         汉字转拼音
         Args:
             hans: 汉字
             style: 返回首字母还是全拼， A：全拼； F：首字母
         Returns:
         Examples:
             >>> print(MockHelper.hans2pinyin("啊哈哈哈"))
             >>> print(MockHelper.hans2pinyin("啊哈哈哈", "F"))
         """
 
-        if style.upper() == 'F':
-            return ''.join(pypinyin.lazy_pinyin(hans=hans, style=pypinyin.Style.FIRST_LETTER))
+        if style.upper() == "F":
+            return "".join(
+                pypinyin.lazy_pinyin(hans=hans, style=pypinyin.Style.FIRST_LETTER)
+            )
         else:
-            return ''.join(pypinyin.lazy_pinyin(hans=hans))
+            return "".join(pypinyin.lazy_pinyin(hans=hans))
 
     @staticmethod
     def rand_mail(email_type=None, max_num=None, rad_count=None):
         """
         Args:
             email_type: 邮箱类型
             max_num: 邮箱地址最大长度
@@ -65,16 +67,15 @@
             "@163.com",
             "@sina.com",
             "@sohu.com",
             "@yahoo.com.cn",
             "@gmail.com",
             "@yahoo.com",
         ]
-        email_type_ = random.choice(
-            email_array) if email_type is None else email_type
+        email_type_ = random.choice(email_array) if email_type is None else email_type
         max_num_ = random.randint(5, 10) if max_num is None else max_num
         rad_count_ = 1 if rad_count is None else rad_count
         while count < rad_count_:
             for i in range(0, max_num_):
                 status = random.randint(0, 1)
                 if status == 0:
                     temp.append(random.choice(string.ascii_letters))
@@ -126,43 +127,47 @@
         生成给定长度的字符串，返回列表格式
         Args:
             length:
         Returns:
         Examples:
             >>> MockHelper.rand_str_list(length=5)
         """
-        init_chars = "".join(
-            "".join(map(str, [i for i in range(10) if i != 4])))  # 数字
+        init_chars = "".join("".join(map(str, [i for i in range(10) if i != 4])))  # 数字
         sample_list = random.sample(init_chars, length)
         return sample_list
 
     @staticmethod
     def rand_str(num_length):
         """
         从a-za-z0-9生成指定数量的随机字符
         Args:
             num_length:
         Returns:
         Examples:
             >>> MockHelper.rand_str(6)
         """
-        return [random.choice(string.digits + string.ascii_letters) for i in range(num_length)]
+        return [
+            random.choice(string.digits + string.ascii_letters)
+            for i in range(num_length)
+        ]
 
     @staticmethod
     def rand_mum(num_length):
         """
         9生成指定数量的随机数字
         Args:
             num_length:
         Returns:
         """
         return "".join([random.choice(string.digits) for i in range(num_length)])
 
     @staticmethod
-    def rand_int_number(min_value: int = 0, max_value: int = 9999, step: int = 1) -> int:
+    def rand_int_number(
+        min_value: int = 0, max_value: int = 9999, step: int = 1
+    ) -> int:
         """
         随机生成整数
         Args:
             min_value:
             max_value:
             step:
         Returns:
@@ -193,22 +198,22 @@
             num = random.uniform(start_num, end_num)
         else:
             num = random.uniform(end_num, start_num)
         return round(num, accuracy)
 
     @staticmethod
     def rand_compute_time(
-            days=0,
-            seconds=0,
-            microseconds=0,
-            milliseconds=0,
-            minutes=0,
-            hours=0,
-            weeks=0,
-            custom=None,
+        days=0,
+        seconds=0,
+        microseconds=0,
+        milliseconds=0,
+        minutes=0,
+        hours=0,
+        weeks=0,
+        custom=None,
     ):
         """
         随机生成偏移时间
         Args:
             days:
             seconds:
             microseconds:
@@ -272,15 +277,17 @@
 
         Returns:
 
         Examples:
             >>> MockHelper.rand_sample(10)
 
         """
-        return "".join([random.choice(string.ascii_letters + string.digits) for i in range(length)])
+        return "".join(
+            [random.choice(string.ascii_letters + string.digits) for i in range(length)]
+        )
 
     @staticmethod
     def rand_mobile_number(length: int):
         """
         随机生成手机号
         Returns:
         Examples:
@@ -314,17 +321,16 @@
             145,
             133,
             153,
             180,
             181,
             189,
         ]
-        rand_phone_prefix = phone_prefixes[random.randint(
-            0, len(phone_prefixes))]
-        return [f'{rand_phone_prefix}{MockHelper.rand_mum(8)}' for i in range(length)]
+        rand_phone_prefix = phone_prefixes[random.randint(0, len(phone_prefixes))]
+        return [f"{rand_phone_prefix}{MockHelper.rand_mum(8)}" for i in range(length)]
 
     @staticmethod
     def rand_name():
         """
         随机生成名字
         Returns:
         Examples:
@@ -470,15 +476,15 @@
         Examples:
             >>> MockHelper.rand_job()
         """
         return fake.job()
 
     @staticmethod
     def rand_pwd(
-            length=10, special_chars=True, digits=True, upper_case=True, lower_case=True
+        length=10, special_chars=True, digits=True, upper_case=True, lower_case=True
     ):
         """
         随机生成密码
         lower_case:
         upper_case:
         digits:
         special_chars:
@@ -668,16 +674,15 @@
             >>> MockHelper.cite('$enc_(base64_encode,base64参数加密)')
         """
         # fix: file "d:\program files\python37\lib\re.py", line 173, in match
         # return _compile(pattern, flags).match(string)
         # typeerror: expected string or bytes-like object
         rand_vars = re.match("\\$\\{rand_(.*)\\((.*)\\)\\}", str(name))  # 带参数
         rand_no_vars = re.match("\\$\\{rand_(.*)\\}", str(name))  # 无参数
-        dynamic_vars = re.match(
-            "\\$\\{get(.*)\\((.*)\\)\\}", str(name))  # 动态自定义
+        dynamic_vars = re.match("\\$\\{get(.*)\\((.*)\\)\\}", str(name))  # 动态自定义
         own_vars = re.match("\\{\\{(.*)\\}\\}", str(name))  # 动态自定义
         extract_vars = re.match("\\$var_(.*)", str(name).upper())  # 后置提取参数
         lock_vars = re.match("\\$enc_(.*)", str(name))  # 带参数
         pattern = rand_vars if rand_vars is not None else dynamic_vars
         func_dict = {
             "int_number": MockHelper.rand_int_number,
             "float_number": MockHelper.rand_float_number,
@@ -721,15 +726,17 @@
                     eval(x) if x.strip().isdigit() else x for x in value.split(",")
                 ]
                 if len(_param) >= 1 and "" not in _param:
                     return func.__call__(*_param)
                 elif "" in _param:
                     return func.__call__()  # 没有带参数的
         elif own_vars:
-            return MockHelper.cite(MockHelper.get_user_vars(own_vars.group().strip("{}")))
+            return MockHelper.cite(
+                MockHelper.get_user_vars(own_vars.group().strip("{}"))
+            )
         elif extract_vars:
             return MockHelper.get_encrypt_vars(extract_vars.group())
         elif rand_no_vars:
             return func_dict[rand_no_vars.group().strip("${rand_}")].__call__()
         elif lock_vars:
             _lock_param = [
                 eval(x) if x.strip().isdigit() else x
@@ -757,32 +764,32 @@
             >>> MockHelper.comb_data({"key1":"$enc_(base64,base64参数加密)"})
         """
         if isinstance(dict_map, dict):
             for key in list(dict_map.keys()):
                 if isinstance(dict_map[key], list):
                     for i in range(len(dict_map[key])):
                         dict_map[key][i] = MockHelper.comb_data(
-                            dict_map=dict_map[key][i])
+                            dict_map=dict_map[key][i]
+                        )
                 elif isinstance(dict_map[key], dict):
-                    dict_map[key] = MockHelper.comb_data(
-                        dict_map=dict_map[key])
+                    dict_map[key] = MockHelper.comb_data(dict_map=dict_map[key])
                 else:
                     dict_map[key] = MockHelper.cite(dict_map[key])
             return dict_map
         elif dict_map is None:  # fix：为空的时候raise 异常导致其它函数调用失败
             pass
 
 
 class AutoVivification(dict):
-  def __getitem__(self, item):
-    try:
-      return dict.__getitem__(self, item)
-    except KeyError:
-      value = self[item] = type(self)()
-    return value
+    def __getitem__(self, item):
+        try:
+            return dict.__getitem__(self, item)
+        except KeyError:
+            value = self[item] = type(self)()
+        return value
 
 
 class MsHelper(object):
     GLOBAL_PAGE_INDEX = ["page_index" "pageindex"]
     GLOBAL_PAGE_SIZE = ["page_size" "pagesize"]
 
     @classmethod
@@ -872,15 +879,15 @@
         """
         try:
             scheme, auth, host, port, path, query, fragment = parse_url(url)
         except LocationParseError as e:
             raise InvalidURL(*e.args)
         output = {}
         if query:
-            query_split = query.split('&')
+            query_split = query.split("&")
             start = 0
             end = len(query_split) - 1
             while start <= end:
                 spl_data = [query_split[start], query_split[end]]
                 output = dict(output, **cls.sub_kv(spl_data))
                 start += 1
                 end -= 1
@@ -906,15 +913,15 @@
         output = ""
         data = cls.obj_convert_dict(obj)
         for key, value in data.items():
             if isinstance(value, (list, dict)):
                 raise TypeError("请核对参数及Content-Type是否规范")
             if isinstance(value, str):
                 value = quote(value, "unicode")
-            output += f'&{key}={value}'
+            output += f"&{key}={value}"
         return output
 
     @classmethod
     def json2vars(cls, target_data, source_data="", replace=True):
         """
         json转为vars
         Args:
@@ -939,77 +946,20 @@
                             value = 1
                         elif key in cls.GLOBAL_PAGE_SIZE:
                             value = 10
                         if key not in paging:
                             value = cls.__property__(value)
                     source_data += f'vars.put("{key}","{value}");\n'
                 else:
-                  source_data = cls.json2vars(target_data=value, source_data=source_data,
-                                              replace=replace)
+                    source_data = cls.json2vars(
+                        target_data=value, source_data=source_data, replace=replace
+                    )
         elif isinstance(target_data, list):
             for index in range(len(target_data)):
                 target_data_ = target_data[index]
                 # 启用该行数据不会去重，有多少条就产生多少
                 # source_data = cls.json2vars(target_data=target_data_, source_data=source_data, replace=replace)
                 # 以下方式会去重
-                return cls.json2vars(target_data=target_data_, source_data=source_data,
-                                     replace=replace)
+                return cls.json2vars(
+                    target_data=target_data_, source_data=source_data, replace=replace
+                )
         return source_data
-
-    @classmethod
-    def change_value(cls, key, oneself):
-        """
-        Args:
-            key:
-            oneself:
-        Returns:
-        Examples:
-            >>> single_dict = {"code": "200", "error": "", "message": "", "data": []}
-            >>> single_mixture = {"code": 200, "details": [{"a1": True, "a2": True}], "total_count": {"c1": 1, "c2": 5}}
-            >>> double_mixture = {"code": 200, "details": [{"a1": True, "a2": True}, {"b1": True, "b2": True}], "total_count": {"c1": 1, "c2": 5}}
-            >>> sd_ov = MsHelper.ov_init(single_dict)
-            >>> sm_ov = MsHelper.ov_init(single_mixture)
-            >>> dm_ov = MsHelper.ov_init(double_mixture)
-            >>> oneself_ov = MsHelper.ov_init(double_mixture, oneself=True)
-        """
-        return f'${{{key}}}' if oneself else ""
-
-    @classmethod
-    def ov_init(cls, target_data, source_data: dict = {}, pater_is_list=False, oneself=False, change_type=json):
-      """
-        将json中所有value初始化为""或者${oneself}
-        Args:
-            target_data:
-            source_data:
-            pater_is_list:
-            oneself:
-            change_type:
-        Returns:
-        Examples:
-            >>> target_data = { "code": 200, "details":[{"b1":True,"b2":True}], "total_count": {"d1":1,"d2":5}}
-            >>> ov_data = MsHelper.ov_init(target_data)
-            >>> print(json.dumps(ov_data))
-        """
-      if isinstance(target_data, dict):
-        data_ = cls.obj_convert_dict(target_data)
-        for key, value in data_.items():
-          if not isinstance(value, (list, dict)):
-              source_data.update({key: cls.change_value(key, oneself)})
-          else:
-            cls.ov_init(target_data=(key, value), source_data=source_data,
-                        oneself=oneself, change_type=change_type)
-      elif isinstance(target_data, tuple):
-        pater_key, pater_value = target_data
-        if isinstance(pater_value, dict):
-          if pater_is_list:
-            temp = [{key: cls.change_value(key, oneself)} for key, value in pater_value.items()]
-            source_data.update({pater_key: temp})
-          else:
-            item = defaultdict(dict)
-            for key, value in pater_value.items():
-              item[pater_key][key] = cls.change_value(key, oneself)
-            source_data.update(item)
-        elif isinstance(pater_value, list) and len(pater_value) > 0:
-            return cls.ov_init(target_data=(pater_key, pater_value[0]), source_data=source_data, pater_is_list=True, oneself=oneself, change_type=change_type)
-        elif isinstance(pater_value, list) and pater_value == []:
-          source_data.update({pater_key: pater_value})
-      return source_data if change_type is dict else json.dumps(source_data)
```

### Comparing `custard-1.0.9/custard/core/kerberos.py` & `custard-1.1.0/custard/core/kerberos.py`

 * *Files identical despite different names*

### Comparing `custard-1.0.9/custard/core/processor.py` & `custard-1.1.0/custard/core/processor.py`

 * *Files identical despite different names*

### Comparing `custard-1.0.9/custard/core/regular.py` & `custard-1.1.0/custard/core/regular.py`

 * *Files identical despite different names*

### Comparing `custard-1.0.9/custard/core/snowflake.py` & `custard-1.1.0/custard/core/snowflake.py`

 * *Files identical despite different names*

### Comparing `custard-1.0.9/custard/core/system.py` & `custard-1.1.0/custard/core/system.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,21 +6,22 @@
 @Author  :  YuYanQing
 @Version :  1.0
 @Contact :  mryu168@163.com
 @License :  (C)Copyright 2022-2026
 @Desc    :  None
 """
 import csv
+import custard
 import json
 import os
 import platform
 
 import yaml
 
-from .processor import DataHand
+from custard.core.processor import DataHand
 
 
 class System:
     @staticmethod
     def get_depend_libs(file_path):
         """
         获取第三方依赖架包
@@ -131,7 +132,25 @@
             elif load_mode == "csv":
                 csv_content_list = []
                 with open(file_path, encoding="utf-8") as csvfile:
                     reader = csv.DictReader(csvfile)
                     for row in reader:
                         csv_content_list.append(row)
                 return csv_content_list
+
+    @classmethod
+    def walk(cls, root_dir: str):
+        """
+        检索根目录，得到所有的子文件夹或子文件名
+        Args:
+            root_dir (str): _description_
+        Examples:
+            >>> root_dir = "../../custard"
+            >>> System.walk(root_dir)
+        """
+        result = []
+        dirs = [os.path.join(root_dir, index) for index in os.listdir(root_dir)]
+        for index in dirs:
+            for root, dirs, files in os.walk(index, topdown=False):
+                file_path = [os.path.join(root, file) for file in files]
+                result += file_path
+        return result
```

### Comparing `custard-1.0.9/custard/core/useragent.py` & `custard-1.1.0/custard/core/useragent.py`

 * *Files identical despite different names*

### Comparing `custard-1.0.9/custard/core/xml2dict.py` & `custard-1.1.0/custard/core/xml2dict.py`

 * *Files identical despite different names*

### Comparing `custard-1.0.9/custard/core/xprint.py` & `custard-1.1.0/custard/core/xprint.py`

 * *Files identical despite different names*

### Comparing `custard-1.0.9/custard/cron/batch_task.py` & `custard-1.1.0/custard/cron/batch_task.py`

 * *Files identical despite different names*

### Comparing `custard-1.0.9/custard/crypto/crypto.py` & `custard-1.1.0/custard/crypto/crypto.py`

 * *Files identical despite different names*

### Comparing `custard-1.0.9/custard/crypto/streambody.py` & `custard-1.1.0/custard/crypto/streambody.py`

 * *Files identical despite different names*

### Comparing `custard-1.0.9/custard/db/inspect.py` & `custard-1.1.0/custard/db/inspect.py`

 * *Files identical despite different names*

### Comparing `custard-1.0.9/custard/db/logger.py` & `custard-1.1.0/custard/db/logger.py`

 * *Files identical despite different names*

### Comparing `custard-1.0.9/custard/db/utils.py` & `custard-1.1.0/custard/db/utils.py`

 * *Files identical despite different names*

### Comparing `custard-1.0.9/custard/expect/context.py` & `custard-1.1.0/custard/expect/context.py`

 * *Files identical despite different names*

### Comparing `custard-1.0.9/custard/expect/exceptions.py` & `custard-1.1.0/custard/expect/exceptions.py`

 * *Files identical despite different names*

### Comparing `custard-1.0.9/custard/expect/record.py` & `custard-1.1.0/custard/expect/record.py`

 * *Files identical despite different names*

### Comparing `custard-1.0.9/custard/expect/spacer.py` & `custard-1.1.0/custard/expect/spacer.py`

 * *Files identical despite different names*

### Comparing `custard-1.0.9/custard/function/callsource.py` & `custard-1.1.0/custard/function/callsource.py`

 * *Files identical despite different names*

### Comparing `custard-1.0.9/custard/function/traverse.py` & `custard-1.1.0/custard/function/traverse.py`

 * *Files identical despite different names*

### Comparing `custard-1.0.9/custard/hitfilter/hitfilter.py` & `custard-1.1.0/custard/hitfilter/hitfilter.py`

 * *Files identical despite different names*

### Comparing `custard-1.0.9/custard/hitfilter/keywords` & `custard-1.1.0/custard/hitfilter/keywords`

 * *Files identical despite different names*

### Comparing `custard-1.0.9/custard/json/jsonlogger.py` & `custard-1.1.0/custard/json/jsonlogger.py`

 * *Files identical despite different names*

### Comparing `custard-1.0.9/custard/kaptcha/captcha.py` & `custard-1.1.0/custard/kaptcha/captcha.py`

 * *Files identical despite different names*

### Comparing `custard-1.0.9/custard/kaptcha/font1.ttf` & `custard-1.1.0/custard/kaptcha/font1.ttf`

 * *Files identical despite different names*

### Comparing `custard-1.0.9/custard/kaptcha/font2.ttf` & `custard-1.1.0/custard/kaptcha/font2.ttf`

 * *Files identical despite different names*

### Comparing `custard-1.0.9/custard/kaptcha/font3.ttf` & `custard-1.1.0/custard/kaptcha/font3.ttf`

 * *Files identical despite different names*

### Comparing `custard-1.0.9/custard/kaptcha/font4.ttf` & `custard-1.1.0/custard/kaptcha/font4.ttf`

 * *Files identical despite different names*

### Comparing `custard-1.0.9/custard/limiter/__init__.py` & `custard-1.1.0/custard/limiter/__init__.py`

 * *Files identical despite different names*

### Comparing `custard-1.0.9/custard/limiter/depends.py` & `custard-1.1.0/custard/limiter/depends.py`

 * *Files identical despite different names*

### Comparing `custard-1.0.9/custard/lock/redis_lock.py` & `custard-1.1.0/custard/lock/redis_lock.py`

 * *Files identical despite different names*

### Comparing `custard-1.0.9/custard/lock/thread_lock.py` & `custard-1.1.0/custard/lock/thread_lock.py`

 * *Files identical despite different names*

### Comparing `custard-1.0.9/custard/lodash/README.md` & `custard-1.1.0/custard/lodash/README.md`

 * *Files identical despite different names*

### Comparing `custard-1.0.9/custard/lodash/__init__.py` & `custard-1.1.0/custard/lodash/__init__.py`

 * *Files identical despite different names*

### Comparing `custard-1.0.9/custard/lodash/arrays.py` & `custard-1.1.0/custard/lodash/arrays.py`

 * *Files identical despite different names*

### Comparing `custard-1.0.9/custard/lodash/maths.py` & `custard-1.1.0/custard/lodash/maths.py`

 * *Files identical despite different names*

### Comparing `custard-1.0.9/custard/lodash/number.py` & `custard-1.1.0/custard/lodash/number.py`

 * *Files identical despite different names*

### Comparing `custard-1.0.9/custard/lodash/string.py` & `custard-1.1.0/custard/lodash/string.py`

 * *Files identical despite different names*

### Comparing `custard-1.0.9/custard/lodash/utilities.py` & `custard-1.1.0/custard/lodash/utilities.py`

 * *Files identical despite different names*

### Comparing `custard-1.0.9/custard/mock/__init__.py` & `custard-1.1.0/custard/mock/__init__.py`

 * *Files identical despite different names*

### Comparing `custard-1.0.9/custard/mock/mini_racer.py` & `custard-1.1.0/custard/mock/mini_racer.py`

 * *Files identical despite different names*

### Comparing `custard-1.0.9/custard/mock/mock.min.js` & `custard-1.1.0/custard/mock/mock.min.js`

 * *Files identical despite different names*

### Comparing `custard-1.0.9/custard/mock/mock.old.min.js` & `custard-1.1.0/custard/mock/mock.old.min.js`

 * *Files identical despite different names*

### Comparing `custard-1.0.9/custard/network/httpclient.py` & `custard-1.1.0/custard/network/httpclient.py`

 * *Files identical despite different names*

### Comparing `custard-1.0.9/custard/pagination/__init__.py` & `custard-1.1.0/custard/pagination/__init__.py`

 * *Files identical despite different names*

### Comparing `custard-1.0.9/custard/pagination/api.py` & `custard-1.1.0/custard/pagination/api.py`

 * *Files identical despite different names*

### Comparing `custard-1.0.9/custard/pagination/async_sqlalchemy.py` & `custard-1.1.0/custard/pagination/async_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `custard-1.0.9/custard/pagination/bases.py` & `custard-1.1.0/custard/pagination/bases.py`

 * *Files identical despite different names*

### Comparing `custard-1.0.9/custard/pagination/default.py` & `custard-1.1.0/custard/pagination/default.py`

 * *Files identical despite different names*

### Comparing `custard-1.0.9/custard/pagination/iterables.py` & `custard-1.1.0/custard/pagination/iterables.py`

 * *Files identical despite different names*

### Comparing `custard-1.0.9/custard/pagination/limit_offset.py` & `custard-1.1.0/custard/pagination/limit_offset.py`

 * *Files identical despite different names*

### Comparing `custard-1.0.9/custard/pagination/pagination.py` & `custard-1.1.0/custard/pagination/pagination.py`

 * *Files identical despite different names*

### Comparing `custard-1.0.9/custard/pagination/paginator.py` & `custard-1.1.0/custard/pagination/paginator.py`

 * *Files identical despite different names*

### Comparing `custard-1.0.9/custard/pagination/sync_sqlalchemy.py` & `custard-1.1.0/custard/pagination/sync_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `custard-1.0.9/custard/script/compat.py` & `custard-1.1.0/custard/script/compat.py`

 * *Files identical despite different names*

### Comparing `custard-1.0.9/custard/script/parser.py` & `custard-1.1.0/custard/script/parser.py`

 * *Files identical despite different names*

### Comparing `custard-1.0.9/custard/script/schema.py` & `custard-1.1.0/custard/script/schema.py`

 * *Files identical despite different names*

### Comparing `custard-1.0.9/custard/swagger/__init__.py` & `custard-1.1.0/custard/swagger/__init__.py`

 * *Files identical despite different names*

### Comparing `custard-1.0.9/custard/swagger/loader.py` & `custard-1.1.0/custard/swagger/loader.py`

 * *Files identical despite different names*

### Comparing `custard-1.0.9/custard/swagger/swagger.py` & `custard-1.1.0/custard/swagger/swagger.py`

 * *Files identical despite different names*

### Comparing `custard-1.0.9/custard/swagger/utils.py` & `custard-1.1.0/custard/swagger/utils.py`

 * *Files identical despite different names*

### Comparing `custard-1.0.9/custard/time/dafunc.py` & `custard-1.1.0/custard/time/dafunc.py`

 * *Files identical despite different names*

### Comparing `custard-1.0.9/custard/time/exceptions.py` & `custard-1.1.0/custard/time/exceptions.py`

 * *Files identical despite different names*

### Comparing `custard-1.0.9/custard/time/moment.py` & `custard-1.1.0/custard/time/moment.py`

 * *Files identical despite different names*

### Comparing `custard-1.0.9/custard/time/stoppable_thread.py` & `custard-1.1.0/custard/time/stoppable_thread.py`

 * *Files identical despite different names*

### Comparing `custard-1.0.9/custard/utils/datasets.py` & `custard-1.1.0/custard/utils/datasets.py`

 * *Files identical despite different names*

### Comparing `custard-1.0.9/custard/utils/decorators.py` & `custard-1.1.0/custard/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `custard-1.0.9/custard/utils/text.py` & `custard-1.1.0/custard/utils/text.py`

 * *Files identical despite different names*

### Comparing `custard-1.0.9/examples/async_lur.py` & `custard-1.1.0/examples/async_lur.py`

 * *Files identical despite different names*

### Comparing `custard-1.0.9/examples/decorator.py` & `custard-1.1.0/examples/decorator.py`

 * *Files identical despite different names*

### Comparing `custard-1.0.9/examples/dts.py` & `custard-1.1.0/examples/dts.py`

 * *Files identical despite different names*

### Comparing `custard-1.0.9/examples/hitfilter.py` & `custard-1.1.0/examples/hitfilter.py`

 * *Files identical despite different names*

### Comparing `custard-1.0.9/examples/json_logger.py` & `custard-1.1.0/examples/json_logger.py`

 * *Files identical despite different names*

### Comparing `custard-1.0.9/examples/kaptcha.py` & `custard-1.1.0/examples/kaptcha.py`

 * *Files identical despite different names*

### Comparing `custard-1.0.9/examples/kaptcha_execution_time.py` & `custard-1.1.0/examples/kaptcha_execution_time.py`

 * *Files identical despite different names*

### Comparing `custard-1.0.9/examples/limiter.py` & `custard-1.1.0/examples/limiter.py`

 * *Files identical despite different names*

### Comparing `custard-1.0.9/examples/mock.py` & `custard-1.1.0/examples/mock.py`

 * *Files identical despite different names*

### Comparing `custard-1.0.9/examples/pagination_async_sqlalchemy.py` & `custard-1.1.0/examples/pagination_async_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `custard-1.0.9/examples/pagination_sqlalchemy.py` & `custard-1.1.0/examples/pagination_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `custard-1.0.9/examples/swagger_usabletest.py` & `custard-1.1.0/examples/swagger_usabletest.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         # 准备测试资源
         if not os.path.exists(cls.default_file):
             with open(cls.default_file, mode='w') as f:
                 f.write('Hello world!')
         if not os.path.exists(cls.result_path):
           os.makedirs(cls.result_path)
         cls.run_host = run_host
-        cls.swagger_host = "https://localhost:7777"
+        cls.swagger_host = "https://awen.uat.rvet.cn"
         cls.swagger_path = "/swagger/doc.json"
         cls.service_list = ["order-api", "product-api", "customer-api", "pay_echo", "mall", "personalized-api", "boss"]
 
     @classmethod
     def tearDownClass(cls):
         # 清理测试资源
         if os.path.exists(cls.default_file):
@@ -65,15 +65,15 @@
         else:
           with open(file_name, "w", encoding="utf-8") as file:
               table_title = f"# {service}{alias}\n"
               table_header = f"|url|method|status_code|headers|params|json|response_text|\n"
               table_style = f"|:------:|:------:|:------:|:------:|:------:|:------:|:------:|\n"
               file.write(f"{table_title}{table_header}{table_style}")
         return file_name, swagger_data
-          
+
     @classmethod
     def thread_scan_api(cls, request, file_name, semaphore):
         """
         给主进程加锁
         Args:
             request: 请求数据
             file_name: 文件名
@@ -129,15 +129,15 @@
                   start = res_text[:curtail_length]
                   omit_length = len(res_text) - (curtail_length)
                   result = f'{global_res_data}`{start}....此处省略{omit_length}个字节.....`|\n'
                 else:
                   result = f'{global_res_data}`{res_text}`|\n'
               file.write(result)
         semaphore.release()  # 释放
-        
+
     def test_run(self):
       for service in self.service_list:  # 事件数
         file_name, swagger_data = self.init_env(service)
         requests_ = swagger_data.apis
         max_thread_ = lambda x: x if x<2000 else 2000
         thread_num = max_thread_(len(requests_))
         print(f"{service} total number of service apis: {len(requests_)}, thread_num: {thread_num}")
```

### Comparing `custard-1.0.9/examples/useragent.py` & `custard-1.1.0/examples/useragent.py`

 * *Files identical despite different names*

### Comparing `custard-1.0.9/README.md` & `custard-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `custard-1.0.9/pyproject.toml` & `custard-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,16 @@
     "lxml>=4.9.0",
     "redis>=3.5.3",
     "mkdocs>=1.3.0",
     "certifi<=2021.10.8",
     "dicttoxml>=1.7.4",
     "crypto~=1.4.1",
     "PyYAML~=6.0",
-    "urllib3~=1.26.12"
+    "urllib3~=1.26.12",
+    "w3lib~=2.1.1"
 ]
 
 [tool.hatch.version]
 path = "custard/__init__.py"
 
 [tool.isort]
 profile = "black"
```

### Comparing `custard-1.0.9/PKG-INFO` & `custard-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: custard
-Version: 1.0.9
+Version: 1.1.0
 Summary: custard easy to learn, fast to code, ready for production
 Project-URL: Homepage, https://github.com/kamalyes/custard
 Author-email: Kamalyes <mryu168@163.com>
 License-Expression: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
@@ -42,14 +42,15 @@
 Requires-Dist: redis>=3.5.3; extra == 'all'
 Requires-Dist: requests~=2.27.0; extra == 'all'
 Requires-Dist: six>=1.16.0; extra == 'all'
 Requires-Dist: sqlalchemy>=1.4.37; extra == 'all'
 Requires-Dist: starlette>=0.19.1; extra == 'all'
 Requires-Dist: urllib3~=1.26.12; extra == 'all'
 Requires-Dist: uvicorn>=0.17.6; extra == 'all'
+Requires-Dist: w3lib~=2.1.1; extra == 'all'
 Provides-Extra: dev
 Requires-Dist: pre-commit<3.0.0,>=2.17.0; extra == 'dev'
 Requires-Dist: ruff==0.0.138; extra == 'dev'
 Requires-Dist: uvicorn[standard]<0.19.0,>=0.12.0; extra == 'dev'
 Provides-Extra: doc
 Requires-Dist: mdx-include<2.0.0,>=1.4.1; extra == 'doc'
 Requires-Dist: mkdocs-markdownextradata-plugin<0.3.0,>=0.1.7; extra == 'doc'
```

