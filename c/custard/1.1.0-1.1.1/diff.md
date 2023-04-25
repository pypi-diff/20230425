# Comparing `tmp/custard-1.1.0.tar.gz` & `tmp/custard-1.1.1.tar.gz`

## Comparing `custard-1.1.0.tar` & `custard-1.1.1.tar`

### file list

```diff
@@ -1,174 +1,174 @@
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 custard-1.1.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 custard-1.1.0/.vscode/launch.json
--rw-r--r--   0        0        0     3993 2020-02-02 00:00:00.000000 custard-1.1.0/.vscode/settings.json
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 custard-1.1.0/custard/__init__.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 custard-1.1.0/custard/cache/__init__.py
--rw-r--r--   0        0        0     4936 2020-02-02 00:00:00.000000 custard-1.1.0/custard/cache/async_lru.py
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 custard-1.1.0/custard/cache/async_lur.md
--rw-r--r--   0        0        0    11971 2020-02-02 00:00:00.000000 custard-1.1.0/custard/cache/redis.py
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 custard-1.1.0/custard/core/__init__.py
--rw-r--r--   0        0        0   770279 2020-02-02 00:00:00.000000 custard-1.1.0/custard/core/decode.py
--rw-r--r--   0        0        0    28578 2020-02-02 00:00:00.000000 custard-1.1.0/custard/core/factory.py
--rw-r--r--   0        0        0     2978 2020-02-02 00:00:00.000000 custard-1.1.0/custard/core/kerberos.py
--rw-r--r--   0        0        0    30562 2020-02-02 00:00:00.000000 custard-1.1.0/custard/core/processor.py
--rw-r--r--   0        0        0    23875 2020-02-02 00:00:00.000000 custard-1.1.0/custard/core/regular.py
--rw-r--r--   0        0        0     1959 2020-02-02 00:00:00.000000 custard-1.1.0/custard/core/snowflake.py
--rw-r--r--   0        0        0     5196 2020-02-02 00:00:00.000000 custard-1.1.0/custard/core/system.py
--rw-r--r--   0        0        0    22331 2020-02-02 00:00:00.000000 custard-1.1.0/custard/core/useragent.py
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 custard-1.1.0/custard/core/xml2dict.py
--rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 custard-1.1.0/custard/core/xprint.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 custard-1.1.0/custard/cron/__init__.py
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 custard-1.1.0/custard/cron/batch_task.py
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 custard-1.1.0/custard/crypto/__init__.py
--rw-r--r--   0        0        0    15727 2020-02-02 00:00:00.000000 custard-1.1.0/custard/crypto/crypto.py
--rw-r--r--   0        0        0     3226 2020-02-02 00:00:00.000000 custard-1.1.0/custard/crypto/streambody.py
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 custard-1.1.0/custard/curl/__init__.py
--rw-r--r--   0        0        0     5883 2020-02-02 00:00:00.000000 custard-1.1.0/custard/curl/parse.py
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 custard-1.1.0/custard/db/__init__.py
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 custard-1.1.0/custard/db/exc.py
--rw-r--r--   0        0        0     4810 2020-02-02 00:00:00.000000 custard-1.1.0/custard/db/inspect.py
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 custard-1.1.0/custard/db/logger.py
--rw-r--r--   0        0        0     4769 2020-02-02 00:00:00.000000 custard-1.1.0/custard/db/utils.py
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 custard-1.1.0/custard/expect/__init__.py
--rw-r--r--   0        0        0     1287 2020-02-02 00:00:00.000000 custard-1.1.0/custard/expect/context.py
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 custard-1.1.0/custard/expect/exceptions.py
--rw-r--r--   0        0        0     3424 2020-02-02 00:00:00.000000 custard-1.1.0/custard/expect/record.py
--rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 custard-1.1.0/custard/expect/spacer.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 custard-1.1.0/custard/extra/__init__.py
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 custard-1.1.0/custard/function/__init__.py
--rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 custard-1.1.0/custard/function/callsource.py
--rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 custard-1.1.0/custard/function/traverse.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 custard-1.1.0/custard/hitfilter/__init__.py
--rw-r--r--   0        0        0     2948 2020-02-02 00:00:00.000000 custard-1.1.0/custard/hitfilter/hitfilter.py
--rw-r--r--   0        0        0   761348 2020-02-02 00:00:00.000000 custard-1.1.0/custard/hitfilter/keywords
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 custard-1.1.0/custard/json/__init__.py
--rw-r--r--   0        0        0     9316 2020-02-02 00:00:00.000000 custard-1.1.0/custard/json/jsonlogger.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 custard-1.1.0/custard/kaptcha/__init__.py
--rw-r--r--   0        0        0     9495 2020-02-02 00:00:00.000000 custard-1.1.0/custard/kaptcha/captcha.py
--rw-r--r--   0        0        0   171508 2020-02-02 00:00:00.000000 custard-1.1.0/custard/kaptcha/font1.ttf
--rw-r--r--   0        0        0    42452 2020-02-02 00:00:00.000000 custard-1.1.0/custard/kaptcha/font2.ttf
--rw-r--r--   0        0        0    92956 2020-02-02 00:00:00.000000 custard-1.1.0/custard/kaptcha/font3.ttf
--rw-r--r--   0        0        0   314452 2020-02-02 00:00:00.000000 custard-1.1.0/custard/kaptcha/font4.ttf
--rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 custard-1.1.0/custard/limiter/__init__.py
--rw-r--r--   0        0        0     2106 2020-02-02 00:00:00.000000 custard-1.1.0/custard/limiter/depends.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 custard-1.1.0/custard/limiter/enums.py
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 custard-1.1.0/custard/limiter/execres.py
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 custard-1.1.0/custard/lock/__init__.py
--rw-r--r--   0        0        0     3070 2020-02-02 00:00:00.000000 custard-1.1.0/custard/lock/redis_lock.py
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 custard-1.1.0/custard/lock/thread_lock.py
--rw-r--r--   0        0        0    12051 2020-02-02 00:00:00.000000 custard-1.1.0/custard/lodash/README.md
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 custard-1.1.0/custard/lodash/__init__.py
--rw-r--r--   0        0        0     5417 2020-02-02 00:00:00.000000 custard-1.1.0/custard/lodash/arrays.py
--rw-r--r--   0        0        0     4307 2020-02-02 00:00:00.000000 custard-1.1.0/custard/lodash/maths.py
--rw-r--r--   0        0        0     3474 2020-02-02 00:00:00.000000 custard-1.1.0/custard/lodash/number.py
--rw-r--r--   0        0        0     7238 2020-02-02 00:00:00.000000 custard-1.1.0/custard/lodash/string.py
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 custard-1.1.0/custard/lodash/utilities.py
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 custard-1.1.0/custard/minioss/__init__.py
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 custard-1.1.0/custard/minioss/aliyun.py
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 custard-1.1.0/custard/minioss/enums.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 custard-1.1.0/custard/minioss/gitee.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 custard-1.1.0/custard/minioss/minio.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 custard-1.1.0/custard/minioss/qiniu.py
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 custard-1.1.0/custard/minioss/tencent.py
--rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 custard-1.1.0/custard/mock/__init__.py
--rw-r--r--   0        0        0    14510 2020-02-02 00:00:00.000000 custard-1.1.0/custard/mock/mini_racer.py
--rw-r--r--   0        0        0   366292 2020-02-02 00:00:00.000000 custard-1.1.0/custard/mock/mock.min.js
--rw-r--r--   0        0        0   292581 2020-02-02 00:00:00.000000 custard-1.1.0/custard/mock/mock.old.min.js
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 custard-1.1.0/custard/network/asynchttp.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 custard-1.1.0/custard/network/enums.py
--rw-r--r--   0        0        0     3426 2020-02-02 00:00:00.000000 custard-1.1.0/custard/network/httpclient.py
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 custard-1.1.0/custard/pagination/__init__.py
--rw-r--r--   0        0        0     4269 2020-02-02 00:00:00.000000 custard-1.1.0/custard/pagination/api.py
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 custard-1.1.0/custard/pagination/async_sqlalchemy.py
--rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 custard-1.1.0/custard/pagination/bases.py
--rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 custard-1.1.0/custard/pagination/default.py
--rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 custard-1.1.0/custard/pagination/iterables.py
--rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 custard-1.1.0/custard/pagination/limit_offset.py
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 custard-1.1.0/custard/pagination/pagination.py
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 custard-1.1.0/custard/pagination/paginator.py
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 custard-1.1.0/custard/pagination/sync_sqlalchemy.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 custard-1.1.0/custard/pio/__init__.py
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 custard-1.1.0/custard/rediscluster/__init__.py
--rw-r--r--   0        0        0    49431 2020-02-02 00:00:00.000000 custard-1.1.0/custard/rediscluster/client.py
--rw-r--r--   0        0        0    23993 2020-02-02 00:00:00.000000 custard-1.1.0/custard/rediscluster/connection.py
--rw-r--r--   0        0        0     2722 2020-02-02 00:00:00.000000 custard-1.1.0/custard/rediscluster/crc.py
--rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 custard-1.1.0/custard/rediscluster/exceptions.py
--rw-r--r--   0        0        0    17930 2020-02-02 00:00:00.000000 custard-1.1.0/custard/rediscluster/nodemanager.py
--rw-r--r--   0        0        0    19857 2020-02-02 00:00:00.000000 custard-1.1.0/custard/rediscluster/pipeline.py
--rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 custard-1.1.0/custard/rediscluster/pubsub.py
--rw-r--r--   0        0        0     6161 2020-02-02 00:00:00.000000 custard-1.1.0/custard/rediscluster/utils.py
--rw-r--r--   0        0        0     3730 2020-02-02 00:00:00.000000 custard-1.1.0/custard/rediscluster/benchmarks/simple.py
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 custard-1.1.0/custard/rediscluster/docs/authors.md
--rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 custard-1.1.0/custard/rediscluster/docs/benchmarks.md
--rw-r--r--   0        0        0     5039 2020-02-02 00:00:00.000000 custard-1.1.0/custard/rediscluster/docs/client.md
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 custard-1.1.0/custard/rediscluster/docs/logging.md
--rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 custard-1.1.0/custard/rediscluster/docs/readonly-mode.md
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 custard-1.1.0/custard/rediscluster/docs/scripting.md
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 custard-1.1.0/custard/rediscluster/examples/basic.py
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 custard-1.1.0/custard/rediscluster/examples/basic_elasticache_password_protected.py
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 custard-1.1.0/custard/rediscluster/examples/basic_password_protected.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 custard-1.1.0/custard/rediscluster/examples/from_url_password_protected.py
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 custard-1.1.0/custard/rediscluster/examples/generate_slot_keys.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 custard-1.1.0/custard/rediscluster/examples/incr-test-writer.py
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 custard-1.1.0/custard/rediscluster/examples/pipeline-incrby.py
--rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 custard-1.1.0/custard/rediscluster/examples/pipeline-readonly-replicas.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 custard-1.1.0/custard/rediscluster/tests/__init__.py
--rw-r--r--   0        0        0     8789 2020-02-02 00:00:00.000000 custard-1.1.0/custard/rediscluster/tests/conftest.py
--rw-r--r--   0        0        0    49667 2020-02-02 00:00:00.000000 custard-1.1.0/custard/rediscluster/tests/redis-trib.rb
--rw-r--r--   0        0        0    36527 2020-02-02 00:00:00.000000 custard-1.1.0/custard/rediscluster/tests/test_cluster_connection_pool.py
--rw-r--r--   0        0        0    21628 2020-02-02 00:00:00.000000 custard-1.1.0/custard/rediscluster/tests/test_cluster_node_manager.py
--rw-r--r--   0        0        0    20803 2020-02-02 00:00:00.000000 custard-1.1.0/custard/rediscluster/tests/test_cluster_obj.py
--rw-r--r--   0        0        0   103248 2020-02-02 00:00:00.000000 custard-1.1.0/custard/rediscluster/tests/test_commands.py
--rw-r--r--   0        0        0    17579 2020-02-02 00:00:00.000000 custard-1.1.0/custard/rediscluster/tests/test_commands_cluster.py
--rw-r--r--   0        0        0     4355 2020-02-02 00:00:00.000000 custard-1.1.0/custard/rediscluster/tests/test_encoding.py
--rw-r--r--   0        0        0     3155 2020-02-02 00:00:00.000000 custard-1.1.0/custard/rediscluster/tests/test_encoding_cluster.py
--rw-r--r--   0        0        0     8016 2020-02-02 00:00:00.000000 custard-1.1.0/custard/rediscluster/tests/test_lock.py
--rw-r--r--   0        0        0     2402 2020-02-02 00:00:00.000000 custard-1.1.0/custard/rediscluster/tests/test_monitor.py
--rw-r--r--   0        0        0     5774 2020-02-02 00:00:00.000000 custard-1.1.0/custard/rediscluster/tests/test_multiprocessing.py
--rw-r--r--   0        0        0     5386 2020-02-02 00:00:00.000000 custard-1.1.0/custard/rediscluster/tests/test_multiprocessing_cluster.py
--rw-r--r--   0        0        0    12150 2020-02-02 00:00:00.000000 custard-1.1.0/custard/rediscluster/tests/test_pipeline.py
--rw-r--r--   0        0        0    12665 2020-02-02 00:00:00.000000 custard-1.1.0/custard/rediscluster/tests/test_pipeline_cluster.py
--rw-r--r--   0        0        0    21944 2020-02-02 00:00:00.000000 custard-1.1.0/custard/rediscluster/tests/test_pubsub.py
--rw-r--r--   0        0        0     5375 2020-02-02 00:00:00.000000 custard-1.1.0/custard/rediscluster/tests/test_scripting.py
--rw-r--r--   0        0        0     4899 2020-02-02 00:00:00.000000 custard-1.1.0/custard/rediscluster/tests/test_utils.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 custard-1.1.0/custard/script/__init__.py
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 custard-1.1.0/custard/script/compat.py
--rw-r--r--   0        0        0    16449 2020-02-02 00:00:00.000000 custard-1.1.0/custard/script/parser.py
--rw-r--r--   0        0        0     2589 2020-02-02 00:00:00.000000 custard-1.1.0/custard/script/schema.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 custard-1.1.0/custard/socket/__init__.py
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 custard-1.1.0/custard/swagger/__init__.py
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 custard-1.1.0/custard/swagger/exception.py
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 custard-1.1.0/custard/swagger/loader.py
--rw-r--r--   0        0        0     6766 2020-02-02 00:00:00.000000 custard-1.1.0/custard/swagger/swagger.py
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 custard-1.1.0/custard/swagger/utils.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 custard-1.1.0/custard/system/__init__.py
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 custard-1.1.0/custard/time/__init__.py
--rw-r--r--   0        0        0     6215 2020-02-02 00:00:00.000000 custard-1.1.0/custard/time/dafunc.py
--rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 custard-1.1.0/custard/time/exceptions.py
--rw-r--r--   0        0        0     5964 2020-02-02 00:00:00.000000 custard-1.1.0/custard/time/moment.py
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 custard-1.1.0/custard/time/stoppable_thread.py
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 custard-1.1.0/custard/utils/__init__.py
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 custard-1.1.0/custard/utils/datasets.py
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 custard-1.1.0/custard/utils/decorators.py
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 custard-1.1.0/custard/utils/text.py
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 custard-1.1.0/examples/async_lur.py
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 custard-1.1.0/examples/crypto.py
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 custard-1.1.0/examples/datum.py
--rw-r--r--   0        0        0     3650 2020-02-02 00:00:00.000000 custard-1.1.0/examples/decorator.py
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 custard-1.1.0/examples/dts.py
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 custard-1.1.0/examples/hitfilter.py
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 custard-1.1.0/examples/hitfilter_keyword
--rw-r--r--   0        0        0     8968 2020-02-02 00:00:00.000000 custard-1.1.0/examples/json_logger.py
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 custard-1.1.0/examples/kaptcha.py
--rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 custard-1.1.0/examples/kaptcha_execution_time.py
--rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 custard-1.1.0/examples/limiter.py
--rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 custard-1.1.0/examples/mock.py
--rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 custard-1.1.0/examples/pagination_async_sqlalchemy.py
--rw-r--r--   0        0        0     2170 2020-02-02 00:00:00.000000 custard-1.1.0/examples/pagination_sqlalchemy.py
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 custard-1.1.0/examples/swagger_online_change.py
--rw-r--r--   0        0        0     6431 2020-02-02 00:00:00.000000 custard-1.1.0/examples/swagger_usabletest.py
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 custard-1.1.0/examples/useragent.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 custard-1.1.0/.gitignore
--rw-r--r--   0        0        0     6988 2020-02-02 00:00:00.000000 custard-1.1.0/README.md
--rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 custard-1.1.0/pyproject.toml
--rw-r--r--   0        0        0    10068 2020-02-02 00:00:00.000000 custard-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 custard-1.1.1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 custard-1.1.1/.vscode/launch.json
+-rw-r--r--   0        0        0     3993 2020-02-02 00:00:00.000000 custard-1.1.1/.vscode/settings.json
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 custard-1.1.1/custard/__init__.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 custard-1.1.1/custard/cache/__init__.py
+-rw-r--r--   0        0        0     4936 2020-02-02 00:00:00.000000 custard-1.1.1/custard/cache/async_lru.py
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 custard-1.1.1/custard/cache/async_lur.md
+-rw-r--r--   0        0        0    11971 2020-02-02 00:00:00.000000 custard-1.1.1/custard/cache/redis.py
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 custard-1.1.1/custard/core/__init__.py
+-rw-r--r--   0        0        0   770279 2020-02-02 00:00:00.000000 custard-1.1.1/custard/core/decode.py
+-rw-r--r--   0        0        0    28578 2020-02-02 00:00:00.000000 custard-1.1.1/custard/core/factory.py
+-rw-r--r--   0        0        0     2978 2020-02-02 00:00:00.000000 custard-1.1.1/custard/core/kerberos.py
+-rw-r--r--   0        0        0    30562 2020-02-02 00:00:00.000000 custard-1.1.1/custard/core/processor.py
+-rw-r--r--   0        0        0    23875 2020-02-02 00:00:00.000000 custard-1.1.1/custard/core/regular.py
+-rw-r--r--   0        0        0     1959 2020-02-02 00:00:00.000000 custard-1.1.1/custard/core/snowflake.py
+-rw-r--r--   0        0        0     5196 2020-02-02 00:00:00.000000 custard-1.1.1/custard/core/system.py
+-rw-r--r--   0        0        0    22331 2020-02-02 00:00:00.000000 custard-1.1.1/custard/core/useragent.py
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 custard-1.1.1/custard/core/xml2dict.py
+-rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 custard-1.1.1/custard/core/xprint.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 custard-1.1.1/custard/cron/__init__.py
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 custard-1.1.1/custard/cron/batch_task.py
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 custard-1.1.1/custard/crypto/__init__.py
+-rw-r--r--   0        0        0    15727 2020-02-02 00:00:00.000000 custard-1.1.1/custard/crypto/crypto.py
+-rw-r--r--   0        0        0     3226 2020-02-02 00:00:00.000000 custard-1.1.1/custard/crypto/streambody.py
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 custard-1.1.1/custard/curl/__init__.py
+-rw-r--r--   0        0        0     5883 2020-02-02 00:00:00.000000 custard-1.1.1/custard/curl/parse.py
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 custard-1.1.1/custard/db/__init__.py
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 custard-1.1.1/custard/db/exc.py
+-rw-r--r--   0        0        0     4810 2020-02-02 00:00:00.000000 custard-1.1.1/custard/db/inspect.py
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 custard-1.1.1/custard/db/logger.py
+-rw-r--r--   0        0        0     4769 2020-02-02 00:00:00.000000 custard-1.1.1/custard/db/utils.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 custard-1.1.1/custard/expect/__init__.py
+-rw-r--r--   0        0        0     1287 2020-02-02 00:00:00.000000 custard-1.1.1/custard/expect/context.py
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 custard-1.1.1/custard/expect/exceptions.py
+-rw-r--r--   0        0        0     3424 2020-02-02 00:00:00.000000 custard-1.1.1/custard/expect/record.py
+-rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 custard-1.1.1/custard/expect/spacer.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 custard-1.1.1/custard/extra/__init__.py
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 custard-1.1.1/custard/function/__init__.py
+-rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 custard-1.1.1/custard/function/callsource.py
+-rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 custard-1.1.1/custard/function/traverse.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 custard-1.1.1/custard/hitfilter/__init__.py
+-rw-r--r--   0        0        0     2948 2020-02-02 00:00:00.000000 custard-1.1.1/custard/hitfilter/hitfilter.py
+-rw-r--r--   0        0        0   761348 2020-02-02 00:00:00.000000 custard-1.1.1/custard/hitfilter/keywords
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 custard-1.1.1/custard/json/__init__.py
+-rw-r--r--   0        0        0     9316 2020-02-02 00:00:00.000000 custard-1.1.1/custard/json/jsonlogger.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 custard-1.1.1/custard/kaptcha/__init__.py
+-rw-r--r--   0        0        0     9495 2020-02-02 00:00:00.000000 custard-1.1.1/custard/kaptcha/captcha.py
+-rw-r--r--   0        0        0   171508 2020-02-02 00:00:00.000000 custard-1.1.1/custard/kaptcha/font1.ttf
+-rw-r--r--   0        0        0    42452 2020-02-02 00:00:00.000000 custard-1.1.1/custard/kaptcha/font2.ttf
+-rw-r--r--   0        0        0    92956 2020-02-02 00:00:00.000000 custard-1.1.1/custard/kaptcha/font3.ttf
+-rw-r--r--   0        0        0   314452 2020-02-02 00:00:00.000000 custard-1.1.1/custard/kaptcha/font4.ttf
+-rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 custard-1.1.1/custard/limiter/__init__.py
+-rw-r--r--   0        0        0     2106 2020-02-02 00:00:00.000000 custard-1.1.1/custard/limiter/depends.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 custard-1.1.1/custard/limiter/enums.py
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 custard-1.1.1/custard/limiter/execres.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 custard-1.1.1/custard/lock/__init__.py
+-rw-r--r--   0        0        0     3070 2020-02-02 00:00:00.000000 custard-1.1.1/custard/lock/redis_lock.py
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 custard-1.1.1/custard/lock/thread_lock.py
+-rw-r--r--   0        0        0    12051 2020-02-02 00:00:00.000000 custard-1.1.1/custard/lodash/README.md
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 custard-1.1.1/custard/lodash/__init__.py
+-rw-r--r--   0        0        0     5417 2020-02-02 00:00:00.000000 custard-1.1.1/custard/lodash/arrays.py
+-rw-r--r--   0        0        0     4307 2020-02-02 00:00:00.000000 custard-1.1.1/custard/lodash/maths.py
+-rw-r--r--   0        0        0     3474 2020-02-02 00:00:00.000000 custard-1.1.1/custard/lodash/number.py
+-rw-r--r--   0        0        0     7238 2020-02-02 00:00:00.000000 custard-1.1.1/custard/lodash/string.py
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 custard-1.1.1/custard/lodash/utilities.py
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 custard-1.1.1/custard/minioss/__init__.py
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 custard-1.1.1/custard/minioss/aliyun.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 custard-1.1.1/custard/minioss/enums.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 custard-1.1.1/custard/minioss/gitee.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 custard-1.1.1/custard/minioss/minio.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 custard-1.1.1/custard/minioss/qiniu.py
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 custard-1.1.1/custard/minioss/tencent.py
+-rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 custard-1.1.1/custard/mock/__init__.py
+-rw-r--r--   0        0        0    14510 2020-02-02 00:00:00.000000 custard-1.1.1/custard/mock/mini_racer.py
+-rw-r--r--   0        0        0   366292 2020-02-02 00:00:00.000000 custard-1.1.1/custard/mock/mock.min.js
+-rw-r--r--   0        0        0   292581 2020-02-02 00:00:00.000000 custard-1.1.1/custard/mock/mock.old.min.js
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 custard-1.1.1/custard/network/asynchttp.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 custard-1.1.1/custard/network/enums.py
+-rw-r--r--   0        0        0     3426 2020-02-02 00:00:00.000000 custard-1.1.1/custard/network/httpclient.py
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 custard-1.1.1/custard/pagination/__init__.py
+-rw-r--r--   0        0        0     4269 2020-02-02 00:00:00.000000 custard-1.1.1/custard/pagination/api.py
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 custard-1.1.1/custard/pagination/async_sqlalchemy.py
+-rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 custard-1.1.1/custard/pagination/bases.py
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 custard-1.1.1/custard/pagination/default.py
+-rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 custard-1.1.1/custard/pagination/iterables.py
+-rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 custard-1.1.1/custard/pagination/limit_offset.py
+-rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 custard-1.1.1/custard/pagination/pagination.py
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 custard-1.1.1/custard/pagination/paginator.py
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 custard-1.1.1/custard/pagination/sync_sqlalchemy.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 custard-1.1.1/custard/pio/__init__.py
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 custard-1.1.1/custard/rediscluster/__init__.py
+-rw-r--r--   0        0        0    49439 2020-02-02 00:00:00.000000 custard-1.1.1/custard/rediscluster/client.py
+-rw-r--r--   0        0        0    24730 2020-02-02 00:00:00.000000 custard-1.1.1/custard/rediscluster/connection.py
+-rw-r--r--   0        0        0     2722 2020-02-02 00:00:00.000000 custard-1.1.1/custard/rediscluster/crc.py
+-rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 custard-1.1.1/custard/rediscluster/exceptions.py
+-rw-r--r--   0        0        0    17930 2020-02-02 00:00:00.000000 custard-1.1.1/custard/rediscluster/nodemanager.py
+-rw-r--r--   0        0        0    19857 2020-02-02 00:00:00.000000 custard-1.1.1/custard/rediscluster/pipeline.py
+-rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 custard-1.1.1/custard/rediscluster/pubsub.py
+-rw-r--r--   0        0        0     6161 2020-02-02 00:00:00.000000 custard-1.1.1/custard/rediscluster/utils.py
+-rw-r--r--   0        0        0     3730 2020-02-02 00:00:00.000000 custard-1.1.1/custard/rediscluster/benchmarks/simple.py
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 custard-1.1.1/custard/rediscluster/docs/authors.md
+-rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 custard-1.1.1/custard/rediscluster/docs/benchmarks.md
+-rw-r--r--   0        0        0     5039 2020-02-02 00:00:00.000000 custard-1.1.1/custard/rediscluster/docs/client.md
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 custard-1.1.1/custard/rediscluster/docs/logging.md
+-rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 custard-1.1.1/custard/rediscluster/docs/readonly-mode.md
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 custard-1.1.1/custard/rediscluster/docs/scripting.md
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 custard-1.1.1/custard/rediscluster/examples/basic.py
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 custard-1.1.1/custard/rediscluster/examples/basic_elasticache_password_protected.py
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 custard-1.1.1/custard/rediscluster/examples/basic_password_protected.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 custard-1.1.1/custard/rediscluster/examples/from_url_password_protected.py
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 custard-1.1.1/custard/rediscluster/examples/generate_slot_keys.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 custard-1.1.1/custard/rediscluster/examples/incr-test-writer.py
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 custard-1.1.1/custard/rediscluster/examples/pipeline-incrby.py
+-rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 custard-1.1.1/custard/rediscluster/examples/pipeline-readonly-replicas.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 custard-1.1.1/custard/rediscluster/tests/__init__.py
+-rw-r--r--   0        0        0     8789 2020-02-02 00:00:00.000000 custard-1.1.1/custard/rediscluster/tests/conftest.py
+-rw-r--r--   0        0        0    49667 2020-02-02 00:00:00.000000 custard-1.1.1/custard/rediscluster/tests/redis-trib.rb
+-rw-r--r--   0        0        0    37246 2020-02-02 00:00:00.000000 custard-1.1.1/custard/rediscluster/tests/test_cluster_connection_pool.py
+-rw-r--r--   0        0        0    21655 2020-02-02 00:00:00.000000 custard-1.1.1/custard/rediscluster/tests/test_cluster_node_manager.py
+-rw-r--r--   0        0        0    20837 2020-02-02 00:00:00.000000 custard-1.1.1/custard/rediscluster/tests/test_cluster_obj.py
+-rw-r--r--   0        0        0   103248 2020-02-02 00:00:00.000000 custard-1.1.1/custard/rediscluster/tests/test_commands.py
+-rw-r--r--   0        0        0    18019 2020-02-02 00:00:00.000000 custard-1.1.1/custard/rediscluster/tests/test_commands_cluster.py
+-rw-r--r--   0        0        0     4355 2020-02-02 00:00:00.000000 custard-1.1.1/custard/rediscluster/tests/test_encoding.py
+-rw-r--r--   0        0        0     3155 2020-02-02 00:00:00.000000 custard-1.1.1/custard/rediscluster/tests/test_encoding_cluster.py
+-rw-r--r--   0        0        0     8016 2020-02-02 00:00:00.000000 custard-1.1.1/custard/rediscluster/tests/test_lock.py
+-rw-r--r--   0        0        0     2402 2020-02-02 00:00:00.000000 custard-1.1.1/custard/rediscluster/tests/test_monitor.py
+-rw-r--r--   0        0        0     5774 2020-02-02 00:00:00.000000 custard-1.1.1/custard/rediscluster/tests/test_multiprocessing.py
+-rw-r--r--   0        0        0     5345 2020-02-02 00:00:00.000000 custard-1.1.1/custard/rediscluster/tests/test_multiprocessing_cluster.py
+-rw-r--r--   0        0        0    12150 2020-02-02 00:00:00.000000 custard-1.1.1/custard/rediscluster/tests/test_pipeline.py
+-rw-r--r--   0        0        0    13109 2020-02-02 00:00:00.000000 custard-1.1.1/custard/rediscluster/tests/test_pipeline_cluster.py
+-rw-r--r--   0        0        0    21952 2020-02-02 00:00:00.000000 custard-1.1.1/custard/rediscluster/tests/test_pubsub.py
+-rw-r--r--   0        0        0     5383 2020-02-02 00:00:00.000000 custard-1.1.1/custard/rediscluster/tests/test_scripting.py
+-rw-r--r--   0        0        0     5374 2020-02-02 00:00:00.000000 custard-1.1.1/custard/rediscluster/tests/test_utils.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 custard-1.1.1/custard/script/__init__.py
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 custard-1.1.1/custard/script/compat.py
+-rw-r--r--   0        0        0    16449 2020-02-02 00:00:00.000000 custard-1.1.1/custard/script/parser.py
+-rw-r--r--   0        0        0     2589 2020-02-02 00:00:00.000000 custard-1.1.1/custard/script/schema.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 custard-1.1.1/custard/socket/__init__.py
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 custard-1.1.1/custard/swagger/__init__.py
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 custard-1.1.1/custard/swagger/exception.py
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 custard-1.1.1/custard/swagger/loader.py
+-rw-r--r--   0        0        0     6766 2020-02-02 00:00:00.000000 custard-1.1.1/custard/swagger/swagger.py
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 custard-1.1.1/custard/swagger/utils.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 custard-1.1.1/custard/system/__init__.py
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 custard-1.1.1/custard/time/__init__.py
+-rw-r--r--   0        0        0     6215 2020-02-02 00:00:00.000000 custard-1.1.1/custard/time/dafunc.py
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 custard-1.1.1/custard/time/exceptions.py
+-rw-r--r--   0        0        0     5964 2020-02-02 00:00:00.000000 custard-1.1.1/custard/time/moment.py
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 custard-1.1.1/custard/time/stoppable_thread.py
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 custard-1.1.1/custard/utils/__init__.py
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 custard-1.1.1/custard/utils/datasets.py
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 custard-1.1.1/custard/utils/decorators.py
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 custard-1.1.1/custard/utils/text.py
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 custard-1.1.1/examples/async_lur.py
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 custard-1.1.1/examples/crypto.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 custard-1.1.1/examples/datum.py
+-rw-r--r--   0        0        0     3650 2020-02-02 00:00:00.000000 custard-1.1.1/examples/decorator.py
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 custard-1.1.1/examples/dts.py
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 custard-1.1.1/examples/hitfilter.py
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 custard-1.1.1/examples/hitfilter_keyword
+-rw-r--r--   0        0        0     8968 2020-02-02 00:00:00.000000 custard-1.1.1/examples/json_logger.py
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 custard-1.1.1/examples/kaptcha.py
+-rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 custard-1.1.1/examples/kaptcha_execution_time.py
+-rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 custard-1.1.1/examples/limiter.py
+-rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 custard-1.1.1/examples/mock.py
+-rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 custard-1.1.1/examples/pagination_async_sqlalchemy.py
+-rw-r--r--   0        0        0     2170 2020-02-02 00:00:00.000000 custard-1.1.1/examples/pagination_sqlalchemy.py
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 custard-1.1.1/examples/swagger_online_change.py
+-rw-r--r--   0        0        0     6431 2020-02-02 00:00:00.000000 custard-1.1.1/examples/swagger_usabletest.py
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 custard-1.1.1/examples/useragent.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 custard-1.1.1/.gitignore
+-rw-r--r--   0        0        0     6988 2020-02-02 00:00:00.000000 custard-1.1.1/README.md
+-rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 custard-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0    10068 2020-02-02 00:00:00.000000 custard-1.1.1/PKG-INFO
```

### Comparing `custard-1.1.0/.github/workflows/python-publish.yml` & `custard-1.1.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/.vscode/launch.json` & `custard-1.1.1/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/.vscode/settings.json` & `custard-1.1.1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/cache/async_lru.py` & `custard-1.1.1/custard/cache/async_lru.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/cache/async_lur.md` & `custard-1.1.1/custard/cache/async_lur.md`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/cache/redis.py` & `custard-1.1.1/custard/cache/redis.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/core/__init__.py` & `custard-1.1.1/custard/core/__init__.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/core/decode.py` & `custard-1.1.1/custard/core/decode.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/core/factory.py` & `custard-1.1.1/custard/core/factory.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/core/kerberos.py` & `custard-1.1.1/custard/core/kerberos.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/core/processor.py` & `custard-1.1.1/custard/core/processor.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/core/regular.py` & `custard-1.1.1/custard/core/regular.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/core/snowflake.py` & `custard-1.1.1/custard/core/snowflake.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/core/system.py` & `custard-1.1.1/custard/core/system.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/core/useragent.py` & `custard-1.1.1/custard/core/useragent.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/core/xml2dict.py` & `custard-1.1.1/custard/core/xml2dict.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/core/xprint.py` & `custard-1.1.1/custard/core/xprint.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/cron/batch_task.py` & `custard-1.1.1/custard/cron/batch_task.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/crypto/crypto.py` & `custard-1.1.1/custard/crypto/crypto.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/crypto/streambody.py` & `custard-1.1.1/custard/crypto/streambody.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/curl/parse.py` & `custard-1.1.1/custard/curl/parse.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/db/inspect.py` & `custard-1.1.1/custard/db/inspect.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/db/logger.py` & `custard-1.1.1/custard/db/logger.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/db/utils.py` & `custard-1.1.1/custard/db/utils.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/expect/context.py` & `custard-1.1.1/custard/expect/context.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/expect/exceptions.py` & `custard-1.1.1/custard/expect/exceptions.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/expect/record.py` & `custard-1.1.1/custard/expect/record.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/expect/spacer.py` & `custard-1.1.1/custard/expect/spacer.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/function/callsource.py` & `custard-1.1.1/custard/function/callsource.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/function/traverse.py` & `custard-1.1.1/custard/function/traverse.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/hitfilter/hitfilter.py` & `custard-1.1.1/custard/hitfilter/hitfilter.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/hitfilter/keywords` & `custard-1.1.1/custard/hitfilter/keywords`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/json/jsonlogger.py` & `custard-1.1.1/custard/json/jsonlogger.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/kaptcha/captcha.py` & `custard-1.1.1/custard/kaptcha/captcha.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/kaptcha/font1.ttf` & `custard-1.1.1/custard/kaptcha/font1.ttf`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/kaptcha/font2.ttf` & `custard-1.1.1/custard/kaptcha/font2.ttf`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/kaptcha/font3.ttf` & `custard-1.1.1/custard/kaptcha/font3.ttf`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/kaptcha/font4.ttf` & `custard-1.1.1/custard/kaptcha/font4.ttf`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/limiter/__init__.py` & `custard-1.1.1/custard/limiter/__init__.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/limiter/depends.py` & `custard-1.1.1/custard/limiter/depends.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/lock/redis_lock.py` & `custard-1.1.1/custard/lock/redis_lock.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/lock/thread_lock.py` & `custard-1.1.1/custard/lock/thread_lock.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/lodash/README.md` & `custard-1.1.1/custard/lodash/README.md`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/lodash/__init__.py` & `custard-1.1.1/custard/lodash/__init__.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/lodash/arrays.py` & `custard-1.1.1/custard/lodash/arrays.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/lodash/maths.py` & `custard-1.1.1/custard/lodash/maths.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/lodash/number.py` & `custard-1.1.1/custard/lodash/number.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/lodash/string.py` & `custard-1.1.1/custard/lodash/string.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/lodash/utilities.py` & `custard-1.1.1/custard/lodash/utilities.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/mock/__init__.py` & `custard-1.1.1/custard/mock/__init__.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/mock/mini_racer.py` & `custard-1.1.1/custard/mock/mini_racer.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/mock/mock.min.js` & `custard-1.1.1/custard/mock/mock.min.js`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/mock/mock.old.min.js` & `custard-1.1.1/custard/mock/mock.old.min.js`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/network/httpclient.py` & `custard-1.1.1/custard/network/httpclient.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/pagination/__init__.py` & `custard-1.1.1/custard/pagination/__init__.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/pagination/api.py` & `custard-1.1.1/custard/pagination/api.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/pagination/async_sqlalchemy.py` & `custard-1.1.1/custard/pagination/async_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/pagination/bases.py` & `custard-1.1.1/custard/pagination/bases.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/pagination/default.py` & `custard-1.1.1/custard/pagination/default.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/pagination/iterables.py` & `custard-1.1.1/custard/pagination/iterables.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/pagination/limit_offset.py` & `custard-1.1.1/custard/pagination/limit_offset.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/pagination/pagination.py` & `custard-1.1.1/custard/pagination/pagination.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/pagination/paginator.py` & `custard-1.1.1/custard/pagination/paginator.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/pagination/sync_sqlalchemy.py` & `custard-1.1.1/custard/pagination/sync_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/rediscluster/__init__.py` & `custard-1.1.1/custard/rediscluster/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 # -*- coding: utf-8 -*-
 
 # python std lib
 import logging
 
 # rediscluster imports
-from rediscluster.client import RedisCluster
-from rediscluster.connection import (
+from custard.rediscluster.client import RedisCluster
+from custard.rediscluster.connection import (
     ClusterBlockingConnectionPool,
     ClusterConnection,
     ClusterConnectionPool,
 )
-from rediscluster.exceptions import (
+from custard.rediscluster.exceptions import (
     RedisClusterException,
     RedisClusterError,
     ClusterDownException,
     ClusterError,
     ClusterCrossSlotError,
     ClusterDownError,
     AskError,
     TryAgainError,
     MovedError,
     MasterDownError,
 )
-from rediscluster.pipeline import ClusterPipeline
+from custard.rediscluster.pipeline import ClusterPipeline
 
 
 def int_or_str(value):
     try:
         return int(value)
     except ValueError:
         return value
```

### Comparing `custard-1.1.0/custard/rediscluster/client.py` & `custard-1.1.1/custard/rediscluster/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1486,8 +1486,8 @@
 
         By default it will generate a 16 character long string based on
         ascii uppercase letters and digits.
         """
         return "".join(random.choice(chars) for _ in range(size))
 
 
-from rediscluster.pipeline import ClusterPipeline
+from custard.rediscluster.pipeline import ClusterPipeline
```

### Comparing `custard-1.1.0/custard/rediscluster/connection.py` & `custard-1.1.1/custard/rediscluster/connection.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,146 +9,177 @@
 from contextlib import contextmanager
 from itertools import chain
 from collections import defaultdict
 
 # rediscluster imports
 from .nodemanager import NodeManager
 from .exceptions import (
-    RedisClusterException, AskError, MovedError,
-    TryAgainError, ClusterDownError, ClusterCrossSlotError,
-    MasterDownError, SlotNotCoveredError,
+    RedisClusterException,
+    AskError,
+    MovedError,
+    TryAgainError,
+    ClusterDownError,
+    ClusterCrossSlotError,
+    MasterDownError,
+    SlotNotCoveredError,
 )
 
 # 3rd party imports
 from redis._compat import nativestr, LifoQueue, Full, Empty
 from redis.client import dict_merge
-from redis.connection import ConnectionPool, Connection, DefaultParser, SSLConnection, UnixDomainSocketConnection
+from redis.connection import (
+    ConnectionPool,
+    Connection,
+    DefaultParser,
+    SSLConnection,
+    UnixDomainSocketConnection,
+)
 from redis.exceptions import ConnectionError
 
 log = logging.getLogger(__name__)
 
 
 class ClusterParser(DefaultParser):
-    """
-    """
+    """ """
+
     EXCEPTION_CLASSES = dict_merge(
-        DefaultParser.EXCEPTION_CLASSES, {
-            'ASK': AskError,
-            'TRYAGAIN': TryAgainError,
-            'MOVED': MovedError,
-            'CLUSTERDOWN': ClusterDownError,
-            'CROSSSLOT': ClusterCrossSlotError,
-            'MASTERDOWN': MasterDownError,
-        })
+        DefaultParser.EXCEPTION_CLASSES,
+        {
+            "ASK": AskError,
+            "TRYAGAIN": TryAgainError,
+            "MOVED": MovedError,
+            "CLUSTERDOWN": ClusterDownError,
+            "CROSSSLOT": ClusterCrossSlotError,
+            "MASTERDOWN": MasterDownError,
+        },
+    )
 
 
 class ClusterConnection(Connection):
     "Manages TCP communication to and from a Redis server"
 
     def __init__(self, *args, **kwargs):
         log.debug("Creating new ClusterConnection instance")
         log.debug(str(args) + " : " + str(kwargs))
 
-        self.readonly = kwargs.pop('readonly', False)
-        kwargs['parser_class'] = ClusterParser
+        self.readonly = kwargs.pop("readonly", False)
+        kwargs["parser_class"] = ClusterParser
         super(ClusterConnection, self).__init__(*args, **kwargs)
 
     def on_connect(self):
-        '''
+        """
         Initialize the connection, authenticate and select a database and send READONLY if it is
         set during object initialization.
-        '''
+        """
         super(ClusterConnection, self).on_connect()
 
         if self.readonly:
-            log.debug("Sending READONLY command to server to configure connection as readonly")
+            log.debug(
+                "Sending READONLY command to server to configure connection as readonly"
+            )
             log.debug(str(self))
 
-            self.send_command('READONLY')
+            self.send_command("READONLY")
 
-            if nativestr(self.read_response()) != 'OK':
-                raise ConnectionError('READONLY command failed')
+            if nativestr(self.read_response()) != "OK":
+                raise ConnectionError("READONLY command failed")
 
 
 class SSLClusterConnection(SSLConnection):
     """
     Manages TCP communication over TLS/SSL to and from a Redis cluster
     Usage:
         pool = ClusterConnectionPool(connection_class=SSLClusterConnection, ...)
         client = RedisCluster(connection_pool=pool)
     """
 
     def __init__(self, *args, **kwargs):
         log.debug("Creating new SSLClusterConnection instance")
         log.debug(str(args) + " : " + str(kwargs))
 
-        self.readonly = kwargs.pop('readonly', False)
+        self.readonly = kwargs.pop("readonly", False)
         # need to pop this off as the redis/connection.py SSLConnection init doesn't work with ssl passed in
-        if 'ssl' in kwargs:
-            kwargs.pop('ssl')
-        kwargs['parser_class'] = ClusterParser
+        if "ssl" in kwargs:
+            kwargs.pop("ssl")
+        kwargs["parser_class"] = ClusterParser
         super(SSLClusterConnection, self).__init__(**kwargs)
 
     def on_connect(self):
-        '''
+        """
         Initialize the connection, authenticate and select a database and send READONLY if it is
         set during object initialization.
-        '''
+        """
         super(SSLClusterConnection, self).on_connect()
 
         if self.readonly:
-            log.debug("Sending READONLY command to server to configure connection as readonly")
+            log.debug(
+                "Sending READONLY command to server to configure connection as readonly"
+            )
 
-            self.send_command('READONLY')
+            self.send_command("READONLY")
 
-            if nativestr(self.read_response()) != 'OK':
-                raise ConnectionError('READONLY command failed')
+            if nativestr(self.read_response()) != "OK":
+                raise ConnectionError("READONLY command failed")
 
 
 class ClusterConnectionPool(ConnectionPool):
     """
     Custom connection pool for rediscluster
     """
+
     RedisClusterDefaultTimeout = None
 
-    def __init__(self, startup_nodes=None, init_slot_cache=True, connection_class=None,
-                 max_connections=None, max_connections_per_node=False, reinitialize_steps=None,
-                 skip_full_coverage_check=False, nodemanager_follow_cluster=False, host_port_remap=None,
-                 **connection_kwargs):
+    def __init__(
+        self,
+        startup_nodes=None,
+        init_slot_cache=True,
+        connection_class=None,
+        max_connections=None,
+        max_connections_per_node=False,
+        reinitialize_steps=None,
+        skip_full_coverage_check=False,
+        nodemanager_follow_cluster=False,
+        host_port_remap=None,
+        **connection_kwargs
+    ):
         """
         :skip_full_coverage_check:
             Skips the check of cluster-require-full-coverage config, useful for clusters
             without the CONFIG command (like aws)
         :nodemanager_follow_cluster:
             The node manager will during initialization try the last set of nodes that
             it was operating on. This will allow the client to drift along side the cluster
             if the cluster nodes move around a lot.
         """
         log.debug("Creating new ClusterConnectionPool instance")
 
         if connection_class is None:
             connection_class = ClusterConnection
 
-        super(ClusterConnectionPool, self).__init__(connection_class=connection_class, max_connections=max_connections)
+        super(ClusterConnectionPool, self).__init__(
+            connection_class=connection_class, max_connections=max_connections
+        )
 
         # Special case to make from_url method compliant with cluster setting.
         # from_url method will send in the ip and port through a different variable then the
         # regular startup_nodes variable.
         if startup_nodes is None:
-            if 'port' in connection_kwargs and 'host' in connection_kwargs:
-                startup_nodes = [{
-                    'host': connection_kwargs.pop('host'),
-                    'port': str(connection_kwargs.pop('port')),
-                }]
+            if "port" in connection_kwargs and "host" in connection_kwargs:
+                startup_nodes = [
+                    {
+                        "host": connection_kwargs.pop("host"),
+                        "port": str(connection_kwargs.pop("port")),
+                    }
+                ]
 
-        self.max_connections = max_connections or 2 ** 31
+        self.max_connections = max_connections or 2**31
         self.max_connections_per_node = max_connections_per_node
 
         if connection_class == SSLClusterConnection:
-            connection_kwargs['ssl'] = True  # needed in Redis init
+            connection_kwargs["ssl"] = True  # needed in Redis init
 
         self.nodes = NodeManager(
             startup_nodes,
             reinitialize_steps=reinitialize_steps,
             skip_full_coverage_check=skip_full_coverage_check,
             max_connections=self.max_connections,
             nodemanager_follow_cluster=nodemanager_follow_cluster,
@@ -160,28 +191,34 @@
             self.nodes.initialize()
 
         self.connections = {}
         self.connection_kwargs = connection_kwargs
         self.reset()
 
         if "socket_timeout" not in self.connection_kwargs:
-            self.connection_kwargs["socket_timeout"] = ClusterConnectionPool.RedisClusterDefaultTimeout
+            self.connection_kwargs[
+                "socket_timeout"
+            ] = ClusterConnectionPool.RedisClusterDefaultTimeout
 
     def __repr__(self):
         """
         Return a string with all unique ip:port combinations that this pool is connected to.
         """
         nodes = [
-            {'host': i['host'], 'port': i['port']}
-            for i in self.nodes.startup_nodes
+            {"host": i["host"], "port": i["port"]} for i in self.nodes.startup_nodes
         ]
 
         return "{0}<{1}>".format(
             type(self).__name__,
-            ", ".join([repr(self.connection_class(**self.connection_kwargs)) for node in nodes])
+            ", ".join(
+                [
+                    repr(self.connection_class(**self.connection_kwargs))
+                    for node in nodes
+                ]
+            ),
         )
 
     def reset(self):
         """
         Resets the connection pool back to a clean state.
         """
         log.debug("Resetting ConnectionPool")
@@ -190,16 +227,15 @@
         self._created_connections = 0
         self._created_connections_per_node = {}  # Dict(Node, Int)
         self._available_connections = {}  # Dict(Node, List)
         self._in_use_connections = {}  # Dict(Node, Set)
         self._check_lock = threading.Lock()
 
     def _checkpid(self):
-        """
-        """
+        """ """
         if self.pid != os.getpid():
             with self._check_lock:
                 if self.pid == os.getpid():
                     # another thread already did the work while we waited
                     # on the lock.
                     return
                 self.disconnect()
@@ -208,51 +244,53 @@
     def get_connection(self, command_name, *keys, **options):
         """
         # TODO: Default method entrypoint.
         Keys, options is not in use by any of the standard code.
         """
         # Only pubsub command/connection should be allowed here
         if command_name != "pubsub":
-            raise RedisClusterException("Only 'pubsub' commands can be used by get_connection()")
+            raise RedisClusterException(
+                "Only 'pubsub' commands can be used by get_connection()"
+            )
 
-        channel = options.pop('channel', None)
+        channel = options.pop("channel", None)
 
         if not channel:
             return self.get_random_connection()
 
         slot = self.nodes.keyslot(channel)
         node = self.get_master_node_by_slot(slot)
 
         self._checkpid()
 
         try:
             connection = self._available_connections.get(node["name"], []).pop()
         except IndexError:
             connection = self.make_connection(node)
 
-        if node['name'] not in self._in_use_connections:
-            self._in_use_connections[node['name']] = set()
+        if node["name"] not in self._in_use_connections:
+            self._in_use_connections[node["name"]] = set()
 
-        self._in_use_connections[node['name']].add(connection)
+        self._in_use_connections[node["name"]].add(connection)
 
         try:
             # ensure this connection is connected to Redis
             connection.connect()
             # connections that the pool provides should be ready to send
             # a command. if not, the connection was either returned to the
             # pool before all data has been read or the socket has been
             # closed. either way, reconnect and verify everything is good.
             try:
                 if connection.can_read():
-                    raise ConnectionError('Connection has data')
+                    raise ConnectionError("Connection has data")
             except ConnectionError:
                 connection.disconnect()
                 connection.connect()
                 if connection.can_read():
-                    raise ConnectionError('Connection not ready')
+                    raise ConnectionError("Connection not ready")
         except BaseException:
             # release the connection back to the pool so that we don't
             # leak it
             self.release(connection)
             raise
 
         return connection
@@ -260,21 +298,27 @@
     def make_connection(self, node):
         """
         Create a new connection
         """
         num_connections = self.count_all_num_connections(node)
         if num_connections >= self.max_connections:
             if self.max_connections_per_node:
-                raise RedisClusterException("Too many connection ({0}) for node: {1}".format(num_connections, node['name']))
+                raise RedisClusterException(
+                    "Too many connection ({0}) for node: {1}".format(
+                        num_connections, node["name"]
+                    )
+                )
 
             raise RedisClusterException("Too many connections")
 
-        self._created_connections_per_node.setdefault(node['name'], 0)
-        self._created_connections_per_node[node['name']] += 1
-        connection = self.connection_class(host=node["host"], port=node["port"], **self.connection_kwargs)
+        self._created_connections_per_node.setdefault(node["name"], 0)
+        self._created_connections_per_node[node["name"]] += 1
+        connection = self.connection_class(
+            host=node["host"], port=node["port"], **self.connection_kwargs
+        )
 
         # Must store node in the connection to make it easier to track
         connection.node = node
 
         return connection
 
     def release(self, connection):
@@ -292,15 +336,17 @@
 
         if connection in i_c:
             i_c.remove(connection)
         else:
             pass
             # TODO: Log.warning("Tried to release connection that did not exist any longer : {0}".format(connection))
 
-        self._available_connections.setdefault(connection.node["name"], []).append(connection)
+        self._available_connections.setdefault(connection.node["name"], []).append(
+            connection
+        )
 
     def disconnect(self):
         """
         Nothing that requires any overwrite.
         """
         all_conns = chain(
             self._available_connections.values(),
@@ -308,18 +354,17 @@
         )
 
         for node_connections in all_conns:
             for connection in node_connections:
                 connection.disconnect()
 
     def count_all_num_connections(self, node):
-        """
-        """
+        """ """
         if self.max_connections_per_node:
-            return self._created_connections_per_node.get(node['name'], 0)
+            return self._created_connections_per_node.get(node["name"], 0)
 
         return sum([i for i in list(self._created_connections_per_node.values())])
 
     def get_random_connection(self):
         """
         Open new connection to random redis server.
         """
@@ -330,18 +375,19 @@
 
             if connection:
                 return connection
 
         raise Exception("Cant reach a single startup node.")
 
     def get_connection_by_key(self, key, command):
-        """
-        """
+        """ """
         if not key:
-            raise RedisClusterException("No way to dispatch this command to Redis Cluster.")
+            raise RedisClusterException(
+                "No way to dispatch this command to Redis Cluster."
+            )
 
         return self.get_connection_by_slot(self.nodes.keyslot(key))
 
     def get_connection_by_slot(self, slot):
         """
         Determine what server a specific slot belongs to and return a redis object that is connected
         """
@@ -366,34 +412,35 @@
             connection = self.make_connection(node)
 
         self._in_use_connections.setdefault(node["name"], set()).add(connection)
 
         return connection
 
     def get_master_node_by_slot(self, slot):
-        """
-        """
+        """ """
         try:
             return self.nodes.slots[slot][0]
         except KeyError:
-            raise SlotNotCoveredError('Slot "{slot}" not covered by the cluster. "skip_full_coverage_check={skip_full_coverage_check}"'.format(
-                slot=slot, skip_full_coverage_check=self.nodes._skip_full_coverage_check,
-            ))
+            raise SlotNotCoveredError(
+                'Slot "{slot}" not covered by the cluster. "skip_full_coverage_check={skip_full_coverage_check}"'.format(
+                    slot=slot,
+                    skip_full_coverage_check=self.nodes._skip_full_coverage_check,
+                )
+            )
 
     def get_node_by_slot(self, slot, *args, **kwargs):
-        """
-        """
+        """ """
         return self.get_master_node_by_slot(slot)
 
 
 class ClusterBlockingConnectionPool(ClusterConnectionPool):
     """
     Thread-safe blocking connection pool for Redis Cluster::
 
-        >>> from rediscluster.client import RedisCluster
+        >>> from custard.rediscluster.client import RedisCluster
         >>> client = RedisCluster(connection_pool=ClusterBlockingConnectionPool())
 
     It performs the same function as the default
     ``:py:class: ~rediscluster.connection.ClusterConnectionPool`` implementation, in that,
     it maintains a pool of reusable connections to a redis cluster that can be shared by
     multiple redis clients (safely across threads if required).
 
@@ -415,18 +462,27 @@
         >>> pool = ClusterBlockingConnectionPool(timeout=None)
 
         # Raise a ``ConnectionError`` after five seconds if a connection is
         # not available.
         >>> pool = ClusterBlockingConnectionPool(timeout=5)
     """
 
-    def __init__(self, startup_nodes=None, init_slot_cache=True, connection_class=None,
-                 max_connections=50, max_connections_per_node=False, reinitialize_steps=None,
-                 skip_full_coverage_check=False, nodemanager_follow_cluster=False,
-                 timeout=20, **connection_kwargs):
+    def __init__(
+        self,
+        startup_nodes=None,
+        init_slot_cache=True,
+        connection_class=None,
+        max_connections=50,
+        max_connections_per_node=False,
+        reinitialize_steps=None,
+        skip_full_coverage_check=False,
+        nodemanager_follow_cluster=False,
+        timeout=20,
+        **connection_kwargs
+    ):
         self.timeout = timeout
 
         super(ClusterBlockingConnectionPool, self).__init__(
             startup_nodes=startup_nodes,
             init_slot_cache=init_slot_cache,
             connection_class=connection_class,
             max_connections=max_connections,
@@ -445,16 +501,19 @@
             try:
                 pool.put_nowait(None)
             except Full:
                 break
         return pool
 
     def _get_pool(self, node):
-        return self._pool_by_node[node["name"]] \
-            if self.max_connections_per_node or node is None else self._group_pool
+        return (
+            self._pool_by_node[node["name"]]
+            if self.max_connections_per_node or node is None
+            else self._group_pool
+        )
 
     def reset(self):
         self.pid = os.getpid()
         self._check_lock = threading.Lock()
 
         """
         We could use a conditional branch on ``max_connections_per_node`` to see which pool to initialize,
@@ -467,33 +526,35 @@
         self._group_pool = self._blocking_pool_factory()
 
         # Keep a list of actual connection instances so that we can
         # disconnect them later.
         self._connections = []
 
     def make_connection(self, node):
-        """ Create a new connection """
-        connection = self.connection_class(host=node["host"], port=node["port"], **self.connection_kwargs)
+        """Create a new connection"""
+        connection = self.connection_class(
+            host=node["host"], port=node["port"], **self.connection_kwargs
+        )
         self._connections.append(connection)
         connection.node = node
         return connection
 
     def get_connection(self, command_name, *keys, **options):
         if command_name != "pubsub":
-            raise RedisClusterException("Only 'pubsub' commands can be used by get_connection()")
+            raise RedisClusterException(
+                "Only 'pubsub' commands can be used by get_connection()"
+            )
 
-        channel = options.pop('channel', None)
+        channel = options.pop("channel", None)
 
         if not channel:
             # find random startup node and try to get connection again
             return self.get_random_connection()
         return self.get_connection_by_node(
-            self.get_master_node_by_slot(
-                self.nodes.keyslot(channel)
-            )
+            self.get_master_node_by_slot(self.nodes.keyslot(channel))
         )
 
     def get_connection_by_node(self, node):
         """
         Get a connection by node
         """
         self._checkpid()
@@ -561,42 +622,51 @@
 
 
 class ClusterReadOnlyConnectionPool(ClusterConnectionPool):
     """
     Readonly connection pool for rediscluster
     """
 
-    def __init__(self, startup_nodes=None, init_slot_cache=True, connection_class=None,
-                 max_connections=None, nodemanager_follow_cluster=False, **connection_kwargs):
-        """
-        """
+    def __init__(
+        self,
+        startup_nodes=None,
+        init_slot_cache=True,
+        connection_class=None,
+        max_connections=None,
+        nodemanager_follow_cluster=False,
+        **connection_kwargs
+    ):
+        """ """
         if connection_class is None:
             connection_class = ClusterConnection
         super(ClusterReadOnlyConnectionPool, self).__init__(
             startup_nodes=startup_nodes,
             init_slot_cache=init_slot_cache,
             connection_class=connection_class,
             max_connections=max_connections,
             readonly=True,
             nodemanager_follow_cluster=nodemanager_follow_cluster,
             **connection_kwargs
         )
 
-        self.master_node_commands = ('SCAN', 'SSCAN', 'HSCAN', 'ZSCAN')
+        self.master_node_commands = ("SCAN", "SSCAN", "HSCAN", "ZSCAN")
 
     def get_connection_by_key(self, key, command):
-        """
-        """
+        """ """
         if not key:
-            raise RedisClusterException("No way to dispatch this command to Redis Cluster.")
+            raise RedisClusterException(
+                "No way to dispatch this command to Redis Cluster."
+            )
 
         if command in self.master_node_commands:
             return self.get_master_connection_by_slot(self.nodes.keyslot(key))
         else:
-            return self.get_random_master_slave_connection_by_slot(self.nodes.keyslot(key))
+            return self.get_random_master_slave_connection_by_slot(
+                self.nodes.keyslot(key)
+            )
 
     def get_master_connection_by_slot(self, slot):
         """
         Returns a connection for the Master node for the specified slot.
 
         Do not return a random node if master node is not available for any reason.
         """
```

### Comparing `custard-1.1.0/custard/rediscluster/crc.py` & `custard-1.1.1/custard/rediscluster/crc.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/rediscluster/exceptions.py` & `custard-1.1.1/custard/rediscluster/exceptions.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/rediscluster/nodemanager.py` & `custard-1.1.1/custard/rediscluster/nodemanager.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/rediscluster/pipeline.py` & `custard-1.1.1/custard/rediscluster/pipeline.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/rediscluster/pubsub.py` & `custard-1.1.1/custard/rediscluster/pubsub.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/rediscluster/utils.py` & `custard-1.1.1/custard/rediscluster/utils.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/rediscluster/benchmarks/simple.py` & `custard-1.1.1/custard/rediscluster/benchmarks/simple.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/rediscluster/docs/authors.md` & `custard-1.1.1/custard/rediscluster/docs/authors.md`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/rediscluster/docs/benchmarks.md` & `custard-1.1.1/custard/rediscluster/docs/benchmarks.md`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/rediscluster/docs/client.md` & `custard-1.1.1/custard/rediscluster/docs/client.md`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/rediscluster/docs/logging.md` & `custard-1.1.1/custard/rediscluster/docs/logging.md`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/rediscluster/docs/readonly-mode.md` & `custard-1.1.1/custard/rediscluster/docs/readonly-mode.md`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/rediscluster/docs/scripting.md` & `custard-1.1.1/custard/rediscluster/docs/scripting.md`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/rediscluster/examples/basic_elasticache_password_protected.py` & `custard-1.1.1/custard/rediscluster/examples/basic_elasticache_password_protected.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/rediscluster/examples/generate_slot_keys.py` & `custard-1.1.1/custard/rediscluster/examples/generate_slot_keys.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/rediscluster/examples/pipeline-incrby.py` & `custard-1.1.1/custard/rediscluster/examples/pipeline-incrby.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/rediscluster/examples/pipeline-readonly-replicas.py` & `custard-1.1.1/custard/rediscluster/examples/pipeline-readonly-replicas.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/rediscluster/tests/conftest.py` & `custard-1.1.1/custard/rediscluster/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/rediscluster/tests/redis-trib.rb` & `custard-1.1.1/custard/rediscluster/tests/redis-trib.rb`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/rediscluster/tests/test_cluster_connection_pool.py` & `custard-1.1.1/custard/rediscluster/tests/test_cluster_connection_pool.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,19 +3,23 @@
 # python std lib
 import os
 import re
 import time
 from threading import Thread
 
 # rediscluster imports
-from rediscluster.connection import (
-    ClusterConnectionPool, ClusterBlockingConnectionPool, ClusterReadOnlyConnectionPool,
-    ClusterConnection, UnixDomainSocketConnection)
-from rediscluster.exceptions import RedisClusterException, SlotNotCoveredError
-from .conftest import (skip_if_server_version_lt, skip_for_no_cluster_impl)
+from custard.redisclusterconnection import (
+    ClusterConnectionPool,
+    ClusterBlockingConnectionPool,
+    ClusterReadOnlyConnectionPool,
+    ClusterConnection,
+    UnixDomainSocketConnection,
+)
+from custard.redisclusterexceptions import RedisClusterException, SlotNotCoveredError
+from .conftest import skip_if_server_version_lt, skip_for_no_cluster_impl
 
 # 3rd party imports
 import pytest
 import redis
 from mock import patch, Mock
 from redis.connection import ssl_available, to_bool
 from redis._compat import unicode
@@ -34,50 +38,64 @@
     def connect(self):
         pass
 
     def can_read(self):
         return False
 
 
-def get_pool(connection_kwargs=None, max_connections=None, max_connections_per_node=None, connection_class=DummyConnection, init_slot_cache=True):
+def get_pool(
+    connection_kwargs=None,
+    max_connections=None,
+    max_connections_per_node=None,
+    connection_class=DummyConnection,
+    init_slot_cache=True,
+):
     connection_kwargs = connection_kwargs or {}
     pool = ClusterConnectionPool(
         connection_class=connection_class,
         max_connections=max_connections,
         max_connections_per_node=max_connections_per_node,
         startup_nodes=[{"host": "127.0.0.1", "port": 7000}],
         init_slot_cache=init_slot_cache,
-        **connection_kwargs)
+        **connection_kwargs
+    )
     return pool
 
 
 class TestConnectionPool(object):
-    def get_pool(self, connection_kwargs=None, max_connections=None, max_connections_per_node=None,
-                 connection_class=DummyConnection, init_slot_cache=True):
+    def get_pool(
+        self,
+        connection_kwargs=None,
+        max_connections=None,
+        max_connections_per_node=None,
+        connection_class=DummyConnection,
+        init_slot_cache=True,
+    ):
         connection_kwargs = connection_kwargs or {}
         pool = ClusterConnectionPool(
             connection_class=connection_class,
             max_connections=max_connections,
             max_connections_per_node=max_connections_per_node,
             startup_nodes=[{"host": "127.0.0.1", "port": 7000}],
             init_slot_cache=init_slot_cache,
-            **connection_kwargs)
+            **connection_kwargs
+        )
         return pool
 
     def test_in_use_not_exists(self):
         """
         Test that if for some reason, the node that it tries to get the connection for
         do not exists in the _in_use_connection variable.
         """
         pool = self.get_pool()
         pool._in_use_connections = {}
         pool.get_connection("pubsub", channel="foobar")
 
     def test_connection_creation(self):
-        connection_kwargs = {'foo': 'bar', 'biz': 'baz'}
+        connection_kwargs = {"foo": "bar", "biz": "baz"}
         pool = self.get_pool(connection_kwargs=connection_kwargs)
         connection = pool.get_connection_by_node({"host": "127.0.0.1", "port": 7000})
         assert isinstance(connection, DummyConnection)
         assert connection.kwargs == connection_kwargs
 
     def test_multiple_connections(self):
         pool = self.get_pool()
@@ -99,85 +117,95 @@
         pool.get_connection_by_node({"host": "127.0.0.1", "port": 7000})
         pool.get_connection_by_node({"host": "127.0.0.1", "port": 7001})
         with pytest.raises(RedisClusterException):
             pool.get_connection_by_node({"host": "127.0.0.1", "port": 7000})
 
     def test_max_connections_default_setting(self):
         pool = self.get_pool(max_connections=None)
-        assert pool.max_connections == 2 ** 31
+        assert pool.max_connections == 2**31
 
     def test_reuse_previously_released_connection(self):
         pool = self.get_pool()
         c1 = pool.get_connection_by_node({"host": "127.0.0.1", "port": 7000})
         pool.release(c1)
         c2 = pool.get_connection_by_node({"host": "127.0.0.1", "port": 7000})
         assert c1 == c2
 
     def test_repr_contains_db_info_tcp(self):
         """
         Note: init_slot_cache must be set to false otherwise it will try to
               query the test server for data and then it can't be predicted reliably
         """
         connection_kwargs = {
-            'host': 'localhost',
-            'port': 7000,
-            'db': 1,
-            'client_name': 'test-client'
-        }
-        pool = self.get_pool(connection_kwargs=connection_kwargs,
-                             connection_class=ClusterConnection,
-                             init_slot_cache=False)
-        expected = 'ClusterConnectionPool<ClusterConnection<host=localhost,port=7000,db=1,client_name=test-client>>'
+            "host": "localhost",
+            "port": 7000,
+            "db": 1,
+            "client_name": "test-client",
+        }
+        pool = self.get_pool(
+            connection_kwargs=connection_kwargs,
+            connection_class=ClusterConnection,
+            init_slot_cache=False,
+        )
+        expected = "ClusterConnectionPool<ClusterConnection<host=localhost,port=7000,db=1,client_name=test-client>>"
         assert repr(pool) == expected
 
     def test_repr_contains_db_info_unix(self):
         """
         Note: init_slot_cache must be set to false otherwise it will try to
               query the test server for data and then it can't be predicted reliably
         """
-        connection_kwargs = {
-            'path': '/abc',
-            'db': 1,
-            'client_name': 'test-client'
-        }
-        pool = self.get_pool(connection_kwargs=connection_kwargs,
-                             connection_class=UnixDomainSocketConnection,
-                             init_slot_cache=False)
-        expected = 'ClusterConnectionPool<UnixDomainSocketConnection<path=/abc,db=1,client_name=test-client>>'
+        connection_kwargs = {"path": "/abc", "db": 1, "client_name": "test-client"}
+        pool = self.get_pool(
+            connection_kwargs=connection_kwargs,
+            connection_class=UnixDomainSocketConnection,
+            init_slot_cache=False,
+        )
+        expected = "ClusterConnectionPool<UnixDomainSocketConnection<path=/abc,db=1,client_name=test-client>>"
         assert repr(pool) == expected
 
     def test_get_connection_by_key(self):
         """
         This test assumes that when hashing key 'foo' will be sent to server with port 7002
         """
         pool = self.get_pool(connection_kwargs={})
 
         # Patch the call that is made inside the method to allow control of the returned connection object
-        with patch.object(ClusterConnectionPool, 'get_connection_by_slot', autospec=True) as pool_mock:
+        with patch.object(
+            ClusterConnectionPool, "get_connection_by_slot", autospec=True
+        ) as pool_mock:
+
             def side_effect(self, *args, **kwargs):
                 return DummyConnection(port=1337)
+
             pool_mock.side_effect = side_effect
 
-            connection = pool.get_connection_by_key("foo", 'GET')
+            connection = pool.get_connection_by_key("foo", "GET")
             assert connection.port == 1337
 
         with pytest.raises(RedisClusterException) as ex:
             pool.get_connection_by_key(None, None)
-        assert unicode(ex.value).startswith("No way to dispatch this command to Redis Cluster."), True
+        assert unicode(ex.value).startswith(
+            "No way to dispatch this command to Redis Cluster."
+        ), True
 
     def test_get_connection_by_slot(self):
         """
         This test assumes that when doing keyslot operation on "foo" it will return 12182
         """
         pool = self.get_pool(connection_kwargs={})
 
         # Patch the call that is made inside the method to allow control of the returned connection object
-        with patch.object(ClusterConnectionPool, 'get_connection_by_node', autospec=True) as pool_mock:
+        with patch.object(
+            ClusterConnectionPool, "get_connection_by_node", autospec=True
+        ) as pool_mock:
+
             def side_effect(self, *args, **kwargs):
                 return DummyConnection(port=1337)
+
             pool_mock.side_effect = side_effect
 
             connection = pool.get_connection_by_slot(12182)
             assert connection.port == 1337
 
         m = Mock()
         pool.get_random_connection = m
@@ -191,67 +219,80 @@
         Currently get_connection() should only be used by pubsub command.
         All other commands should be blocked and exception raised.
         """
         pool = self.get_pool()
 
         with pytest.raises(RedisClusterException) as ex:
             pool.get_connection("GET")
-        assert unicode(ex.value).startswith("Only 'pubsub' commands can be used by get_connection()")
+        assert unicode(ex.value).startswith(
+            "Only 'pubsub' commands can be used by get_connection()"
+        )
 
     def test_master_node_by_slot(self):
         pool = self.get_pool(connection_kwargs={})
         node = pool.get_master_node_by_slot(0)
-        node['port'] = 7000
+        node["port"] = 7000
         node = pool.get_master_node_by_slot(12182)
-        node['port'] = 7002
+        node["port"] = 7002
 
         pool = self.get_pool(connection_kwargs={})
         pool.nodes.slots = {}
         with pytest.raises(SlotNotCoveredError):
             pool.get_master_node_by_slot(12182)
 
     def test_from_url_connection_classes(self):
-        from rediscluster.client import RedisCluster
-        from rediscluster.connection import ClusterConnectionPool, ClusterConnection, SSLClusterConnection
+        from custard.redisclusterclient import RedisCluster
+        from custard.redisclusterconnection import (
+            ClusterConnectionPool,
+            ClusterConnection,
+            SSLClusterConnection,
+        )
 
-        r = RedisCluster.from_url('redis://localhost:7000')
+        r = RedisCluster.from_url("redis://localhost:7000")
         assert isinstance(r.connection_pool, ClusterConnectionPool)
         # connection_class is not an object but a ref to the class
         assert r.connection_pool.connection_class == ClusterConnection
 
-        r = RedisCluster.from_url('rediss://localhost:7000')
+        r = RedisCluster.from_url("rediss://localhost:7000")
         assert isinstance(r.connection_pool, ClusterConnectionPool)
         assert r.connection_pool.connection_class == SSLClusterConnection
 
         # Unix socket connections do not work in cluster environment
         with pytest.raises(RedisClusterException):
-            r = RedisCluster.from_url('unix://foobar@/tmp/random.sock')
+            r = RedisCluster.from_url("unix://foobar@/tmp/random.sock")
 
 
 class TestClusterBlockingConnectionPool(object):
-    def get_pool(self, connection_kwargs=None, max_connections=100, max_connections_per_node=None,
-                 connection_class=DummyConnection, init_slot_cache=True, timeout=20):
-        '''
+    def get_pool(
+        self,
+        connection_kwargs=None,
+        max_connections=100,
+        max_connections_per_node=None,
+        connection_class=DummyConnection,
+        init_slot_cache=True,
+        timeout=20,
+    ):
+        """
         Setting max_connections default to 100 instead of None (which === 2**31) like in ClusterConnectionPool as
         BlockingClusterConnectionPool takes time to setup a queue containing max_connections num of elements
-        '''
+        """
         connection_kwargs = connection_kwargs or {}
         pool = ClusterBlockingConnectionPool(
             startup_nodes=[{"host": "127.0.0.1", "port": 7000}],
             init_slot_cache=init_slot_cache,
             connection_class=connection_class,
             max_connections=max_connections,
             max_connections_per_node=max_connections_per_node,
             timeout=timeout,
             **connection_kwargs
         )
         return pool
 
     def test_connection_creation(self):
-        connection_kwargs = {'foo': 'bar', 'biz': 'baz'}
+        connection_kwargs = {"foo": "bar", "biz": "baz"}
         pool = self.get_pool(connection_kwargs=connection_kwargs)
         connection = pool.get_connection_by_node({"host": "127.0.0.1", "port": 7000})
         assert isinstance(connection, DummyConnection)
         assert connection.kwargs == connection_kwargs
 
     def test_multiple_connections(self):
         pool = self.get_pool()
@@ -268,15 +309,17 @@
         with pytest.raises(redis.ConnectionError):
             pool.get_connection("pubsub")
         # we should have waited at least 0.1 seconds
         assert time.time() - start >= 0.1
 
     def test_max_per_node_connection_pool_blocks_until_timeout(self):
         "When out of connections, block for timeout seconds, then raise"
-        pool = self.get_pool(max_connections=1, max_connections_per_node=True, timeout=0.1)
+        pool = self.get_pool(
+            max_connections=1, max_connections_per_node=True, timeout=0.1
+        )
         pool.get_connection_by_node({"host": "127.0.0.1", "port": 7000})
 
         start = time.time()
         with pytest.raises(redis.ConnectionError):
             pool.get_connection_by_node({"host": "127.0.0.1", "port": 7000})
         # we should have waited at least 0.1 seconds
         assert time.time() - start >= 0.1
@@ -303,20 +346,24 @@
             pool.release(c1)
 
         Thread(target=target).start()
         start = time.time()
         pool.get_connection_by_node({"host": "127.0.0.1", "port": 7000})
         assert time.time() - start >= 0.1
 
-    def test_max_per_node_connection_pool_blocks_until_another_connection_released(self):
+    def test_max_per_node_connection_pool_blocks_until_another_connection_released(
+        self,
+    ):
         """
         When out of connections, block until another connection is released
         to the pool
         """
-        pool = self.get_pool(max_connections=1, max_connections_per_node=True, timeout=2)
+        pool = self.get_pool(
+            max_connections=1, max_connections_per_node=True, timeout=2
+        )
         c1 = pool.get_connection_by_node({"host": "127.0.0.1", "port": 7000})
 
         def release_connection_after_sleep(connection):
             time.sleep(0.1)
             pool.release(connection)
 
         Thread(target=release_connection_after_sleep, args=(c1,)).start()
@@ -333,15 +380,17 @@
         start = time.time()
         pool.get_connection_by_node({"host": "127.0.0.1", "port": 7001})
         assert time.time() - start >= 0.1
 
     def test_reuse_previously_released_connection(self):
         # Test that behaviour for re-use is the same whatever metric we block on.
         def reuse_previously_released_connections_test(enable_max_connections_per_node):
-            pool = self.get_pool(max_connections_per_node=enable_max_connections_per_node)
+            pool = self.get_pool(
+                max_connections_per_node=enable_max_connections_per_node
+            )
             c1 = pool.get_connection_by_node({"host": "127.0.0.1", "port": 7000})
             pool.release(c1)
 
             # release c2 back in and make sure c3 still picks the connection with the correct node
             c2 = pool.get_connection_by_node({"host": "127.0.0.1", "port": 7001})
             pool.release(c2)
 
@@ -353,57 +402,65 @@
             assert c1 == c3
             assert c2 == c4
 
             # check that re-use policy is not naive
             assert c5 != c1  # also expresses that c5 does not equal c3
 
         reuse_previously_released_connections_test(enable_max_connections_per_node=True)
-        reuse_previously_released_connections_test(enable_max_connections_per_node=False)
+        reuse_previously_released_connections_test(
+            enable_max_connections_per_node=False
+        )
 
     def test_repr_contains_db_info_tcp(self):
         """
         Note: init_slot_cache must be set to false otherwise it will try to
               query the test server for data and then it can't be predicted reliably
         """
         connection_kwargs = {
-            'host': 'localhost',
-            'port': 7000,
-            'db': 0,
-            'client_name': 'test-client'
+            "host": "localhost",
+            "port": 7000,
+            "db": 0,
+            "client_name": "test-client",
         }
         pool = self.get_pool(
             connection_kwargs=connection_kwargs,
             connection_class=ClusterConnection,
             init_slot_cache=False,
         )
-        expected = 'ClusterBlockingConnectionPool<ClusterConnection<host=localhost,port=7000,db=0,client_name=test-client>>'
+        expected = "ClusterBlockingConnectionPool<ClusterConnection<host=localhost,port=7000,db=0,client_name=test-client>>"
         assert repr(pool) == expected
 
     def test_repr_contains_db_info_unix(self):
         """
         Note: init_slot_cache must be set to false otherwise it will try to
               query the test server for data and then it can't be predicted reliably
         """
         connection_kwargs = {
-            'path': '/abc',
-            'db': 1,
-            'client_name': 'test-client',
+            "path": "/abc",
+            "db": 1,
+            "client_name": "test-client",
         }
         pool = self.get_pool(
             connection_kwargs=connection_kwargs,
             connection_class=UnixDomainSocketConnection,
             init_slot_cache=False,
         )
-        expected = 'ClusterBlockingConnectionPool<UnixDomainSocketConnection<path=/abc,db=1,client_name=test-client>>'
+        expected = "ClusterBlockingConnectionPool<UnixDomainSocketConnection<path=/abc,db=1,client_name=test-client>>"
         assert repr(pool) == expected
 
 
 class TestReadOnlyConnectionPool(object):
-    def get_pool(self, connection_kwargs=None, max_connections=None, init_slot_cache=True, startup_nodes=None):
-        startup_nodes = startup_nodes or [{'host': '127.0.0.1', 'port': 7000}]
+    def get_pool(
+        self,
+        connection_kwargs=None,
+        max_connections=None,
+        init_slot_cache=True,
+        startup_nodes=None,
+    ):
+        startup_nodes = startup_nodes or [{"host": "127.0.0.1", "port": 7000}]
         connection_kwargs = connection_kwargs or {}
         pool = ClusterReadOnlyConnectionPool(
             init_slot_cache=init_slot_cache,
             max_connections=max_connections,
             startup_nodes=startup_nodes,
             **connection_kwargs
         )
@@ -412,434 +469,468 @@
     @pytest.mark.xfail(reason="Broken, needs repair")
     def test_repr_contains_db_info_readonly(self):
         """
         Note: init_slot_cache must be set to false otherwise it will try to
               query the test server for data and then it can't be predicted reliably
         """
         connection_kwargs = {
-            'db': 0,
+            "db": 0,
         }
         pool = self.get_pool(
             connection_kwargs=connection_kwargs,
             init_slot_cache=False,
             startup_nodes=[
                 {"host": "127.0.0.1", "port": 7000},
                 {"host": "127.0.0.2", "port": 7001},
             ],
         )
-        expected = 'ClusterReadOnlyConnectionPool<ClusterConnection<host=127.0.0.1,port=7000>, ClusterConnection<host=127.0.0.2,port=7001>>'
+        expected = "ClusterReadOnlyConnectionPool<ClusterConnection<host=127.0.0.1,port=7000>, ClusterConnection<host=127.0.0.2,port=7001>>"
         assert repr(pool) == expected
 
     def test_max_connections(self):
         pool = self.get_pool(max_connections=2)
         pool.get_connection_by_node({"host": "127.0.0.1", "port": 7000})
         pool.get_connection_by_node({"host": "127.0.0.1", "port": 7001})
         with pytest.raises(RedisClusterException):
             pool.get_connection_by_node({"host": "127.0.0.1", "port": 7000})
 
     def test_get_connection_by_slot(self):
-        """
-        """
+        """ """
         pool = self.get_pool(connection_kwargs={})
 
         # Patch the call that is made inside the method to allow control of the returned connection object
-        with patch.object(ClusterReadOnlyConnectionPool, 'get_master_connection_by_slot', autospec=True) as pool_mock:
+        with patch.object(
+            ClusterReadOnlyConnectionPool,
+            "get_master_connection_by_slot",
+            autospec=True,
+        ) as pool_mock:
+
             def side_effect(self, *args, **kwargs):
                 return DummyConnection(port=1337)
+
             pool_mock.side_effect = side_effect
 
             # Try a master only command
-            connection = pool.get_connection_by_key("foo", 'ZSCAN')
+            connection = pool.get_connection_by_key("foo", "ZSCAN")
             assert connection.port == 1337
 
-        with patch.object(ClusterReadOnlyConnectionPool, 'get_random_master_slave_connection_by_slot', autospec=True) as pool_mock:
+        with patch.object(
+            ClusterReadOnlyConnectionPool,
+            "get_random_master_slave_connection_by_slot",
+            autospec=True,
+        ) as pool_mock:
+
             def side_effect(self, *args, **kwargs):
                 return DummyConnection(port=1337)
+
             pool_mock.side_effect = side_effect
 
             # try a random node command
-            connection = pool.get_connection_by_key('foo', 'GET')
+            connection = pool.get_connection_by_key("foo", "GET")
             assert connection.port == 1337
 
         with pytest.raises(RedisClusterException) as ex:
             pool.get_connection_by_key(None, None)
-        assert unicode(ex.value).startswith("No way to dispatch this command to Redis Cluster."), True
+        assert unicode(ex.value).startswith(
+            "No way to dispatch this command to Redis Cluster."
+        ), True
 
     def test_get_node_by_slot_random(self):
         """
         We can randomly get all nodes in readonly mode.
         """
         pool = self.get_pool(connection_kwargs={})
 
         # Set the values that we expect to be set for the NodeManager. Represents 2 nodes for 1 specific slot
         pool.nodes.slots[0] = [
-            {'host': '172.20.0.2', 'port': 7000, 'name': '172.20.0.2:7000', 'server_type': 'master'},
-            {'host': '172.20.0.2', 'port': 7003, 'name': '172.20.0.2:7003', 'server_type': 'slave'},
+            {
+                "host": "172.20.0.2",
+                "port": 7000,
+                "name": "172.20.0.2:7000",
+                "server_type": "master",
+            },
+            {
+                "host": "172.20.0.2",
+                "port": 7003,
+                "name": "172.20.0.2:7003",
+                "server_type": "slave",
+            },
         ]
 
         expected_ports = {7000, 7003}
         actual_ports = set()
         for _ in range(0, 100):
             node = pool.get_node_by_slot_random(0)
-            actual_ports.add(node['port'])
+            actual_ports.add(node["port"])
         assert actual_ports == expected_ports
 
 
-@pytest.mark.xfail(reason="Blocking connection pool is not supported in this cluster client")
+@pytest.mark.xfail(
+    reason="Blocking connection pool is not supported in this cluster client"
+)
 class TestBlockingConnectionPool(object):
     def get_pool(self, connection_kwargs=None, max_connections=10, timeout=20):
         connection_kwargs = connection_kwargs or {}
         pool = redis.BlockingConnectionPool(
             connection_class=DummyConnection,
             max_connections=max_connections,
             timeout=timeout,
             **connection_kwargs
         )
         return pool
 
     def test_connection_creation(self):
-        connection_kwargs = {'foo': 'bar', 'biz': 'baz'}
+        connection_kwargs = {"foo": "bar", "biz": "baz"}
         pool = self.get_pool(connection_kwargs=connection_kwargs)
-        connection = pool.get_connection('_')
+        connection = pool.get_connection("_")
         assert isinstance(connection, DummyConnection)
         assert connection.kwargs == connection_kwargs
 
     def test_multiple_connections(self):
         pool = self.get_pool()
-        c1 = pool.get_connection('_')
-        c2 = pool.get_connection('_')
+        c1 = pool.get_connection("_")
+        c2 = pool.get_connection("_")
         assert c1 != c2
 
     def test_connection_pool_blocks_until_timeout(self):
         "When out of connections, block for timeout seconds, then raise"
         pool = self.get_pool(max_connections=1, timeout=0.1)
-        pool.get_connection('_')
+        pool.get_connection("_")
 
         start = time.time()
         with pytest.raises(redis.ConnectionError):
-            pool.get_connection('_')
+            pool.get_connection("_")
         # we should have waited at least 0.1 seconds
         assert time.time() - start >= 0.1
 
     def connection_pool_blocks_until_another_connection_released(self):
         """
         When out of connections, block until another connection is released
         to the pool
         """
         pool = self.get_pool(max_connections=1, timeout=2)
-        c1 = pool.get_connection('_')
+        c1 = pool.get_connection("_")
 
         def target():
             time.sleep(0.1)
             pool.release(c1)
 
         Thread(target=target).start()
         start = time.time()
-        pool.get_connection('_')
+        pool.get_connection("_")
         assert time.time() - start >= 0.1
 
     def test_reuse_previously_released_connection(self):
         pool = self.get_pool()
-        c1 = pool.get_connection('_')
+        c1 = pool.get_connection("_")
         pool.release(c1)
-        c2 = pool.get_connection('_')
+        c2 = pool.get_connection("_")
         assert c1 == c2
 
     def test_repr_contains_db_info_tcp(self):
-        pool = redis.ConnectionPool(host='localhost', port=6379, db=0)
-        expected = 'ConnectionPool<Connection<host=localhost,port=6379,db=0>>'
+        pool = redis.ConnectionPool(host="localhost", port=6379, db=0)
+        expected = "ConnectionPool<Connection<host=localhost,port=6379,db=0>>"
         assert repr(pool) == expected
 
     def test_repr_contains_db_info_unix(self):
         pool = redis.ConnectionPool(
             connection_class=redis.UnixDomainSocketConnection,
-            path='abc',
+            path="abc",
             db=0,
         )
-        expected = 'ConnectionPool<UnixDomainSocketConnection<path=abc,db=0>>'
+        expected = "ConnectionPool<UnixDomainSocketConnection<path=abc,db=0>>"
         assert repr(pool) == expected
 
 
 class TestConnectionPoolURLParsing(object):
     def test_defaults(self):
-        pool = redis.ConnectionPool.from_url('redis://localhost')
+        pool = redis.ConnectionPool.from_url("redis://localhost")
         assert pool.connection_class == redis.Connection
         assert pool.connection_kwargs == {
-            'host': 'localhost',
-            'port': 6379,
-            'db': 0,
-            'username': None,
-            'password': None,
+            "host": "localhost",
+            "port": 6379,
+            "db": 0,
+            "username": None,
+            "password": None,
         }
 
     def test_hostname(self):
-        pool = redis.ConnectionPool.from_url('redis://myhost')
+        pool = redis.ConnectionPool.from_url("redis://myhost")
         assert pool.connection_class == redis.Connection
         assert pool.connection_kwargs == {
-            'host': 'myhost',
-            'port': 6379,
-            'db': 0,
-            'username': None,
-            'password': None,
+            "host": "myhost",
+            "port": 6379,
+            "db": 0,
+            "username": None,
+            "password": None,
         }
 
     def test_quoted_hostname(self):
-        pool = redis.ConnectionPool.from_url('redis://my %2F host %2B%3D+',
-                                             decode_components=True)
+        pool = redis.ConnectionPool.from_url(
+            "redis://my %2F host %2B%3D+", decode_components=True
+        )
         assert pool.connection_class == redis.Connection
         assert pool.connection_kwargs == {
-            'host': 'my / host +=+',
-            'port': 6379,
-            'db': 0,
-            'username': None,
-            'password': None,
+            "host": "my / host +=+",
+            "port": 6379,
+            "db": 0,
+            "username": None,
+            "password": None,
         }
 
     def test_port(self):
-        pool = redis.ConnectionPool.from_url('redis://localhost:6380')
+        pool = redis.ConnectionPool.from_url("redis://localhost:6380")
         assert pool.connection_class == redis.Connection
         assert pool.connection_kwargs == {
-            'host': 'localhost',
-            'port': 6380,
-            'db': 0,
-            'username': None,
-            'password': None,
+            "host": "localhost",
+            "port": 6380,
+            "db": 0,
+            "username": None,
+            "password": None,
         }
 
     def test_password(self):
-        pool = redis.ConnectionPool.from_url('redis://:mypassword@localhost')
+        pool = redis.ConnectionPool.from_url("redis://:mypassword@localhost")
         assert pool.connection_class == redis.Connection
         assert pool.connection_kwargs == {
-            'host': 'localhost',
-            'port': 6379,
-            'db': 0,
-            'username': None,
-            'password': 'mypassword',
+            "host": "localhost",
+            "port": 6379,
+            "db": 0,
+            "username": None,
+            "password": "mypassword",
         }
 
     def test_quoted_password(self):
         pool = redis.ConnectionPool.from_url(
-            'redis://:%2Fmypass%2F%2B word%3D%24+@localhost',
-            decode_components=True)
+            "redis://:%2Fmypass%2F%2B word%3D%24+@localhost", decode_components=True
+        )
         assert pool.connection_class == redis.Connection
         assert pool.connection_kwargs == {
-            'host': 'localhost',
-            'port': 6379,
-            'db': 0,
-            'username': None,
-            'password': '/mypass/+ word=$+',
+            "host": "localhost",
+            "port": 6379,
+            "db": 0,
+            "username": None,
+            "password": "/mypass/+ word=$+",
         }
 
     def test_quoted_path(self):
         pool = redis.ConnectionPool.from_url(
-            'unix://:mypassword@/my%2Fpath%2Fto%2F..%2F+_%2B%3D%24ocket',
-            decode_components=True)
+            "unix://:mypassword@/my%2Fpath%2Fto%2F..%2F+_%2B%3D%24ocket",
+            decode_components=True,
+        )
         assert pool.connection_class == redis.UnixDomainSocketConnection
         assert pool.connection_kwargs == {
-            'path': '/my/path/to/../+_+=$ocket',
-            'db': 0,
-            'username': None,
-            'password': 'mypassword',
+            "path": "/my/path/to/../+_+=$ocket",
+            "db": 0,
+            "username": None,
+            "password": "mypassword",
         }
 
     def test_db_as_argument(self):
-        pool = redis.ConnectionPool.from_url('redis://localhost', db='1')
+        pool = redis.ConnectionPool.from_url("redis://localhost", db="1")
         assert pool.connection_class == redis.Connection
         assert pool.connection_kwargs == {
-            'host': 'localhost',
-            'port': 6379,
-            'db': 1,
-            'username': None,
-            'password': None,
+            "host": "localhost",
+            "port": 6379,
+            "db": 1,
+            "username": None,
+            "password": None,
         }
 
     def test_db_in_path(self):
-        pool = redis.ConnectionPool.from_url('redis://localhost/2', db='1')
+        pool = redis.ConnectionPool.from_url("redis://localhost/2", db="1")
         assert pool.connection_class == redis.Connection
         assert pool.connection_kwargs == {
-            'host': 'localhost',
-            'port': 6379,
-            'db': 2,
-            'username': None,
-            'password': None,
+            "host": "localhost",
+            "port": 6379,
+            "db": 2,
+            "username": None,
+            "password": None,
         }
 
     def test_db_in_querystring(self):
-        pool = redis.ConnectionPool.from_url('redis://localhost/2?db=3',
-                                             db='1')
+        pool = redis.ConnectionPool.from_url("redis://localhost/2?db=3", db="1")
         assert pool.connection_class == redis.Connection
         assert pool.connection_kwargs == {
-            'host': 'localhost',
-            'port': 6379,
-            'db': 3,
-            'username': None,
-            'password': None,
+            "host": "localhost",
+            "port": 6379,
+            "db": 3,
+            "username": None,
+            "password": None,
         }
 
     def test_extra_typed_querystring_options(self):
         pool = redis.ConnectionPool.from_url(
-            'redis://localhost/2?socket_timeout=20&socket_connect_timeout=10'
-            '&socket_keepalive=&retry_on_timeout=Yes&max_connections=10'
+            "redis://localhost/2?socket_timeout=20&socket_connect_timeout=10"
+            "&socket_keepalive=&retry_on_timeout=Yes&max_connections=10"
         )
 
         assert pool.connection_class == redis.Connection
         assert pool.connection_kwargs == {
-            'host': 'localhost',
-            'port': 6379,
-            'db': 2,
-            'username': None,
-            'socket_timeout': 20.0,
-            'socket_connect_timeout': 10.0,
-            'retry_on_timeout': True,
-            'password': None,
+            "host": "localhost",
+            "port": 6379,
+            "db": 2,
+            "username": None,
+            "socket_timeout": 20.0,
+            "socket_connect_timeout": 10.0,
+            "retry_on_timeout": True,
+            "password": None,
         }
         assert pool.max_connections == 10
 
     def test_boolean_parsing(self):
         test_data = (
             (None, None),
-            (None, ''),
-            (False, 0), (False, '0'),
-            (False, 'f'), (False, 'F'), (False, 'False'),
-            (False, 'n'), (False, 'N'), (False, 'No'),
-            (True, 1), (True, '1'),
-            (True, 'y'), (True, 'Y'), (True, 'Yes'),
+            (None, ""),
+            (False, 0),
+            (False, "0"),
+            (False, "f"),
+            (False, "F"),
+            (False, "False"),
+            (False, "n"),
+            (False, "N"),
+            (False, "No"),
+            (True, 1),
+            (True, "1"),
+            (True, "y"),
+            (True, "Y"),
+            (True, "Yes"),
         )
 
         for expected, value in test_data:
             assert expected is to_bool(value)
 
     def test_extra_querystring_options(self):
-        pool = redis.ConnectionPool.from_url('redis://localhost?a=1&b=2')
+        pool = redis.ConnectionPool.from_url("redis://localhost?a=1&b=2")
         assert pool.connection_class == redis.Connection
         assert pool.connection_kwargs == {
-            'host': 'localhost',
-            'port': 6379,
-            'db': 0,
-            'username': None,
-            'password': None,
-            'a': '1',
-            'b': '2',
+            "host": "localhost",
+            "port": 6379,
+            "db": 0,
+            "username": None,
+            "password": None,
+            "a": "1",
+            "b": "2",
         }
 
     def test_calling_from_subclass_returns_correct_instance(self):
-        pool = redis.BlockingConnectionPool.from_url('redis://localhost')
+        pool = redis.BlockingConnectionPool.from_url("redis://localhost")
         assert isinstance(pool, redis.BlockingConnectionPool)
 
     def test_client_creates_connection_pool(self):
-        r = redis.Redis.from_url('redis://myhost')
+        r = redis.Redis.from_url("redis://myhost")
         assert r.connection_pool.connection_class == redis.Connection
         assert r.connection_pool.connection_kwargs == {
-            'host': 'myhost',
-            'port': 6379,
-            'db': 0,
-            'username': None,
-            'password': None,
+            "host": "myhost",
+            "port": 6379,
+            "db": 0,
+            "username": None,
+            "password": None,
         }
 
 
 class TestConnectionPoolUnixSocketURLParsing(object):
     """
     Unix sockets do not work with redis-cluster as it do not really provide a startup nodes
     that can be used by the client for cluster discovery.
     """
 
     @skip_for_no_cluster_impl()
     def test_defaults(self):
-        pool = redis.ConnectionPool.from_url('unix:///socket')
+        pool = redis.ConnectionPool.from_url("unix:///socket")
         assert pool.connection_class == redis.UnixDomainSocketConnection
         assert pool.connection_kwargs == {
-            'path': '/socket',
-            'db': 0,
-            'username': None,
-            'password': None,
+            "path": "/socket",
+            "db": 0,
+            "username": None,
+            "password": None,
         }
 
     @skip_for_no_cluster_impl()
     def test_password(self):
-        pool = redis.ConnectionPool.from_url('unix://:mypassword@/socket')
+        pool = redis.ConnectionPool.from_url("unix://:mypassword@/socket")
         assert pool.connection_class == redis.UnixDomainSocketConnection
         assert pool.connection_kwargs == {
-            'path': '/socket',
-            'db': 0,
-            'username': None,
-            'password': 'mypassword',
+            "path": "/socket",
+            "db": 0,
+            "username": None,
+            "password": "mypassword",
         }
 
     @skip_for_no_cluster_impl()
     def test_db_as_argument(self):
-        pool = redis.ConnectionPool.from_url('unix:///socket', db=1)
+        pool = redis.ConnectionPool.from_url("unix:///socket", db=1)
         assert pool.connection_class == redis.UnixDomainSocketConnection
         assert pool.connection_kwargs == {
-            'path': '/socket',
-            'db': 1,
-            'username': None,
-            'password': None,
+            "path": "/socket",
+            "db": 1,
+            "username": None,
+            "password": None,
         }
 
     @skip_for_no_cluster_impl()
     def test_db_in_querystring(self):
-        pool = redis.ConnectionPool.from_url('unix:///socket?db=2', db=1)
+        pool = redis.ConnectionPool.from_url("unix:///socket?db=2", db=1)
         assert pool.connection_class == redis.UnixDomainSocketConnection
         assert pool.connection_kwargs == {
-            'path': '/socket',
-            'db': 2,
-            'username': None,
-            'password': None,
+            "path": "/socket",
+            "db": 2,
+            "username": None,
+            "password": None,
         }
 
     @skip_for_no_cluster_impl()
     def test_extra_querystring_options(self):
-        pool = redis.ConnectionPool.from_url('unix:///socket?a=1&b=2')
+        pool = redis.ConnectionPool.from_url("unix:///socket?a=1&b=2")
         assert pool.connection_class == redis.UnixDomainSocketConnection
         assert pool.connection_kwargs == {
-            'path': '/socket',
-            'db': 0,
-            'username': None,
-            'password': None,
-            'a': '1',
-            'b': '2',
+            "path": "/socket",
+            "db": 0,
+            "username": None,
+            "password": None,
+            "a": "1",
+            "b": "2",
         }
 
 
 class TestSSLConnectionURLParsing(object):
     @pytest.mark.skipif(not ssl_available, reason="SSL not installed")
     def test_defaults(self):
-        pool = redis.ConnectionPool.from_url('rediss://localhost')
+        pool = redis.ConnectionPool.from_url("rediss://localhost")
         assert pool.connection_class == redis.SSLConnection
         assert pool.connection_kwargs == {
-            'host': 'localhost',
-            'port': 6379,
-            'db': 0,
-            'username': None,
-            'password': None,
+            "host": "localhost",
+            "port": 6379,
+            "db": 0,
+            "username": None,
+            "password": None,
         }
 
     @pytest.mark.skipif(not ssl_available, reason="SSL not installed")
     def test_cert_reqs_options(self):
         import ssl
 
         class DummyConnectionPool(redis.ConnectionPool):
             def get_connection(self, *args, **kwargs):
                 return self.make_connection()
 
-        pool = DummyConnectionPool.from_url('rediss://?ssl_cert_reqs=none')
-        assert pool.get_connection('_').cert_reqs == ssl.CERT_NONE
+        pool = DummyConnectionPool.from_url("rediss://?ssl_cert_reqs=none")
+        assert pool.get_connection("_").cert_reqs == ssl.CERT_NONE
 
-        pool = DummyConnectionPool.from_url('rediss://?ssl_cert_reqs=optional')
-        assert pool.get_connection('_').cert_reqs == ssl.CERT_OPTIONAL
+        pool = DummyConnectionPool.from_url("rediss://?ssl_cert_reqs=optional")
+        assert pool.get_connection("_").cert_reqs == ssl.CERT_OPTIONAL
 
-        pool = DummyConnectionPool.from_url('rediss://?ssl_cert_reqs=required')
-        assert pool.get_connection('_').cert_reqs == ssl.CERT_REQUIRED
+        pool = DummyConnectionPool.from_url("rediss://?ssl_cert_reqs=required")
+        assert pool.get_connection("_").cert_reqs == ssl.CERT_REQUIRED
 
-        pool = DummyConnectionPool.from_url('rediss://?ssl_check_hostname=False')
-        assert pool.get_connection('_').check_hostname is False
+        pool = DummyConnectionPool.from_url("rediss://?ssl_check_hostname=False")
+        assert pool.get_connection("_").check_hostname is False
 
-        pool = DummyConnectionPool.from_url('rediss://?ssl_check_hostname=True')
-        assert pool.get_connection('_').check_hostname is True
+        pool = DummyConnectionPool.from_url("rediss://?ssl_check_hostname=True")
+        assert pool.get_connection("_").check_hostname is True
 
 
 class TestConnection(object):
     def test_on_connect_error(self):
         """
         An error in Connection.on_connect should disconnect from the server
         see for details: https://github.com/andymccurdy/redis-py/issues/368
@@ -850,81 +941,82 @@
         # an error should be raised on connect
         with pytest.raises(redis.RedisError):
             bad_connection.info()
         pool = bad_connection.connection_pool
         assert len(pool._available_connections) == 1
         assert not pool._available_connections[0]._sock
 
-    @skip_if_server_version_lt('2.8.8')
+    @skip_if_server_version_lt("2.8.8")
     def test_busy_loading_disconnects_socket(self, r):
         """
         If Redis raises a LOADING error, the connection should be
         disconnected and a BusyLoadingError raised
         """
         with pytest.raises(redis.BusyLoadingError):
-            r.execute_command('DEBUG', 'ERROR', 'LOADING fake message')
+            r.execute_command("DEBUG", "ERROR", "LOADING fake message")
         # TODO: Sinc we have to query the cluster before we send this DEBUG command
         #  we will have more then 1 connection in our pool and asserting 1 connection will
         #  not work.
         pool = r.connection_pool
         assert len(pool._available_connections) >= 1
         # assert not pool._available_connections[0]._sock
 
     @pytest.mark.xfail(reason="pipeline NYI")
-    @skip_if_server_version_lt('2.8.8')
+    @skip_if_server_version_lt("2.8.8")
     def test_busy_loading_from_pipeline_immediate_command(self, r):
         """
         BusyLoadingErrors should raise from Pipelines that execute a
         command immediately, like WATCH does.
         """
         pipe = r.pipeline()
         with pytest.raises(redis.BusyLoadingError):
             pipe.immediate_execute_command(
-                'DEBUG', 'ERROR',
-                'LOADING fake message',
+                "DEBUG",
+                "ERROR",
+                "LOADING fake message",
             )
         pool = r.connection_pool
         assert not pipe.connection
         assert len(pool._available_connections) == 1
         assert not pool._available_connections[0]._sock
 
     @pytest.mark.xfail(reason="pipeline NYI")
-    @skip_if_server_version_lt('2.8.8')
+    @skip_if_server_version_lt("2.8.8")
     def test_busy_loading_from_pipeline(self, r):
         """
         BusyLoadingErrors should be raised from a pipeline execution
         regardless of the raise_on_error flag.
         """
         pipe = r.pipeline()
-        pipe.execute_command('DEBUG', 'ERROR', 'LOADING fake message')
+        pipe.execute_command("DEBUG", "ERROR", "LOADING fake message")
         with pytest.raises(redis.BusyLoadingError):
             pipe.execute()
         pool = r.connection_pool
         assert not pipe.connection
         assert len(pool._available_connections) == 1
         assert not pool._available_connections[0]._sock
 
-    @skip_if_server_version_lt('2.8.8')
+    @skip_if_server_version_lt("2.8.8")
     def test_read_only_error(self, r):
         "READONLY errors get turned in ReadOnlyError exceptions"
         with pytest.raises(redis.ReadOnlyError):
-            r.execute_command('DEBUG', 'ERROR', 'READONLY blah blah')
+            r.execute_command("DEBUG", "ERROR", "READONLY blah blah")
 
     def test_connect_from_url_tcp(self):
-        connection = redis.Redis.from_url('redis://localhost')
+        connection = redis.Redis.from_url("redis://localhost")
         pool = connection.connection_pool
 
-        assert re.match('(.*)<(.*)<(.*)>>', repr(pool)).groups() == (
-            'ConnectionPool',
-            'Connection',
-            'host=localhost,port=6379,db=0',
+        assert re.match("(.*)<(.*)<(.*)>>", repr(pool)).groups() == (
+            "ConnectionPool",
+            "Connection",
+            "host=localhost,port=6379,db=0",
         )
 
     def test_connect_from_url_unix(self):
-        connection = redis.Redis.from_url('unix:///path/to/socket')
+        connection = redis.Redis.from_url("unix:///path/to/socket")
         pool = connection.connection_pool
 
-        assert re.match('(.*)<(.*)<(.*)>>', repr(pool)).groups() == (
-            'ConnectionPool',
-            'UnixDomainSocketConnection',
-            'path=/path/to/socket,db=0',
+        assert re.match("(.*)<(.*)<(.*)>>", repr(pool)).groups() == (
+            "ConnectionPool",
+            "UnixDomainSocketConnection",
+            "path=/path/to/socket,db=0",
         )
```

### Comparing `custard-1.1.0/custard/rediscluster/tests/test_cluster_node_manager.py` & `custard-1.1.1/custard/rediscluster/tests/test_cluster_node_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,19 @@
 
 # python std lib
 from __future__ import with_statement
 
 # rediscluster imports
 from tests.conftest import skip_if_server_version_lt
 from custard.rediscluster import RedisCluster
-from rediscluster.exceptions import RedisClusterException, RedisClusterConfigError
-from rediscluster.nodemanager import NodeManager
+from custard.redisclusterexceptions import (
+    RedisClusterException,
+    RedisClusterConfigError,
+)
+from custard.redisclusternodemanager import NodeManager
 
 # 3rd party imports
 import pytest
 from mock import patch, Mock
 from redis import Redis
 from redis._compat import unicode
 from redis import ConnectionError, ResponseError
```

### Comparing `custard-1.1.0/custard/rediscluster/tests/test_cluster_obj.py` & `custard-1.1.1/custard/rediscluster/tests/test_cluster_obj.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,22 +2,25 @@
 
 # python std lib
 from __future__ import with_statement
 import re
 
 # rediscluster imports
 from custard.rediscluster import RedisCluster
-from rediscluster.connection import ClusterConnectionPool, ClusterReadOnlyConnectionPool
-from rediscluster.exceptions import (
+from custard.redisclusterconnection import (
+    ClusterConnectionPool,
+    ClusterReadOnlyConnectionPool,
+)
+from custard.redisclusterexceptions import (
     RedisClusterException,
     MovedError,
     AskError,
     ClusterDownError,
 )
-from rediscluster.nodemanager import NodeManager
+from custard.redisclusternodemanager import NodeManager
 from tests.conftest import (
     _get_client,
     skip_if_server_version_lt,
     skip_if_not_password_protected_nodes,
 )
 
 # 3rd party imports
```

### Comparing `custard-1.1.0/custard/rediscluster/tests/test_commands.py` & `custard-1.1.1/custard/rediscluster/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/rediscluster/tests/test_commands_cluster.py` & `custard-1.1.1/custard/rediscluster/tests/test_commands_cluster.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,42 +2,42 @@
 
 # python std lib
 from __future__ import unicode_literals
 import datetime
 
 # rediscluster imports
 import rediscluster
-from rediscluster.exceptions import RedisClusterException
-from rediscluster.utils import dict_merge
+from custard.redisclusterexceptions import RedisClusterException
+from custard.redisclusterutils import dict_merge
 from .conftest import (
     skip_if_server_version_lt,
     REDIS_6_VERSION,
 )
 
 # 3rd party imports
 import pytest
 from redis import exceptions
 
 
 def redis_server_time(client):
     all_clients_time = client.time()
     for server_id, server_time_data in all_clients_time.items():
-        if '7000' in server_id:
+        if "7000" in server_id:
             seconds, milliseconds = server_time_data
 
-    timestamp = float('%s.%s' % (seconds, milliseconds))
+    timestamp = float("%s.%s" % (seconds, milliseconds))
     return datetime.datetime.fromtimestamp(timestamp)
 
 
 def get_main_cluster_node_data(command_result):
     """
     Tries to find whatever node is running on port :7000 in the cluster resonse
     """
     for node_id, node_data in command_result.items():
-        if '7000' in node_id:
+        if "7000" in node_id:
             return node_data
     return None
 
 
 # RESPONSE CALLBACKS
 class TestResponseCallbacksCluster(object):
     "Tests for the response callback system"
@@ -46,415 +46,455 @@
         all_response_callbacks = dict_merge(
             rediscluster.RedisCluster.RESPONSE_CALLBACKS,
             rediscluster.RedisCluster.CLUSTER_COMMANDS_RESPONSE_CALLBACKS,
         )
 
         assert r.response_callbacks == all_response_callbacks
         assert id(r.response_callbacks) != id(all_response_callbacks)
-        r.set_response_callback('GET', lambda x: 'static')
-        r['a'] = 'foo'
-        assert r['a'] == 'static'
+        r.set_response_callback("GET", lambda x: "static")
+        r["a"] = "foo"
+        assert r["a"] == "static"
 
 
 class TestRedisCommandsCluster(object):
 
     # SERVER INFORMATION
     def test_client_list(self, r):
         clients = r.client_list()
         client_data = get_main_cluster_node_data(clients)[0]
         assert isinstance(client_data, dict)
-        assert 'addr' in client_data
+        assert "addr" in client_data
 
-    @skip_if_server_version_lt('5.0.0')
+    @skip_if_server_version_lt("5.0.0")
     def test_client_list_type(self, r):
         with pytest.raises(exceptions.RedisError):
-            r.client_list(_type='not a client type')
-        for client_type in ['normal', 'master', 'replica', 'pubsub']:
+            r.client_list(_type="not a client type")
+        for client_type in ["normal", "master", "replica", "pubsub"]:
             clients = get_main_cluster_node_data(r.client_list(_type=client_type))
             assert isinstance(clients, list)
 
-    @skip_if_server_version_lt('5.0.0')
+    @skip_if_server_version_lt("5.0.0")
     def test_client_id(self, r):
         assert get_main_cluster_node_data(r.client_id()) > 0
 
-    @skip_if_server_version_lt('5.0.0')
+    @skip_if_server_version_lt("5.0.0")
     def test_client_unblock(self, r):
         myid = get_main_cluster_node_data(r.client_id())
         assert not r.client_unblock(myid)
         assert not r.client_unblock(myid, error=True)
         assert not r.client_unblock(myid, error=False)
 
-    @skip_if_server_version_lt('2.6.9')
+    @skip_if_server_version_lt("2.6.9")
     def test_client_getname(self, r):
         assert get_main_cluster_node_data(r.client_getname()) is None
 
-    @skip_if_server_version_lt('2.6.9')
+    @skip_if_server_version_lt("2.6.9")
     def test_client_setname(self, r):
-        assert r.client_setname('redis_py_test')
-        assert get_main_cluster_node_data(r.client_getname()) == 'redis_py_test'
+        assert r.client_setname("redis_py_test")
+        assert get_main_cluster_node_data(r.client_getname()) == "redis_py_test"
 
     def test_config_get(self, r):
         data = get_main_cluster_node_data(r.config_get())
-        assert 'maxmemory' in data
-        assert data['maxmemory'].isdigit()
+        assert "maxmemory" in data
+        assert data["maxmemory"].isdigit()
 
     def test_config_resetstat(self, r):
         r.ping()
-        prior_commands_processed = int(get_main_cluster_node_data(r.info())['total_commands_processed'])
+        prior_commands_processed = int(
+            get_main_cluster_node_data(r.info())["total_commands_processed"]
+        )
         assert prior_commands_processed >= 1
         r.config_resetstat()
-        reset_commands_processed = int(get_main_cluster_node_data(r.info())['total_commands_processed'])
+        reset_commands_processed = int(
+            get_main_cluster_node_data(r.info())["total_commands_processed"]
+        )
         assert reset_commands_processed < prior_commands_processed
 
     def test_config_set(self, r):
         data = get_main_cluster_node_data(r.config_get())
-        rdbname = data['dbfilename']
+        rdbname = data["dbfilename"]
         try:
-            assert r.config_set('dbfilename', 'redis_py_test.rdb')
-            assert get_main_cluster_node_data(r.config_get())['dbfilename'] == 'redis_py_test.rdb'
+            assert r.config_set("dbfilename", "redis_py_test.rdb")
+            assert (
+                get_main_cluster_node_data(r.config_get())["dbfilename"]
+                == "redis_py_test.rdb"
+            )
         finally:
-            assert r.config_set('dbfilename', rdbname)
+            assert r.config_set("dbfilename", rdbname)
 
     def test_dbsize(self, r):
-        r['a'] = 'foo'
-        r['b'] = 'bar'
+        r["a"] = "foo"
+        r["b"] = "bar"
         # Count all commands sent to the DB. Since we have one slave
         # for every master we will look for 4 and not 2
-        dbsize_sum = sum([db_size_count for node_id, db_size_count in r.dbsize().items()])
+        dbsize_sum = sum(
+            [db_size_count for node_id, db_size_count in r.dbsize().items()]
+        )
         assert dbsize_sum == 4
 
     def test_echo(self, r):
-        assert get_main_cluster_node_data(r.echo('foo bar')) == b'foo bar'
+        assert get_main_cluster_node_data(r.echo("foo bar")) == b"foo bar"
 
     def test_info(self, r):
-        r['a'] = 'foo'
-        r['b'] = 'bar'
+        r["a"] = "foo"
+        r["b"] = "bar"
         info = get_main_cluster_node_data(r.info())
         assert isinstance(info, dict)
         # We only have a "db0" in cluster mode and only one of the commands will bind to node :7000
-        assert info['db0']['keys'] == 1
+        assert info["db0"]["keys"] == 1
         # Sum all keys in all slots
-        keys_sum = sum([node_data.get('db0', {}).get('keys', 0) for node_id, node_data in r.info().items()])
+        keys_sum = sum(
+            [
+                node_data.get("db0", {}).get("keys", 0)
+                for node_id, node_data in r.info().items()
+            ]
+        )
         assert keys_sum == 4
 
     def test_lastsave(self, r):
         assert isinstance(get_main_cluster_node_data(r.lastsave()), datetime.datetime)
 
-    @skip_if_server_version_lt('2.6.0')
+    @skip_if_server_version_lt("2.6.0")
     def test_time(self, r):
         t = get_main_cluster_node_data(r.time())
         assert len(t) == 2
         assert isinstance(t[0], int)
         assert isinstance(t[1], int)
 
     # FIXME: Move this method to a more generic solution/method that tests the blocked nodes flags feature
     def test_bitop_not_supported(self, r):
         """
         Validate that the command is blocked in cluster mode and throws an Exception
         """
-        r['a'] = ''
+        r["a"] = ""
         with pytest.raises(RedisClusterException):
-            r.bitop('not', 'r', 'a')
+            r.bitop("not", "r", "a")
 
     def test_exists(self, r):
         """
         Keys need to be in specific slots to work out
         """
-        assert r.exists('a') == 0
-        r['G0B96'] = 'foo'
-        r['TEFX5'] = 'bar'
-        assert r.exists('G0B96') == 1
-        assert r.exists('G0B96', 'TEFX5') == 2
+        assert r.exists("a") == 0
+        r["G0B96"] = "foo"
+        r["TEFX5"] = "bar"
+        assert r.exists("G0B96") == 1
+        assert r.exists("G0B96", "TEFX5") == 2
 
     def test_blpop(self, r):
         """
         Generated keys for slot
             16299: ['0J8KD', '822JO', '8TJPT', 'HD644', 'SKUCM', 'N4N5Z', 'NRSWJ']
         """
-        r.rpush('0J8KD', '1', '2')
-        r.rpush('822JO', '3', '4')
-        assert r.blpop(['822JO', '0J8KD'], timeout=1) == (b'822JO', b'3')
-        assert r.blpop(['822JO', '0J8KD'], timeout=1) == (b'822JO', b'4')
-        assert r.blpop(['822JO', '0J8KD'], timeout=1) == (b'0J8KD', b'1')
-        assert r.blpop(['822JO', '0J8KD'], timeout=1) == (b'0J8KD', b'2')
-        assert r.blpop(['822JO', '0J8KD'], timeout=1) is None
-        r.rpush('c', '1')
-        assert r.blpop('c', timeout=1) == (b'c', b'1')
+        r.rpush("0J8KD", "1", "2")
+        r.rpush("822JO", "3", "4")
+        assert r.blpop(["822JO", "0J8KD"], timeout=1) == (b"822JO", b"3")
+        assert r.blpop(["822JO", "0J8KD"], timeout=1) == (b"822JO", b"4")
+        assert r.blpop(["822JO", "0J8KD"], timeout=1) == (b"0J8KD", b"1")
+        assert r.blpop(["822JO", "0J8KD"], timeout=1) == (b"0J8KD", b"2")
+        assert r.blpop(["822JO", "0J8KD"], timeout=1) is None
+        r.rpush("c", "1")
+        assert r.blpop("c", timeout=1) == (b"c", b"1")
 
     def test_brpop(self, r):
         """
         Generated keys for slot
             16299: ['0J8KD', '822JO', '8TJPT', 'HD644', 'SKUCM', 'N4N5Z', 'NRSWJ']
         """
-        r.rpush('0J8KD', '1', '2')
-        r.rpush('822JO', '3', '4')
-        assert r.brpop(['822JO', '0J8KD'], timeout=1) == (b'822JO', b'4')
-        assert r.brpop(['822JO', '0J8KD'], timeout=1) == (b'822JO', b'3')
-        assert r.brpop(['822JO', '0J8KD'], timeout=1) == (b'0J8KD', b'2')
-        assert r.brpop(['822JO', '0J8KD'], timeout=1) == (b'0J8KD', b'1')
-        assert r.brpop(['822JO', '0J8KD'], timeout=1) is None
-        r.rpush('c', '1')
-        assert r.brpop('c', timeout=1) == (b'c', b'1')
+        r.rpush("0J8KD", "1", "2")
+        r.rpush("822JO", "3", "4")
+        assert r.brpop(["822JO", "0J8KD"], timeout=1) == (b"822JO", b"4")
+        assert r.brpop(["822JO", "0J8KD"], timeout=1) == (b"822JO", b"3")
+        assert r.brpop(["822JO", "0J8KD"], timeout=1) == (b"0J8KD", b"2")
+        assert r.brpop(["822JO", "0J8KD"], timeout=1) == (b"0J8KD", b"1")
+        assert r.brpop(["822JO", "0J8KD"], timeout=1) is None
+        r.rpush("c", "1")
+        assert r.brpop("c", timeout=1) == (b"c", b"1")
 
-    @skip_if_server_version_lt('2.8.0')
+    @skip_if_server_version_lt("2.8.0")
     def test_scan(self, r):
         """
         Test is adapted for a same slot scenario in a clustered environment.
 
         FIXME: Add test for cross slot functionality test
 
         Generated keys for slot
             0 : ['GQ5KU', 'IFWJL', 'X582D']
         """
-        r.set('GQ5KU', 1)
-        r.set('IFWJL', 2)
-        r.set('X582D', 3)
+        r.set("GQ5KU", 1)
+        r.set("IFWJL", 2)
+        r.set("X582D", 3)
         cursor, keys = get_main_cluster_node_data(r.scan())
         assert cursor == 0
-        assert set(keys) == {b'GQ5KU', b'IFWJL', b'X582D'}
-        _, keys = get_main_cluster_node_data(r.scan(match='GQ5KU'))
-        assert set(keys) == {b'GQ5KU'}
+        assert set(keys) == {b"GQ5KU", b"IFWJL", b"X582D"}
+        _, keys = get_main_cluster_node_data(r.scan(match="GQ5KU"))
+        assert set(keys) == {b"GQ5KU"}
 
     @skip_if_server_version_lt(REDIS_6_VERSION)
     def test_scan_type(self, r):
         """
         Test is adapted for a same slot scenario in a clustered environment.
 
         FIXME: Add test for cross slot functionality test
 
         Generated keys for slot
             0 : ['GQ5KU', 'IFWJL', 'X582D']
         """
-        r.sadd('GQ5KU', 1)
-        r.hset('IFWJL', 'foo', 2)
-        r.lpush('X582D', 'aux', 3)
-        _, keys = get_main_cluster_node_data(r.scan(match='G*', _type='SET'))
-        assert set(keys) == {b'GQ5KU'}
+        r.sadd("GQ5KU", 1)
+        r.hset("IFWJL", "foo", 2)
+        r.lpush("X582D", "aux", 3)
+        _, keys = get_main_cluster_node_data(r.scan(match="G*", _type="SET"))
+        assert set(keys) == {b"GQ5KU"}
 
     def test_zadd_incr_with_xx(self, r):
         """
         Generated keys for slot
             0 : ['60ZE7', '8I2EQ', 'R8H1V', 'NJP6N', '0VI0A', '0CEIC', 'MV75A', 'TMKD9']
         """
         # this asks zadd to incr 'a1' only if it exists, but it clearly
         # doesn't. Redis returns a null value in this case and so should
         # redis-py
-        assert r.zadd('a', {'a1': 1}, xx=True, incr=True) is None
+        assert r.zadd("a", {"a1": 1}, xx=True, incr=True) is None
 
     def test_zinterstore_sum(self, r):
         """
         Generated keys for slot
             0 : ['60ZE7', '8I2EQ', 'R8H1V', 'NJP6N', '0VI0A', '0CEIC', 'MV75A', 'TMKD9']
         """
-        r.zadd('60ZE7', {'a1': 1, 'a2': 1, 'a3': 1})
-        r.zadd('8I2EQ', {'a1': 2, 'a2': 2, 'a3': 2})
-        r.zadd('R8H1V', {'a1': 6, 'a3': 5, 'a4': 4})
-        assert r.zinterstore('NJP6N', ['60ZE7', '8I2EQ', 'R8H1V']) == 2
-        assert r.zrange('NJP6N', 0, -1, withscores=True) == \
-            [(b'a3', 8), (b'a1', 9)]
+        r.zadd("60ZE7", {"a1": 1, "a2": 1, "a3": 1})
+        r.zadd("8I2EQ", {"a1": 2, "a2": 2, "a3": 2})
+        r.zadd("R8H1V", {"a1": 6, "a3": 5, "a4": 4})
+        assert r.zinterstore("NJP6N", ["60ZE7", "8I2EQ", "R8H1V"]) == 2
+        assert r.zrange("NJP6N", 0, -1, withscores=True) == [(b"a3", 8), (b"a1", 9)]
 
     def test_zinterstore_max(self, r):
         """
         Generated keys for slot
             0 : ['60ZE7', '8I2EQ', 'R8H1V', 'NJP6N', '0VI0A', '0CEIC', 'MV75A', 'TMKD9']
         """
-        r.zadd('60ZE7', {'a1': 1, 'a2': 1, 'a3': 1})
-        r.zadd('8I2EQ', {'a1': 2, 'a2': 2, 'a3': 2})
-        r.zadd('R8H1V', {'a1': 6, 'a3': 5, 'a4': 4})
-        assert r.zinterstore('NJP6N', ['60ZE7', '8I2EQ', 'R8H1V'], aggregate='MAX') == 2
-        assert r.zrange('NJP6N', 0, -1, withscores=True) == \
-            [(b'a3', 5), (b'a1', 6)]
+        r.zadd("60ZE7", {"a1": 1, "a2": 1, "a3": 1})
+        r.zadd("8I2EQ", {"a1": 2, "a2": 2, "a3": 2})
+        r.zadd("R8H1V", {"a1": 6, "a3": 5, "a4": 4})
+        assert r.zinterstore("NJP6N", ["60ZE7", "8I2EQ", "R8H1V"], aggregate="MAX") == 2
+        assert r.zrange("NJP6N", 0, -1, withscores=True) == [(b"a3", 5), (b"a1", 6)]
 
     def test_zinterstore_min(self, r):
         """
         Generated keys for slot
             0 : ['60ZE7', '8I2EQ', 'R8H1V', 'NJP6N', '0VI0A', '0CEIC', 'MV75A', 'TMKD9']
         """
-        r.zadd('60ZE7', {'a1': 1, 'a2': 2, 'a3': 3})
-        r.zadd('8I2EQ', {'a1': 2, 'a2': 3, 'a3': 5})
-        r.zadd('R8H1V', {'a1': 6, 'a3': 5, 'a4': 4})
-        assert r.zinterstore('NJP6N', ['60ZE7', '8I2EQ', 'R8H1V'], aggregate='MIN') == 2
-        assert r.zrange('NJP6N', 0, -1, withscores=True) == \
-            [(b'a1', 1), (b'a3', 3)]
+        r.zadd("60ZE7", {"a1": 1, "a2": 2, "a3": 3})
+        r.zadd("8I2EQ", {"a1": 2, "a2": 3, "a3": 5})
+        r.zadd("R8H1V", {"a1": 6, "a3": 5, "a4": 4})
+        assert r.zinterstore("NJP6N", ["60ZE7", "8I2EQ", "R8H1V"], aggregate="MIN") == 2
+        assert r.zrange("NJP6N", 0, -1, withscores=True) == [(b"a1", 1), (b"a3", 3)]
 
     def test_zinterstore_with_weight(self, r):
         """
         Generated keys for slot
             0 : ['60ZE7', '8I2EQ', 'R8H1V', 'NJP6N', '0VI0A', '0CEIC', 'MV75A', 'TMKD9']
         """
-        r.zadd('60ZE7', {'a1': 1, 'a2': 1, 'a3': 1})
-        r.zadd('8I2EQ', {'a1': 2, 'a2': 2, 'a3': 2})
-        r.zadd('R8H1V', {'a1': 6, 'a3': 5, 'a4': 4})
-        assert r.zinterstore('NJP6N', {'60ZE7': 1, '8I2EQ': 2, 'R8H1V': 3}) == 2
-        assert r.zrange('NJP6N', 0, -1, withscores=True) == \
-            [(b'a3', 20), (b'a1', 23)]
+        r.zadd("60ZE7", {"a1": 1, "a2": 1, "a3": 1})
+        r.zadd("8I2EQ", {"a1": 2, "a2": 2, "a3": 2})
+        r.zadd("R8H1V", {"a1": 6, "a3": 5, "a4": 4})
+        assert r.zinterstore("NJP6N", {"60ZE7": 1, "8I2EQ": 2, "R8H1V": 3}) == 2
+        assert r.zrange("NJP6N", 0, -1, withscores=True) == [(b"a3", 20), (b"a1", 23)]
 
-    @skip_if_server_version_lt('4.9.0')
+    @skip_if_server_version_lt("4.9.0")
     def test_zpopmax(self, r):
         """
         Generated keys for slot
             0 : ['60ZE7', '8I2EQ', 'R8H1V', 'NJP6N', '0VI0A', '0CEIC', 'MV75A', 'TMKD9']
         """
-        r.zadd('60ZE7', {'a1': 1, 'a2': 2, 'a3': 3})
-        assert r.zpopmax('60ZE7') == [(b'a3', 3)]
+        r.zadd("60ZE7", {"a1": 1, "a2": 2, "a3": 3})
+        assert r.zpopmax("60ZE7") == [(b"a3", 3)]
 
         # with count
-        assert r.zpopmax('60ZE7', count=2) == \
-            [(b'a2', 2), (b'a1', 1)]
+        assert r.zpopmax("60ZE7", count=2) == [(b"a2", 2), (b"a1", 1)]
 
-    @skip_if_server_version_lt('4.9.0')
+    @skip_if_server_version_lt("4.9.0")
     def test_zpopmin(self, r):
         """
         Generated keys for slot
             0 : ['60ZE7', '8I2EQ', 'R8H1V', 'NJP6N', '0VI0A', '0CEIC', 'MV75A', 'TMKD9']
         """
-        r.zadd('60ZE7', {'a1': 1, 'a2': 2, 'a3': 3})
-        assert r.zpopmin('60ZE7') == [(b'a1', 1)]
+        r.zadd("60ZE7", {"a1": 1, "a2": 2, "a3": 3})
+        assert r.zpopmin("60ZE7") == [(b"a1", 1)]
 
         # with count
-        assert r.zpopmin('60ZE7', count=2) == \
-            [(b'a2', 2), (b'a3', 3)]
+        assert r.zpopmin("60ZE7", count=2) == [(b"a2", 2), (b"a3", 3)]
 
     def test_zunionstore_sum(self, r):
         """
         Generated keys for slot
             0 : ['60ZE7', '8I2EQ', 'R8H1V', 'NJP6N', '0VI0A', '0CEIC', 'MV75A', 'TMKD9']
         """
-        r.zadd('60ZE7', {'a1': 1, 'a2': 1, 'a3': 1})
-        r.zadd('8I2EQ', {'a1': 2, 'a2': 2, 'a3': 2})
-        r.zadd('R8H1V', {'a1': 6, 'a3': 5, 'a4': 4})
-        assert r.zunionstore('NJP6N', ['60ZE7', '8I2EQ', 'R8H1V']) == 4
-        assert r.zrange('NJP6N', 0, -1, withscores=True) == \
-            [(b'a2', 3), (b'a4', 4), (b'a3', 8), (b'a1', 9)]
+        r.zadd("60ZE7", {"a1": 1, "a2": 1, "a3": 1})
+        r.zadd("8I2EQ", {"a1": 2, "a2": 2, "a3": 2})
+        r.zadd("R8H1V", {"a1": 6, "a3": 5, "a4": 4})
+        assert r.zunionstore("NJP6N", ["60ZE7", "8I2EQ", "R8H1V"]) == 4
+        assert r.zrange("NJP6N", 0, -1, withscores=True) == [
+            (b"a2", 3),
+            (b"a4", 4),
+            (b"a3", 8),
+            (b"a1", 9),
+        ]
 
     def test_zunionstore_max(self, r):
         """
         Generated keys for slot
             0 : ['60ZE7', '8I2EQ', 'R8H1V', 'NJP6N', '0VI0A', '0CEIC', 'MV75A', 'TMKD9']
         """
-        r.zadd('60ZE7', {'a1': 1, 'a2': 1, 'a3': 1})
-        r.zadd('8I2EQ', {'a1': 2, 'a2': 2, 'a3': 2})
-        r.zadd('R8H1V', {'a1': 6, 'a3': 5, 'a4': 4})
-        assert r.zunionstore('NJP6N', ['60ZE7', '8I2EQ', 'R8H1V'], aggregate='MAX') == 4
-        assert r.zrange('NJP6N', 0, -1, withscores=True) == \
-            [(b'a2', 2), (b'a4', 4), (b'a3', 5), (b'a1', 6)]
+        r.zadd("60ZE7", {"a1": 1, "a2": 1, "a3": 1})
+        r.zadd("8I2EQ", {"a1": 2, "a2": 2, "a3": 2})
+        r.zadd("R8H1V", {"a1": 6, "a3": 5, "a4": 4})
+        assert r.zunionstore("NJP6N", ["60ZE7", "8I2EQ", "R8H1V"], aggregate="MAX") == 4
+        assert r.zrange("NJP6N", 0, -1, withscores=True) == [
+            (b"a2", 2),
+            (b"a4", 4),
+            (b"a3", 5),
+            (b"a1", 6),
+        ]
 
     def test_zunionstore_min(self, r):
         """
         Generated keys for slot
             0 : ['60ZE7', '8I2EQ', 'R8H1V', 'NJP6N', '0VI0A', '0CEIC', 'MV75A', 'TMKD9']
         """
-        r.zadd('60ZE7', {'a1': 1, 'a2': 2, 'a3': 3})
-        r.zadd('8I2EQ', {'a1': 2, 'a2': 2, 'a3': 4})
-        r.zadd('R8H1V', {'a1': 6, 'a3': 5, 'a4': 4})
-        assert r.zunionstore('NJP6N', ['60ZE7', '8I2EQ', 'R8H1V'], aggregate='MIN') == 4
-        assert r.zrange('NJP6N', 0, -1, withscores=True) == \
-            [(b'a1', 1), (b'a2', 2), (b'a3', 3), (b'a4', 4)]
+        r.zadd("60ZE7", {"a1": 1, "a2": 2, "a3": 3})
+        r.zadd("8I2EQ", {"a1": 2, "a2": 2, "a3": 4})
+        r.zadd("R8H1V", {"a1": 6, "a3": 5, "a4": 4})
+        assert r.zunionstore("NJP6N", ["60ZE7", "8I2EQ", "R8H1V"], aggregate="MIN") == 4
+        assert r.zrange("NJP6N", 0, -1, withscores=True) == [
+            (b"a1", 1),
+            (b"a2", 2),
+            (b"a3", 3),
+            (b"a4", 4),
+        ]
 
     def test_zunionstore_with_weight(self, r):
         """
         Generated keys for slot
             0 : ['60ZE7', '8I2EQ', 'R8H1V', 'NJP6N', '0VI0A', '0CEIC', 'MV75A', 'TMKD9']
         """
-        r.zadd('60ZE7', {'a1': 1, 'a2': 1, 'a3': 1})
-        r.zadd('8I2EQ', {'a1': 2, 'a2': 2, 'a3': 2})
-        r.zadd('R8H1V', {'a1': 6, 'a3': 5, 'a4': 4})
-        assert r.zunionstore('NJP6N', {'60ZE7': 1, '8I2EQ': 2, 'R8H1V': 3}) == 4
-        assert r.zrange('NJP6N', 0, -1, withscores=True) == \
-            [(b'a2', 5), (b'a4', 12), (b'a3', 20), (b'a1', 23)]
+        r.zadd("60ZE7", {"a1": 1, "a2": 1, "a3": 1})
+        r.zadd("8I2EQ", {"a1": 2, "a2": 2, "a3": 2})
+        r.zadd("R8H1V", {"a1": 6, "a3": 5, "a4": 4})
+        assert r.zunionstore("NJP6N", {"60ZE7": 1, "8I2EQ": 2, "R8H1V": 3}) == 4
+        assert r.zrange("NJP6N", 0, -1, withscores=True) == [
+            (b"a2", 5),
+            (b"a4", 12),
+            (b"a3", 20),
+            (b"a1", 23),
+        ]
 
     def test_hmset(self, r):
         """
         Warning message is different in a RedisCluster instance
         """
-        warning_message = (r'^RedisCluster\.hmset\(\) is deprecated\. '
-                           r'Use RedisCluster\.hset\(\) instead\.$')
-        h = {b'a': b'1', b'b': b'2', b'c': b'3'}
+        warning_message = (
+            r"^RedisCluster\.hmset\(\) is deprecated\. "
+            r"Use RedisCluster\.hset\(\) instead\.$"
+        )
+        h = {b"a": b"1", b"b": b"2", b"c": b"3"}
         with pytest.warns(DeprecationWarning, match=warning_message):
-            assert r.hmset('a', h)
-        assert r.hgetall('a') == h
+            assert r.hmset("a", h)
+        assert r.hgetall("a") == h
 
     def test_sort_store(self, r):
         """
         Generated keys for slot
             0 : ['60ZE7', '8I2EQ', 'R8H1V', 'NJP6N', '0VI0A', '0CEIC', 'MV75A', 'TMKD9']
         """
-        r.rpush('60ZE7', '2', '3', '1')
-        assert r.sort('60ZE7', store='8I2EQ') == 3
-        assert r.lrange('8I2EQ', 0, -1) == [b'1', b'2', b'3']
+        r.rpush("60ZE7", "2", "3", "1")
+        assert r.sort("60ZE7", store="8I2EQ") == 3
+        assert r.lrange("8I2EQ", 0, -1) == [b"1", b"2", b"3"]
 
-    @skip_if_server_version_lt('3.2.0')
+    @skip_if_server_version_lt("3.2.0")
     def test_georadius_store(self, r):
         """
         Generated keys for slot
             0 : ['60ZE7', '8I2EQ']
         """
-        values = (2.1909389952632, 41.433791470673, 'place1') +\
-                 (2.1873744593677, 41.406342043777, 'place2')
+        values = (2.1909389952632, 41.433791470673, "place1") + (
+            2.1873744593677,
+            41.406342043777,
+            "place2",
+        )
 
-        r.geoadd('60ZE7', *values)
-        r.georadius('60ZE7', 2.191, 41.433, 1000, store='8I2EQ')
-        assert r.zrange('8I2EQ', 0, -1) == [b'place1']
+        r.geoadd("60ZE7", *values)
+        r.georadius("60ZE7", 2.191, 41.433, 1000, store="8I2EQ")
+        assert r.zrange("8I2EQ", 0, -1) == [b"place1"]
 
-    @skip_if_server_version_lt('3.2.0')
+    @skip_if_server_version_lt("3.2.0")
     def test_georadius_store_dist(self, r):
         """
         Generated keys for slot
             0 : ['60ZE7', '8I2EQ']
         """
-        values = (2.1909389952632, 41.433791470673, 'place1') +\
-                 (2.1873744593677, 41.406342043777, 'place2')
+        values = (2.1909389952632, 41.433791470673, "place1") + (
+            2.1873744593677,
+            41.406342043777,
+            "place2",
+        )
 
-        r.geoadd('60ZE7', *values)
-        r.georadius('60ZE7', 2.191, 41.433, 1000,
-                    store_dist='8I2EQ')
+        r.geoadd("60ZE7", *values)
+        r.georadius("60ZE7", 2.191, 41.433, 1000, store_dist="8I2EQ")
         # instead of save the geo score, the distance is saved.
-        assert r.zscore('8I2EQ', 'place1') == 88.05060698409301
+        assert r.zscore("8I2EQ", "place1") == 88.05060698409301
 
     @pytest.mark.skip(reason="Sort works if done against keys in same slot")
     def test_sort_by(self, r):
-        r['score:1'] = 8
-        r['score:2'] = 3
-        r['score:3'] = 5
-        r.rpush('a', '3', '2', '1')
-        assert r.sort('a', by='score:*') == [b'2', b'3', b'1']
+        r["score:1"] = 8
+        r["score:2"] = 3
+        r["score:3"] = 5
+        r.rpush("a", "3", "2", "1")
+        assert r.sort("a", by="score:*") == [b"2", b"3", b"1"]
 
     @pytest.mark.skip(reason="Sort works if done against keys in same slot")
     def test_sort_get(self, r):
-        r['user:1'] = 'u1'
-        r['user:2'] = 'u2'
-        r['user:3'] = 'u3'
-        r.rpush('a', '2', '3', '1')
-        assert r.sort('a', get='user:*') == [b'u1', b'u2', b'u3']
+        r["user:1"] = "u1"
+        r["user:2"] = "u2"
+        r["user:3"] = "u3"
+        r.rpush("a", "2", "3", "1")
+        assert r.sort("a", get="user:*") == [b"u1", b"u2", b"u3"]
 
     @pytest.mark.skip(reason="Sort works if done against keys in same slot")
     def test_sort_get_multi(self, r):
-        r['user:1'] = 'u1'
-        r['user:2'] = 'u2'
-        r['user:3'] = 'u3'
-        r.rpush('a', '2', '3', '1')
-        assert r.sort('a', get=('user:*', '#')) == \
-            [b'u1', b'1', b'u2', b'2', b'u3', b'3']
+        r["user:1"] = "u1"
+        r["user:2"] = "u2"
+        r["user:3"] = "u3"
+        r.rpush("a", "2", "3", "1")
+        assert r.sort("a", get=("user:*", "#")) == [
+            b"u1",
+            b"1",
+            b"u2",
+            b"2",
+            b"u3",
+            b"3",
+        ]
 
     @pytest.mark.skip(reason="Sort works if done against keys in same slot")
     def test_sort_get_groups_two(self, r):
-        r['user:1'] = 'u1'
-        r['user:2'] = 'u2'
-        r['user:3'] = 'u3'
-        r.rpush('a', '2', '3', '1')
-        assert r.sort('a', get=('user:*', '#'), groups=True) == \
-            [(b'u1', b'1'), (b'u2', b'2'), (b'u3', b'3')]
+        r["user:1"] = "u1"
+        r["user:2"] = "u2"
+        r["user:3"] = "u3"
+        r.rpush("a", "2", "3", "1")
+        assert r.sort("a", get=("user:*", "#"), groups=True) == [
+            (b"u1", b"1"),
+            (b"u2", b"2"),
+            (b"u3", b"3"),
+        ]
 
     @pytest.mark.skip(reason="Sort works if done against keys in same slot")
     def test_sort_groups_three_gets(self, r):
-        r['user:1'] = 'u1'
-        r['user:2'] = 'u2'
-        r['user:3'] = 'u3'
-        r['door:1'] = 'd1'
-        r['door:2'] = 'd2'
-        r['door:3'] = 'd3'
-        r.rpush('a', '2', '3', '1')
-        assert r.sort('a', get=('user:*', 'door:*', '#'), groups=True) == [
-            (b'u1', b'd1', b'1'),
-            (b'u2', b'd2', b'2'),
-            (b'u3', b'd3', b'3')
+        r["user:1"] = "u1"
+        r["user:2"] = "u2"
+        r["user:3"] = "u3"
+        r["door:1"] = "d1"
+        r["door:2"] = "d2"
+        r["door:3"] = "d3"
+        r.rpush("a", "2", "3", "1")
+        assert r.sort("a", get=("user:*", "door:*", "#"), groups=True) == [
+            (b"u1", b"d1", b"1"),
+            (b"u2", b"d2", b"2"),
+            (b"u3", b"d3", b"3"),
         ]
```

### Comparing `custard-1.1.0/custard/rediscluster/tests/test_encoding.py` & `custard-1.1.1/custard/rediscluster/tests/test_encoding.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/rediscluster/tests/test_encoding_cluster.py` & `custard-1.1.1/custard/rediscluster/tests/test_encoding_cluster.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/rediscluster/tests/test_lock.py` & `custard-1.1.1/custard/rediscluster/tests/test_lock.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/rediscluster/tests/test_monitor.py` & `custard-1.1.1/custard/rediscluster/tests/test_monitor.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/rediscluster/tests/test_multiprocessing.py` & `custard-1.1.1/custard/rediscluster/tests/test_multiprocessing.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/rediscluster/tests/test_multiprocessing_cluster.py` & `custard-1.1.1/custard/rediscluster/tests/test_multiprocessing_cluster.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pytest
 import multiprocessing
 import contextlib
 
 import rediscluster
-from rediscluster.connection import ClusterConnection, ClusterConnectionPool
+from custard.redisclusterconnection import ClusterConnection, ClusterConnectionPool
 from redis.exceptions import ConnectionError
 
 from .conftest import _get_client
 
 
 @contextlib.contextmanager
 def exit_callback(callback, *args):
@@ -18,135 +18,137 @@
 
 
 class TestMultiprocessing(object):
     """
     Cluster: tests must use the cluster specific connection class and client class
              to make tests valid for a cluster case.
     """
+
     # Test connection sharing between forks.
     # See issue #1085 for details.
 
     # use a multi-connection client as that's the only type that is
     # actuall fork/process-safe
     @pytest.fixture()
     def r(self, request):
         return _get_client(
-            rediscluster.RedisCluster,
-            request=request,
-            single_connection_client=False)
+            rediscluster.RedisCluster, request=request, single_connection_client=False
+        )
 
     def test_close_connection_in_child(self):
         """
         A connection owned by a parent and closed by a child doesn't
         destroy the file descriptors so a parent can still use it.
         """
         conn = ClusterConnection(port=7000)
-        conn.send_command('ping')
-        assert conn.read_response() == b'PONG'
+        conn.send_command("ping")
+        assert conn.read_response() == b"PONG"
 
         def target(conn):
-            conn.send_command('ping')
-            assert conn.read_response() == b'PONG'
+            conn.send_command("ping")
+            assert conn.read_response() == b"PONG"
             conn.disconnect()
 
         proc = multiprocessing.Process(target=target, args=(conn,))
         proc.start()
         proc.join(3)
         assert proc.exitcode == 0
 
         # The connection was created in the parent but disconnected in the
         # child. The child called socket.close() but did not call
         # socket.shutdown() because it wasn't the "owning" process.
         # Therefore the connection still works in the parent.
-        conn.send_command('ping')
-        assert conn.read_response() == b'PONG'
+        conn.send_command("ping")
+        assert conn.read_response() == b"PONG"
 
     def test_close_connection_in_parent(self):
         """
         A connection owned by a parent is unusable by a child if the parent
         (the owning process) closes the connection.
         """
         conn = ClusterConnection(port=7000)
-        conn.send_command('ping')
-        assert conn.read_response() == b'PONG'
+        conn.send_command("ping")
+        assert conn.read_response() == b"PONG"
 
         def target(conn, ev):
             ev.wait()
             # the parent closed the connection. because it also created the
             # connection, the connection is shutdown and the child
             # cannot use it.
             with pytest.raises(ConnectionError):
-                conn.send_command('ping')
+                conn.send_command("ping")
 
         ev = multiprocessing.Event()
         proc = multiprocessing.Process(target=target, args=(conn, ev))
         proc.start()
 
         conn.disconnect()
         ev.set()
 
         proc.join(3)
         assert proc.exitcode == 0
 
-    @pytest.mark.parametrize('max_connections', [1, 2, None])
+    @pytest.mark.parametrize("max_connections", [1, 2, None])
     def test_pool(self, max_connections):
         """
         A child will create its own connections when using a pool created
         by a parent.
         """
-        pool = ClusterConnectionPool.from_url('redis://localhost:7000',
-                                       max_connections=max_connections)
+        pool = ClusterConnectionPool.from_url(
+            "redis://localhost:7000", max_connections=max_connections
+        )
 
         conn = pool.get_random_connection()
         main_conn_pid = conn.pid
         with exit_callback(pool.release, conn):
-            conn.send_command('ping')
-            assert conn.read_response() == b'PONG'
+            conn.send_command("ping")
+            assert conn.read_response() == b"PONG"
 
         def target(pool):
             with exit_callback(pool.disconnect):
                 conn = pool.get_random_connection()
                 assert conn.pid != main_conn_pid
                 with exit_callback(pool.release, conn):
-                    assert conn.send_command('ping') is None
-                    assert conn.read_response() == b'PONG'
+                    assert conn.send_command("ping") is None
+                    assert conn.read_response() == b"PONG"
 
         proc = multiprocessing.Process(target=target, args=(pool,))
         proc.start()
         proc.join(3)
         assert proc.exitcode == 0
 
         # Check that connection is still alive after fork process has exited
         # and disconnected the connections in its pool
         conn = pool.get_random_connection()
         with exit_callback(pool.release, conn):
-            assert conn.send_command('ping') is None
-            assert conn.read_response() == b'PONG'
+            assert conn.send_command("ping") is None
+            assert conn.read_response() == b"PONG"
 
-    @pytest.mark.parametrize('max_connections', [1, 2, None])
+    @pytest.mark.parametrize("max_connections", [1, 2, None])
     def test_close_pool_in_main(self, max_connections):
         """
         A child process that uses the same pool as its parent isn't affected
         when the parent disconnects all connections within the pool.
         """
-        pool = ClusterConnectionPool.from_url('redis://localhost:7000',
-                                       max_connections=max_connections)
+        pool = ClusterConnectionPool.from_url(
+            "redis://localhost:7000", max_connections=max_connections
+        )
 
         conn = pool.get_random_connection()
-        assert conn.send_command('ping') is None
-        assert conn.read_response() == b'PONG'
+        assert conn.send_command("ping") is None
+        assert conn.read_response() == b"PONG"
 
         def target(pool, disconnect_event):
             conn = pool.get_random_connection()
             with exit_callback(pool.release, conn):
-                assert conn.send_command('ping') is None
-                assert conn.read_response() == b'PONG'
+                assert conn.send_command("ping") is None
+                assert conn.read_response() == b"PONG"
                 disconnect_event.wait()
-                assert conn.send_command('ping') is None
-                assert conn.read_response() == b'PONG'
+                assert conn.send_command("ping") is None
+                assert conn.read_response() == b"PONG"
 
         ev = multiprocessing.Event()
 
         proc = multiprocessing.Process(target=target, args=(pool, ev))
         proc.start()
 
         pool.disconnect()
```

### Comparing `custard-1.1.0/custard/rediscluster/tests/test_pipeline.py` & `custard-1.1.1/custard/rediscluster/tests/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/rediscluster/tests/test_pipeline_cluster.py` & `custard-1.1.1/custard/rediscluster/tests/test_pipeline_cluster.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,38 +1,47 @@
 # -*- coding: utf-8 -*-
 
 # python std lib
 from __future__ import unicode_literals
 import re
 
 # rediscluster imports
-from rediscluster.client import RedisCluster
-from rediscluster.connection import ClusterConnectionPool, ClusterReadOnlyConnectionPool
-from rediscluster.exceptions import RedisClusterException
+from custard.rediscluster.client import RedisCluster
+from custard.rediscluster.connection import (
+    ClusterConnectionPool,
+    ClusterReadOnlyConnectionPool,
+)
+from custard.rediscluster.exceptions import RedisClusterException
 from tests.conftest import _get_client
 
 # 3rd party imports
 import pytest
 from mock import patch
 from redis._compat import unicode
 from redis.exceptions import ResponseError, ConnectionError
 
 
 class TestPipeline(object):
-    """
-    """
+    """ """
 
     def test_pipeline_eval(self, r):
         with r.pipeline(transaction=False) as pipe:
-            pipe.eval("return {KEYS[1],KEYS[2],ARGV[1],ARGV[2]}", 2, "A{foo}", "B{foo}", "first", "second")
+            pipe.eval(
+                "return {KEYS[1],KEYS[2],ARGV[1],ARGV[2]}",
+                2,
+                "A{foo}",
+                "B{foo}",
+                "first",
+                "second",
+            )
             res = pipe.execute()[0]
-            assert res[0] == b'A{foo}'
-            assert res[1] == b'B{foo}'
-            assert res[2] == b'first'
-            assert res[3] == b'second'
+            assert res[0] == b"A{foo}"
+            assert res[1] == b"B{foo}"
+            assert res[2] == b"first"
+            assert res[3] == b"second"
 
     def test_blocked_methods(self, r):
         """
         Currently some method calls on a Cluster pipeline
         is blocked when using in cluster mode.
         They maybe implemented in the future.
         """
@@ -65,61 +74,65 @@
         """
         Currently some arguments is blocked when using in cluster mode.
         They maybe implemented in the future.
         """
         with pytest.raises(RedisClusterException) as ex:
             r.pipeline(transaction=True)
 
-        assert unicode(ex.value).startswith("transaction is deprecated in cluster mode"), True
+        assert unicode(ex.value).startswith(
+            "transaction is deprecated in cluster mode"
+        ), True
 
         with pytest.raises(RedisClusterException) as ex:
             r.pipeline(shard_hint=True)
 
-        assert unicode(ex.value).startswith("shard_hint is deprecated in cluster mode"), True
+        assert unicode(ex.value).startswith(
+            "shard_hint is deprecated in cluster mode"
+        ), True
 
     def test_redis_cluster_pipeline(self):
         """
         Test that we can use a pipeline with the RedisCluster class
         """
         r = _get_client(RedisCluster)
         with r.pipeline(transaction=False) as pipe:
             pipe.get("foobar")
 
     def test_mget_disabled(self, r):
         with r.pipeline(transaction=False) as pipe:
             with pytest.raises(RedisClusterException):
-                pipe.mget(['a'])
+                pipe.mget(["a"])
 
     def test_mset_disabled(self, r):
         with r.pipeline(transaction=False) as pipe:
             with pytest.raises(RedisClusterException):
-                pipe.mset({'a': 1, 'b': 2})
+                pipe.mset({"a": 1, "b": 2})
 
     def test_rename_disabled(self, r):
         with r.pipeline(transaction=False) as pipe:
             with pytest.raises(RedisClusterException):
-                pipe.rename('a', 'b')
+                pipe.rename("a", "b")
 
     def test_renamenx_disabled(self, r):
         with r.pipeline(transaction=False) as pipe:
             with pytest.raises(RedisClusterException):
-                pipe.renamenx('a', 'b')
+                pipe.renamenx("a", "b")
 
     def test_delete_single(self, r):
-        r['a'] = 1
+        r["a"] = 1
         with r.pipeline(transaction=False) as pipe:
-            pipe.delete('a')
+            pipe.delete("a")
             assert pipe.execute(), True
 
     def test_multi_delete_unsupported(self, r):
         with r.pipeline(transaction=False) as pipe:
-            r['a'] = 1
-            r['b'] = 2
+            r["a"] = 1
+            r["b"] = 2
             with pytest.raises(RedisClusterException):
-                pipe.delete('a', 'b')
+                pipe.delete("a", "b")
 
     def test_brpoplpush_disabled(self, r):
         with r.pipeline(transaction=False) as pipe:
             with pytest.raises(RedisClusterException):
                 pipe.brpoplpush()
 
     def test_rpoplpush_disabled(self, r):
@@ -170,88 +183,88 @@
     def test_spfmerge_disabled(self, r):
         with r.pipeline(transaction=False) as pipe:
             with pytest.raises(RedisClusterException):
                 pipe.pfmerge()
 
     def test_multi_key_operation_with_shared_shards(self, r):
         pipe = r.pipeline(transaction=False)
-        pipe.set('a{foo}', 1)
-        pipe.set('b{foo}', 2)
-        pipe.set('c{foo}', 3)
-        pipe.set('bar', 4)
-        pipe.set('bazz', 5)
-        pipe.get('a{foo}')
-        pipe.get('b{foo}')
-        pipe.get('c{foo}')
-        pipe.get('bar')
-        pipe.get('bazz')
+        pipe.set("a{foo}", 1)
+        pipe.set("b{foo}", 2)
+        pipe.set("c{foo}", 3)
+        pipe.set("bar", 4)
+        pipe.set("bazz", 5)
+        pipe.get("a{foo}")
+        pipe.get("b{foo}")
+        pipe.get("c{foo}")
+        pipe.get("bar")
+        pipe.get("bazz")
         res = pipe.execute()
-        assert res == [True, True, True, True, True, b'1', b'2', b'3', b'4', b'5']
+        assert res == [True, True, True, True, True, b"1", b"2", b"3", b"4", b"5"]
 
     @pytest.mark.xfail(reson="perform_execute_pipeline is not used any longer")
     def test_connection_error(self, r):
         test = self
         test._calls = []
 
         def perform_execute_pipeline(pipe):
             if not test._calls:
-                e = ConnectionError('test')
-                test._calls.append({'exception': e})
+                e = ConnectionError("test")
+                test._calls.append({"exception": e})
                 return [e]
             result = pipe.execute(raise_on_error=False)
-            test._calls.append({'result': result})
+            test._calls.append({"result": result})
             return result
 
         pipe = r.pipeline(transaction=False)
         orig_perform_execute_pipeline = pipe.perform_execute_pipeline
         pipe.perform_execute_pipeline = perform_execute_pipeline
 
         try:
-            pipe.set('foo', 1)
+            pipe.set("foo", 1)
             res = pipe.execute()
             assert res, [True]
-            assert isinstance(test._calls[0]['exception'], ConnectionError)
+            assert isinstance(test._calls[0]["exception"], ConnectionError)
             if len(test._calls) == 2:
-                assert test._calls[1] == {'result': [True]}
+                assert test._calls[1] == {"result": [True]}
             else:
-                assert isinstance(test._calls[1]['result'][0], ResponseError)
-                assert test._calls[2] == {'result': [True]}
+                assert isinstance(test._calls[1]["result"][0], ResponseError)
+                assert test._calls[2] == {"result": [True]}
         finally:
             pipe.perform_execute_pipeline = orig_perform_execute_pipeline
             del test._calls
 
     @pytest.mark.xfail(reson="perform_execute_pipeline is not used any longer")
     def test_asking_error(self, r):
         test = self
         test._calls = []
 
         def perform_execute_pipeline(pipe):
             if not test._calls:
 
-                e = ResponseError("ASK {0} 127.0.0.1:7003".format(r.keyslot('foo')))
-                test._calls.append({'exception': e})
+                e = ResponseError("ASK {0} 127.0.0.1:7003".format(r.keyslot("foo")))
+                test._calls.append({"exception": e})
                 return [e, e]
             result = pipe.execute(raise_on_error=False)
-            test._calls.append({'result': result})
+            test._calls.append({"result": result})
             return result
 
         pipe = r.pipeline(transaction=False)
         orig_perform_execute_pipeline = pipe.perform_execute_pipeline
         pipe.perform_execute_pipeline = perform_execute_pipeline
 
         try:
-            pipe.set('foo', 1)
-            pipe.get('foo')
+            pipe.set("foo", 1)
+            pipe.get("foo")
             res = pipe.execute()
-            assert res == [True, b'1']
-            assert isinstance(test._calls[0]['exception'], ResponseError)
-            assert re.match("ASK", str(test._calls[0]['exception']))
-            assert isinstance(test._calls[1]['result'][0], ResponseError)
-            assert re.match("MOVED", str(test._calls[1]['result'][0]))
-            assert test._calls[2] == {'result': [True, b'1']}
+            assert res == [True, b"1"]
+            assert isinstance(test._calls[0]["exception"], ResponseError)
+            assert re.match("ASK", str(test._calls[0]["exception"]))
+            assert isinstance(test._calls[1]["result"][0], ResponseError)
+            assert re.match("MOVED", str(test._calls[1]["result"][0]))
+            assert test._calls[2] == {"result": [True, b"1"]}
         finally:
             pipe.perform_execute_pipeline = orig_perform_execute_pipeline
             del test._calls
 
     def test_empty_stack(self, r):
         """
         If pipeline is executed with no commands it should
@@ -259,90 +272,106 @@
         """
         p = r.pipeline()
         result = p.execute()
         assert result == []
 
 
 class TestReadOnlyPipeline(object):
-
     def test_pipeline_readonly(self, r, ro):
         """
         On readonly mode, we supports get related stuff only.
         """
-        r.set('foo71', 'a1')   # we assume this key is set on 127.0.0.1:7001
-        r.zadd('foo88', {'z1': 1})  # we assume this key is set on 127.0.0.1:7002
-        r.zadd('foo88', {'z2': 4})
+        r.set("foo71", "a1")  # we assume this key is set on 127.0.0.1:7001
+        r.zadd("foo88", {"z1": 1})  # we assume this key is set on 127.0.0.1:7002
+        r.zadd("foo88", {"z2": 4})
 
         with ro.pipeline() as readonly_pipe:
-            readonly_pipe.get('foo71').zrange('foo88', 0, 5, withscores=True)
+            readonly_pipe.get("foo71").zrange("foo88", 0, 5, withscores=True)
             assert readonly_pipe.execute() == [
-                b'a1',
-                [(b'z1', 1.0), (b'z2', 4)],
+                b"a1",
+                [(b"z1", 1.0), (b"z2", 4)],
             ]
 
     def assert_moved_redirection_on_slave(self, connection_pool_cls, cluster_obj):
-        with patch.object(connection_pool_cls, 'get_node_by_slot') as return_slave_mock:
-            with patch.object(ClusterConnectionPool, 'get_master_node_by_slot') as return_master_mock:
+        with patch.object(connection_pool_cls, "get_node_by_slot") as return_slave_mock:
+            with patch.object(
+                ClusterConnectionPool, "get_master_node_by_slot"
+            ) as return_master_mock:
+
                 def get_mock_node(role, port):
                     return {
-                        'name': '127.0.0.1:{0}'.format(port),
-                        'host': '127.0.0.1',
-                        'port': port,
-                        'server_type': role,
+                        "name": "127.0.0.1:{0}".format(port),
+                        "host": "127.0.0.1",
+                        "port": port,
+                        "server_type": role,
                     }
 
-                return_slave_mock.return_value = get_mock_node('slave', 7005)
-                return_master_mock.return_value = get_mock_node('slave', 7001)
+                return_slave_mock.return_value = get_mock_node("slave", 7005)
+                return_master_mock.return_value = get_mock_node("slave", 7001)
 
                 with cluster_obj.pipeline() as pipe:
                     # we assume this key is set on 127.0.0.1:7001(7004)
-                    pipe.get('foo87').get('foo88').execute() == [None, None]
+                    pipe.get("foo87").get("foo88").execute() == [None, None]
 
     def test_moved_redirection_on_slave_with_default(self):
         """
         On Pipeline, we redirected once and finally get from master with
         readonly client when data is completely moved.
         """
         self.assert_moved_redirection_on_slave(
             ClusterConnectionPool,
-            RedisCluster(host="127.0.0.1", port=7000, reinitialize_steps=1)
+            RedisCluster(host="127.0.0.1", port=7000, reinitialize_steps=1),
         )
 
     def test_moved_redirection_on_slave_with_readonly_mode_client(self):
         """
         Ditto with READONLY mode.
         """
         self.assert_moved_redirection_on_slave(
             ClusterReadOnlyConnectionPool,
-            RedisCluster(host="127.0.0.1", port=7000, readonly_mode=True, reinitialize_steps=1)
+            RedisCluster(
+                host="127.0.0.1", port=7000, readonly_mode=True, reinitialize_steps=1
+            ),
         )
 
     def test_access_correct_slave_with_readonly_mode_client(self, sr):
         """
         Test that the client can get value normally with readonly mode
         when we connect to correct slave.
         """
 
         # we assume this key is set on 127.0.0.1:7001
-        sr.set('foo87', 'foo')
-        sr.set('foo88', 'bar')
+        sr.set("foo87", "foo")
+        sr.set("foo88", "bar")
         import time
+
         time.sleep(1)
 
-        with patch.object(ClusterReadOnlyConnectionPool, 'get_node_by_slot') as return_slave_mock:
+        with patch.object(
+            ClusterReadOnlyConnectionPool, "get_node_by_slot"
+        ) as return_slave_mock:
             return_slave_mock.return_value = {
-                'name': '127.0.0.1:7004',
-                'host': '127.0.0.1',
-                'port': 7004,
-                'server_type': 'slave',
+                "name": "127.0.0.1:7004",
+                "host": "127.0.0.1",
+                "port": 7004,
+                "server_type": "slave",
             }
 
             master_value = {
-                'host': '127.0.0.1',
-                'name': '127.0.0.1:7001',
-                'port': 7001,
-                'server_type': 'master',
+                "host": "127.0.0.1",
+                "name": "127.0.0.1:7001",
+                "port": 7001,
+                "server_type": "master",
             }
-            with patch.object(ClusterConnectionPool, 'get_master_node_by_slot', return_value=master_value):
-                readonly_client = RedisCluster(host="127.0.0.1", port=7000, readonly_mode=True)
+            with patch.object(
+                ClusterConnectionPool,
+                "get_master_node_by_slot",
+                return_value=master_value,
+            ):
+                readonly_client = RedisCluster(
+                    host="127.0.0.1", port=7000, readonly_mode=True
+                )
                 with readonly_client.pipeline() as readonly_pipe:
-                    assert readonly_pipe.get('foo88').get('foo87').execute() == [b'bar', b'foo']
+                    assert readonly_pipe.get("foo88").get("foo87").execute() == [
+                        b"bar",
+                        b"foo",
+                    ]
```

### Comparing `custard-1.1.0/custard/rediscluster/tests/test_pubsub.py` & `custard-1.1.1/custard/rediscluster/tests/test_pubsub.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # python std lib
 from __future__ import unicode_literals
 import threading
 import time
 
 # rediscluster imports
-from rediscluster.client import RedisCluster
+from custard.rediscluster.client import RedisCluster
 
 # 3rd party imports
 import pytest
 
 import redis
 from redis import Redis
 from redis.exceptions import ConnectionError
```

### Comparing `custard-1.1.0/custard/rediscluster/tests/test_scripting.py` & `custard-1.1.1/custard/rediscluster/tests/test_scripting.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 # python std lib
 from __future__ import unicode_literals
 
 # rediscluster imports
-from rediscluster.exceptions import RedisClusterException
+from custard.rediscluster.exceptions import RedisClusterException
 
 # 3rd party imports
 from redis import exceptions
 import pytest
 
 
 multiply_script = """
@@ -30,129 +30,129 @@
 
 class TestScripting(object):
     @pytest.fixture(autouse=True)
     def reset_scripts(self, r):
         r.script_flush()
 
     def test_eval(self, r):
-        r.set('a', 2)
+        r.set("a", 2)
         # 2 * 3 == 6
-        assert r.eval(multiply_script, 1, 'a', 3) == 6
+        assert r.eval(multiply_script, 1, "a", 3) == 6
 
     def test_eval_same_slot(self, r):
-        r.set('A{foo}', 2)
-        r.set('B{foo}', 4)
+        r.set("A{foo}", 2)
+        r.set("B{foo}", 4)
         # 2 * 4 == 8
 
         script = """
         local value = redis.call('GET', KEYS[1])
         local value2 = redis.call('GET', KEYS[2])
         return value * value2
         """
-        result = r.eval(script, 2, 'A{foo}', 'B{foo}')
+        result = r.eval(script, 2, "A{foo}", "B{foo}")
         assert result == 8
 
     def test_eval_crossslot(self, r):
         """
         This test assumes that {foo} and {bar} will not go to the same
         server when used. In 3 masters + 3 slaves config this should pass.
         """
-        r.set('A{foo}', 2)
-        r.set('B{bar}', 4)
+        r.set("A{foo}", 2)
+        r.set("B{bar}", 4)
         # 2 * 4 == 8
 
         script = """
         local value = redis.call('GET', KEYS[1])
         local value2 = redis.call('GET', KEYS[2])
         return value * value2
         """
         with pytest.raises(RedisClusterException):
-            r.eval(script, 2, 'A{foo}', 'B{bar}')
+            r.eval(script, 2, "A{foo}", "B{bar}")
 
     def test_evalsha(self, r):
-        r.set('a', 2)
+        r.set("a", 2)
         sha = r.script_load(multiply_script)
         # 2 * 3 == 6
-        assert r.evalsha(sha, 1, 'a', 3) == 6
+        assert r.evalsha(sha, 1, "a", 3) == 6
 
     def test_evalsha_script_not_loaded(self, r):
-        r.set('a', 2)
+        r.set("a", 2)
         sha = r.script_load(multiply_script)
         # remove the script from Redis's cache
         r.script_flush()
         with pytest.raises(exceptions.NoScriptError):
-            r.evalsha(sha, 1, 'a', 3)
+            r.evalsha(sha, 1, "a", 3)
 
     def test_script_loading(self, r):
         # get the sha, then clear the cache
         sha = r.script_load(multiply_script)
         r.script_flush()
         assert r.script_exists(sha) == [False]
         r.script_load(multiply_script)
         assert r.script_exists(sha) == [True]
 
     def test_script_object(self, r):
-        r.set('a', 2)
+        r.set("a", 2)
         multiply = r.register_script(multiply_script)
         precalculated_sha = multiply.sha
         assert precalculated_sha
         assert r.script_exists(multiply.sha) == [False]
         # Test second evalsha block (after NoScriptError)
-        assert multiply(keys=['a'], args=[3]) == 6
+        assert multiply(keys=["a"], args=[3]) == 6
         # At this point, the script should be loaded
         assert r.script_exists(multiply.sha) == [True]
         # Test that the precalculated sha matches the one from redis
         assert multiply.sha == precalculated_sha
         # Test first evalsha block
-        assert multiply(keys=['a'], args=[3]) == 6
+        assert multiply(keys=["a"], args=[3]) == 6
 
     @pytest.mark.xfail(reason="Script object not supported in cluster")
     def test_script_object_in_pipeline(self, r):
         multiply = r.register_script(multiply_script)
         precalculated_sha = multiply.sha
         assert precalculated_sha
         pipe = r.pipeline()
-        pipe.set('a', 2)
-        pipe.get('a')
-        multiply(keys=['a'], args=[3], client=pipe)
+        pipe.set("a", 2)
+        pipe.get("a")
+        multiply(keys=["a"], args=[3], client=pipe)
         assert r.script_exists(multiply.sha) == [False]
         # [SET worked, GET 'a', result of multiple script]
-        assert pipe.execute() == [True, b'2', 6]
+        assert pipe.execute() == [True, b"2", 6]
         # The script should have been loaded by pipe.execute()
         assert r.script_exists(multiply.sha) == [True]
         # The precalculated sha should have been the correct one
         assert multiply.sha == precalculated_sha
 
         # purge the script from redis's cache and re-run the pipeline
         # the multiply script should be reloaded by pipe.execute()
         r.script_flush()
         pipe = r.pipeline()
-        pipe.set('a', 2)
-        pipe.get('a')
-        multiply(keys=['a'], args=[3], client=pipe)
+        pipe.set("a", 2)
+        pipe.get("a")
+        multiply(keys=["a"], args=[3], client=pipe)
         assert r.script_exists(multiply.sha) == [False]
         # [SET worked, GET 'a', result of multiple script]
-        assert pipe.execute() == [True, b'2', 6]
+        assert pipe.execute() == [True, b"2", 6]
         assert r.script_exists(multiply.sha) == [True]
 
     @pytest.mark.xfail(reason="LUA is not supported in cluster")
     def test_eval_msgpack_pipeline_error_in_lua(self, r):
         msgpack_hello = r.register_script(msgpack_hello_script)
         assert msgpack_hello.sha
 
         pipe = r.pipeline()
 
         # avoiding a dependency to msgpack, this is the output of
         # msgpack.dumps({"name": "joe"})
-        msgpack_message_1 = b'\x81\xa4name\xa3Joe'
+        msgpack_message_1 = b"\x81\xa4name\xa3Joe"
 
         msgpack_hello(args=[msgpack_message_1], client=pipe)
 
         assert r.script_exists(msgpack_hello.sha) == [False]
-        assert pipe.execute()[0] == b'hello Joe'
+        assert pipe.execute()[0] == b"hello Joe"
         assert r.script_exists(msgpack_hello.sha) == [True]
 
         msgpack_hello_broken = r.register_script(msgpack_hello_script_broken)
 
         msgpack_hello_broken(args=[msgpack_message_1], client=pipe)
         with pytest.raises(exceptions.ResponseError) as excinfo:
             pipe.execute()
```

### Comparing `custard-1.1.0/custard/rediscluster/tests/test_utils.py` & `custard-1.1.1/custard/rediscluster/tests/test_utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 
 # python std lib
 from __future__ import with_statement
 
 # rediscluster imports
-from rediscluster.exceptions import RedisClusterException
-from rediscluster.utils import (
+from custard.rediscluster.exceptions import RedisClusterException
+from custard.rediscluster.utils import (
     string_keys_to_dict,
     dict_merge,
     blocked_command,
     merge_result,
     first_key,
     parse_cluster_slots,
 )
@@ -49,56 +49,94 @@
           2) (integer) 10000
           3) "069cda388c7c41c62abe892d9e0a2d55fbf5ffd5"
        4) 1) "10.0.0.6"
           2) (integer) 10000
           3) "dc152a08b4cf1f2a0baf775fb86ad0938cb907dc"
     """
     mock_response = [
-        [0, 5460, ['172.17.0.2', 7000], ['172.17.0.2', 7003]],
-        [5461, 10922, ['172.17.0.2', 7001], ['172.17.0.2', 7004]],
-        [10923, 16383, ['172.17.0.2', 7002], ['172.17.0.2', 7005]]
+        [0, 5460, ["172.17.0.2", 7000], ["172.17.0.2", 7003]],
+        [5461, 10922, ["172.17.0.2", 7001], ["172.17.0.2", 7004]],
+        [10923, 16383, ["172.17.0.2", 7002], ["172.17.0.2", 7005]],
     ]
     parse_cluster_slots(mock_response)
 
     extended_mock_response = [
-        [0, 5460, ['172.17.0.2', 7000, 'ffd36d8d7cb10d813f81f9662a835f6beea72677'], ['172.17.0.2', 7003, '5c15b69186017ddc25ebfac81e74694fc0c1a160']],
-        [5461, 10922, ['172.17.0.2', 7001, '069cda388c7c41c62abe892d9e0a2d55fbf5ffd5'], ['172.17.0.2', 7004, 'dc152a08b4cf1f2a0baf775fb86ad0938cb907dc']],
-        [10923, 16383, ['172.17.0.2', 7002, '3588b4cf9fc72d57bb262a024747797ead0cf7ea'], ['172.17.0.2', 7005, 'a72c02c7d85f4ec3145ab2c411eefc0812aa96b0']]
+        [
+            0,
+            5460,
+            ["172.17.0.2", 7000, "ffd36d8d7cb10d813f81f9662a835f6beea72677"],
+            ["172.17.0.2", 7003, "5c15b69186017ddc25ebfac81e74694fc0c1a160"],
+        ],
+        [
+            5461,
+            10922,
+            ["172.17.0.2", 7001, "069cda388c7c41c62abe892d9e0a2d55fbf5ffd5"],
+            ["172.17.0.2", 7004, "dc152a08b4cf1f2a0baf775fb86ad0938cb907dc"],
+        ],
+        [
+            10923,
+            16383,
+            ["172.17.0.2", 7002, "3588b4cf9fc72d57bb262a024747797ead0cf7ea"],
+            ["172.17.0.2", 7005, "a72c02c7d85f4ec3145ab2c411eefc0812aa96b0"],
+        ],
     ]
 
     parse_cluster_slots(extended_mock_response)
 
     mock_binary_response = [
-        [0, 5460, [b'172.17.0.2', 7000], [b'172.17.0.2', 7003]],
-        [5461, 10922, [b'172.17.0.2', 7001], [b'172.17.0.2', 7004]],
-        [10923, 16383, [b'172.17.0.2', 7002], [b'172.17.0.2', 7005]]
+        [0, 5460, [b"172.17.0.2", 7000], [b"172.17.0.2", 7003]],
+        [5461, 10922, [b"172.17.0.2", 7001], [b"172.17.0.2", 7004]],
+        [10923, 16383, [b"172.17.0.2", 7002], [b"172.17.0.2", 7005]],
     ]
     parse_cluster_slots(mock_binary_response)
 
     extended_mock_binary_response = [
-        [0, 5460, [b'172.17.0.2', 7000, b'ffd36d8d7cb10d813f81f9662a835f6beea72677'], [b'172.17.0.2', 7003, b'5c15b69186017ddc25ebfac81e74694fc0c1a160']],
-        [5461, 10922, [b'172.17.0.2', 7001, b'069cda388c7c41c62abe892d9e0a2d55fbf5ffd5'], [b'172.17.0.2', 7004, b'dc152a08b4cf1f2a0baf775fb86ad0938cb907dc']],
-        [10923, 16383, [b'172.17.0.2', 7002, b'3588b4cf9fc72d57bb262a024747797ead0cf7ea'], [b'172.17.0.2', 7005, b'a72c02c7d85f4ec3145ab2c411eefc0812aa96b0']]
+        [
+            0,
+            5460,
+            [b"172.17.0.2", 7000, b"ffd36d8d7cb10d813f81f9662a835f6beea72677"],
+            [b"172.17.0.2", 7003, b"5c15b69186017ddc25ebfac81e74694fc0c1a160"],
+        ],
+        [
+            5461,
+            10922,
+            [b"172.17.0.2", 7001, b"069cda388c7c41c62abe892d9e0a2d55fbf5ffd5"],
+            [b"172.17.0.2", 7004, b"dc152a08b4cf1f2a0baf775fb86ad0938cb907dc"],
+        ],
+        [
+            10923,
+            16383,
+            [b"172.17.0.2", 7002, b"3588b4cf9fc72d57bb262a024747797ead0cf7ea"],
+            [b"172.17.0.2", 7005, b"a72c02c7d85f4ec3145ab2c411eefc0812aa96b0"],
+        ],
     ]
 
     extended_mock_parsed = {
-        (0, 5460): {'master': ('172.17.0.2', 7000), 'slaves': [('172.17.0.2', 7003)]},
-        (5461, 10922): {'master': ('172.17.0.2', 7001),
-                        'slaves': [('172.17.0.2', 7004)]},
-        (10923, 16383): {'master': ('172.17.0.2', 7002),
-                         'slaves': [('172.17.0.2', 7005)]}
+        (0, 5460): {"master": ("172.17.0.2", 7000), "slaves": [("172.17.0.2", 7003)]},
+        (5461, 10922): {
+            "master": ("172.17.0.2", 7001),
+            "slaves": [("172.17.0.2", 7004)],
+        },
+        (10923, 16383): {
+            "master": ("172.17.0.2", 7002),
+            "slaves": [("172.17.0.2", 7005)],
+        },
     }
 
     assert parse_cluster_slots(extended_mock_binary_response) == extended_mock_parsed
 
 
 def test_string_keys_to():
     def mock_true():
         return True
-    assert string_keys_to_dict(["FOO", "BAR"], mock_true) == {"FOO": mock_true, "BAR": mock_true}
+
+    assert string_keys_to_dict(["FOO", "BAR"], mock_true) == {
+        "FOO": mock_true,
+        "BAR": mock_true,
+    }
 
 
 def test_dict_merge():
     a = {"a": 1}
     b = {"b": 2}
     c = {"c": 3}
     assert dict_merge(a, b, c) == {"a": 1, "b": 2, "c": 3}
@@ -112,15 +150,22 @@
 def test_blocked_command():
     with pytest.raises(RedisClusterException) as ex:
         blocked_command(None, "SET")
     assert unicode(ex.value) == "Command: SET is blocked in redis cluster mode"
 
 
 def test_merge_result():
-    assert merge_result("foobar", {"a": [1, 2, 3], "b": [4, 5, 6]}) == [1, 2, 3, 4, 5, 6]
+    assert merge_result("foobar", {"a": [1, 2, 3], "b": [4, 5, 6]}) == [
+        1,
+        2,
+        3,
+        4,
+        5,
+        6,
+    ]
     assert merge_result("foobar", {"a": [1, 2, 3], "b": [1, 2, 3]}) == [1, 2, 3]
 
 
 def test_merge_result_value_error():
     with pytest.raises(ValueError):
         merge_result("foobar", [])
```

### Comparing `custard-1.1.0/custard/script/compat.py` & `custard-1.1.1/custard/script/compat.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/script/parser.py` & `custard-1.1.1/custard/script/parser.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/script/schema.py` & `custard-1.1.1/custard/script/schema.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/swagger/__init__.py` & `custard-1.1.1/custard/swagger/__init__.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/swagger/loader.py` & `custard-1.1.1/custard/swagger/loader.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/swagger/swagger.py` & `custard-1.1.1/custard/swagger/swagger.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/swagger/utils.py` & `custard-1.1.1/custard/swagger/utils.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/time/dafunc.py` & `custard-1.1.1/custard/time/dafunc.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/time/exceptions.py` & `custard-1.1.1/custard/time/exceptions.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/time/moment.py` & `custard-1.1.1/custard/time/moment.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/time/stoppable_thread.py` & `custard-1.1.1/custard/time/stoppable_thread.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/utils/datasets.py` & `custard-1.1.1/custard/utils/datasets.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/utils/decorators.py` & `custard-1.1.1/custard/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/custard/utils/text.py` & `custard-1.1.1/custard/utils/text.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/examples/async_lur.py` & `custard-1.1.1/examples/async_lur.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/examples/decorator.py` & `custard-1.1.1/examples/decorator.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/examples/dts.py` & `custard-1.1.1/examples/dts.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/examples/hitfilter.py` & `custard-1.1.1/examples/hitfilter.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/examples/json_logger.py` & `custard-1.1.1/examples/json_logger.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/examples/kaptcha.py` & `custard-1.1.1/examples/kaptcha.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/examples/kaptcha_execution_time.py` & `custard-1.1.1/examples/kaptcha_execution_time.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/examples/limiter.py` & `custard-1.1.1/examples/limiter.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/examples/mock.py` & `custard-1.1.1/examples/mock.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/examples/pagination_async_sqlalchemy.py` & `custard-1.1.1/examples/pagination_async_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/examples/pagination_sqlalchemy.py` & `custard-1.1.1/examples/pagination_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/examples/swagger_online_change.py` & `custard-1.1.1/examples/swagger_online_change.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/examples/swagger_usabletest.py` & `custard-1.1.1/examples/swagger_usabletest.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/examples/useragent.py` & `custard-1.1.1/examples/useragent.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/README.md` & `custard-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/pyproject.toml` & `custard-1.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `custard-1.1.0/PKG-INFO` & `custard-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: custard
-Version: 1.1.0
+Version: 1.1.1
 Summary: custard easy to learn, fast to code, ready for production
 Project-URL: Homepage, https://github.com/kamalyes/custard
 Author-email: Kamalyes <mryu168@163.com>
 License-Expression: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
```

