# Comparing `tmp/PlexTraktSync-0.26.3.tar.gz` & `tmp/PlexTraktSync-0.26.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/PlexTraktSync/PlexTraktSync/dist/.tmp-y45vpp_0/PlexTraktSync-0.26.3.tar", last modified: Mon Apr 24 18:36:04 2023, max compression
+gzip compressed data, was "/home/runner/work/PlexTraktSync/PlexTraktSync/dist/.tmp-ro158mv9/PlexTraktSync-0.26.4.tar", last modified: Tue Apr 25 07:57:20 2023, max compression
```

## Comparing `PlexTraktSync-0.26.3.tar` & `PlexTraktSync-0.26.4.tar`

### file list

```diff
@@ -1,130 +1,130 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:36:04.000000 PlexTraktSync-0.26.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18583 2023-04-24 18:36:04.000000 PlexTraktSync-0.26.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:36:04.000000 PlexTraktSync-0.26.3/PlexTraktSync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18583 2023-04-24 18:36:04.000000 PlexTraktSync-0.26.3/PlexTraktSync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-04-24 18:36:04.000000 PlexTraktSync-0.26.3/PlexTraktSync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 18:36:04.000000 PlexTraktSync-0.26.3/PlexTraktSync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-24 18:36:04.000000 PlexTraktSync-0.26.3/PlexTraktSync.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-04-24 18:36:04.000000 PlexTraktSync-0.26.3/PlexTraktSync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-24 18:36:04.000000 PlexTraktSync-0.26.3/PlexTraktSync.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    17733 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:36:04.000000 PlexTraktSync-0.26.3/plextraktsync/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-24 18:35:51.000000 PlexTraktSync-0.26.3/plextraktsync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/plextraktsync/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7741 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/plextraktsync/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:36:04.000000 PlexTraktSync-0.26.3/plextraktsync/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/plextraktsync/commands/bug_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/plextraktsync/commands/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/plextraktsync/commands/clear_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/plextraktsync/commands/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/plextraktsync/commands/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/plextraktsync/commands/imdb_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/plextraktsync/commands/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/plextraktsync/commands/inspect.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/plextraktsync/commands/login.py
--rw-r--r--   0 runner    (1001) docker     (123)     7158 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/plextraktsync/commands/plex_login.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/plextraktsync/commands/self_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/plextraktsync/commands/sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/plextraktsync/commands/trakt_login.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/plextraktsync/commands/unmatched.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/plextraktsync/commands/watch.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/plextraktsync/commands/watched_shows.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:36:04.000000 PlexTraktSync-0.26.3/plextraktsync/config/
--rw-r--r--   0 runner    (1001) docker     (123)     5899 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/plextraktsync/config/Config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/plextraktsync/config/ConfigLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/plextraktsync/config/ConfigMergeMixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/plextraktsync/config/HttpCacheConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/plextraktsync/config/PlexServerConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/plextraktsync/config/RunConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/plextraktsync/config/ServerConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/plextraktsync/config/SyncConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/plextraktsync/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/plextraktsync/config.default.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:36:04.000000 PlexTraktSync-0.26.3/plextraktsync/decorators/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/plextraktsync/decorators/cached_property.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/plextraktsync/decorators/flatten.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/plextraktsync/decorators/http_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/plextraktsync/decorators/measure_time.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/plextraktsync/decorators/memoize.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/plextraktsync/decorators/nocache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/plextraktsync/decorators/rate_limit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/plextraktsync/decorators/retry.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/plextraktsync/decorators/time_limit.py
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/plextraktsync/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:36:04.000000 PlexTraktSync-0.26.3/plextraktsync/logger/
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/plextraktsync/logger/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/plextraktsync/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     9383 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/plextraktsync/media.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:36:04.000000 PlexTraktSync-0.26.3/plextraktsync/mixin/
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/plextraktsync/mixin/ChangeNotifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/plextraktsync/path.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:36:04.000000 PlexTraktSync-0.26.3/plextraktsync/plex/
--rw-r--r--   0 runner    (1001) docker     (123)     9862 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/plextraktsync/plex/PlexApi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/plextraktsync/plex/PlexAudioCodec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/plextraktsync/plex/PlexGuid.py
--rw-r--r--   0 runner    (1001) docker     (123)     8856 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/plextraktsync/plex/PlexLibraryItem.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/plextraktsync/plex/PlexLibrarySection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/plextraktsync/plex/PlexRatings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/plextraktsync/plex/PlexServerConnection.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/plextraktsync/plex/PlexWatchList.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/plextraktsync/plex/SessionCollection.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/plextraktsync/plex/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/plextraktsync/pytrakt_extensions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:36:04.000000 PlexTraktSync-0.26.3/plextraktsync/queue/
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/plextraktsync/queue/BackgroundTask.py
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/plextraktsync/queue/Queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/plextraktsync/queue/TraktBatchWorker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/plextraktsync/queue/TraktMarkWatchedWorker.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/plextraktsync/rich_addons.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/plextraktsync/servers.default.yml
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/plextraktsync/style.py
--rw-r--r--   0 runner    (1001) docker     (123)    10159 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/plextraktsync/sync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:36:04.000000 PlexTraktSync-0.26.3/plextraktsync/trakt/
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/plextraktsync/trakt/PartialTraktMedia.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/plextraktsync/trakt/ScrobblerCollection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/plextraktsync/trakt/ScrobblerProxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     8988 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/plextraktsync/trakt/TraktApi.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/plextraktsync/trakt/TraktItem.py
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/plextraktsync/trakt/TraktLookup.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/plextraktsync/trakt/TraktRatingCollection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/plextraktsync/trakt/TraktWatchlist.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/plextraktsync/trakt/trakt_set.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/plextraktsync/trakt/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/plextraktsync/trakt_list_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:36:04.000000 PlexTraktSync-0.26.3/plextraktsync/util/
--rw-r--r--   0 runner    (1001) docker     (123)     7997 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/plextraktsync/util/Factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/plextraktsync/util/Path.py
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/plextraktsync/util/Timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/plextraktsync/util/Version.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/plextraktsync/util/execp.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/plextraktsync/util/execx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/plextraktsync/util/expand_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/plextraktsync/util/git_version_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/plextraktsync/util/local_url.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/plextraktsync/util/openurl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/plextraktsync/util/packaging.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/plextraktsync/util/parse_date.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/plextraktsync/util/remove_empty_values.py
--rw-r--r--   0 runner    (1001) docker     (123)    11713 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/plextraktsync/walker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:36:04.000000 PlexTraktSync-0.26.3/plextraktsync/watch/
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/plextraktsync/watch/EventDispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/plextraktsync/watch/EventFactory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/plextraktsync/watch/ProgressBar.py
--rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/plextraktsync/watch/WatchStateUpdater.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/plextraktsync/watch/WebSocketListener.py
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/plextraktsync/watch/events.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-04-24 18:35:56.000000 PlexTraktSync-0.26.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-04-24 18:36:04.000000 PlexTraktSync-0.26.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:36:04.000000 PlexTraktSync-0.26.3/tests/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1923 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/tests/test_collection_metadata.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1443 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/tests/test_config.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2703 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/tests/test_events.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      977 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/tests/test_new_agent.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      442 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/tests/test_plex_search.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      503 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/tests/test_threading.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1174 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/tests/test_timer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      572 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/tests/test_trakt_progress.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3584 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/tests/test_tv_lookup.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1926 2023-04-24 18:35:50.000000 PlexTraktSync-0.26.3/tests/test_walker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:57:20.000000 PlexTraktSync-0.26.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18583 2023-04-25 07:57:20.000000 PlexTraktSync-0.26.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:57:20.000000 PlexTraktSync-0.26.4/PlexTraktSync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18583 2023-04-25 07:57:20.000000 PlexTraktSync-0.26.4/PlexTraktSync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-04-25 07:57:20.000000 PlexTraktSync-0.26.4/PlexTraktSync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 07:57:20.000000 PlexTraktSync-0.26.4/PlexTraktSync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-25 07:57:20.000000 PlexTraktSync-0.26.4/PlexTraktSync.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-04-25 07:57:20.000000 PlexTraktSync-0.26.4/PlexTraktSync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-25 07:57:20.000000 PlexTraktSync-0.26.4/PlexTraktSync.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    17733 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:57:20.000000 PlexTraktSync-0.26.4/plextraktsync/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7741 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:57:20.000000 PlexTraktSync-0.26.4/plextraktsync/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/commands/bug_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/commands/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/commands/clear_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/commands/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/commands/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/commands/imdb_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/commands/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/commands/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/commands/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7158 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/commands/plex_login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/commands/self_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/commands/sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/commands/trakt_login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/commands/unmatched.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/commands/watch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/commands/watched_shows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:57:20.000000 PlexTraktSync-0.26.4/plextraktsync/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     5899 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/config/Config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/config/ConfigLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/config/ConfigMergeMixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/config/HttpCacheConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/config/PlexServerConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/config/RunConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/config/ServerConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/config/SyncConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/config.default.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:57:20.000000 PlexTraktSync-0.26.4/plextraktsync/decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/decorators/cached_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/decorators/flatten.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/decorators/http_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/decorators/measure_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/decorators/memoize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/decorators/nocache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/decorators/rate_limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/decorators/retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/decorators/time_limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:57:20.000000 PlexTraktSync-0.26.4/plextraktsync/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/logger/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9383 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/media.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:57:20.000000 PlexTraktSync-0.26.4/plextraktsync/mixin/
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/mixin/ChangeNotifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/path.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:57:20.000000 PlexTraktSync-0.26.4/plextraktsync/plex/
+-rw-r--r--   0 runner    (1001) docker     (123)     9862 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/plex/PlexApi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/plex/PlexAudioCodec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/plex/PlexGuid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8856 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/plex/PlexLibraryItem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/plex/PlexLibrarySection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/plex/PlexRatings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/plex/PlexServerConnection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/plex/PlexWatchList.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/plex/SessionCollection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/plex/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/pytrakt_extensions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:57:20.000000 PlexTraktSync-0.26.4/plextraktsync/queue/
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/queue/BackgroundTask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/queue/Queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/queue/TraktBatchWorker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/queue/TraktMarkWatchedWorker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/rich_addons.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/servers.default.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/style.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10159 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/sync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:57:20.000000 PlexTraktSync-0.26.4/plextraktsync/trakt/
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/trakt/PartialTraktMedia.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/trakt/ScrobblerCollection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/trakt/ScrobblerProxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8988 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/trakt/TraktApi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/trakt/TraktItem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/trakt/TraktLookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/trakt/TraktRatingCollection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/trakt/TraktWatchlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/trakt/trakt_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/trakt/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/trakt_list_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:57:20.000000 PlexTraktSync-0.26.4/plextraktsync/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     7997 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/util/Factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/util/Path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/util/Timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/util/Version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/util/execp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/util/execx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/util/expand_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/util/git_version_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/util/local_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/util/openurl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/util/packaging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/util/parse_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/util/remove_empty_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11713 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/walker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:57:20.000000 PlexTraktSync-0.26.4/plextraktsync/watch/
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/watch/EventDispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/watch/EventFactory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/watch/ProgressBar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/watch/WatchStateUpdater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/watch/WebSocketListener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/watch/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-04-25 07:57:12.000000 PlexTraktSync-0.26.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-04-25 07:57:20.000000 PlexTraktSync-0.26.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:57:20.000000 PlexTraktSync-0.26.4/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1923 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/tests/test_collection_metadata.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1443 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/tests/test_config.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2703 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/tests/test_events.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      977 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/tests/test_new_agent.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      442 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/tests/test_plex_search.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      503 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/tests/test_threading.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1174 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/tests/test_timer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      572 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/tests/test_trakt_progress.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3584 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/tests/test_tv_lookup.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1926 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/tests/test_walker.py
```

### Comparing `PlexTraktSync-0.26.3/LICENSE` & `PlexTraktSync-0.26.4/LICENSE`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.3/PKG-INFO` & `PlexTraktSync-0.26.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PlexTraktSync
-Version: 0.26.3
+Version: 0.26.4
 Summary: Plex-Trakt-Sync is a two-way-sync between trakt.tv and Plex Media Server
 Home-page: https://github.com/Taxel/PlexTraktSync
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Taxel/PlexTraktSync/issues
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `PlexTraktSync-0.26.3/PlexTraktSync.egg-info/PKG-INFO` & `PlexTraktSync-0.26.4/PlexTraktSync.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PlexTraktSync
-Version: 0.26.3
+Version: 0.26.4
 Summary: Plex-Trakt-Sync is a two-way-sync between trakt.tv and Plex Media Server
 Home-page: https://github.com/Taxel/PlexTraktSync
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Taxel/PlexTraktSync/issues
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `PlexTraktSync-0.26.3/PlexTraktSync.egg-info/SOURCES.txt` & `PlexTraktSync-0.26.4/PlexTraktSync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.3/PlexTraktSync.egg-info/requires.txt` & `PlexTraktSync-0.26.4/PlexTraktSync.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.3/README.md` & `PlexTraktSync-0.26.4/README.md`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.3/plextraktsync/cli.py` & `PlexTraktSync-0.26.4/plextraktsync/cli.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.3/plextraktsync/commands/bug_report.py` & `PlexTraktSync-0.26.4/plextraktsync/commands/bug_report.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.3/plextraktsync/commands/cache.py` & `PlexTraktSync-0.26.4/plextraktsync/commands/cache.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.3/plextraktsync/commands/clear_collections.py` & `PlexTraktSync-0.26.4/plextraktsync/commands/clear_collections.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.3/plextraktsync/commands/config.py` & `PlexTraktSync-0.26.4/plextraktsync/commands/config.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.3/plextraktsync/commands/download.py` & `PlexTraktSync-0.26.4/plextraktsync/commands/download.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.3/plextraktsync/commands/imdb_import.py` & `PlexTraktSync-0.26.4/plextraktsync/commands/imdb_import.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.3/plextraktsync/commands/info.py` & `PlexTraktSync-0.26.4/plextraktsync/commands/info.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.3/plextraktsync/commands/inspect.py` & `PlexTraktSync-0.26.4/plextraktsync/commands/inspect.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.3/plextraktsync/commands/login.py` & `PlexTraktSync-0.26.4/plextraktsync/commands/login.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.3/plextraktsync/commands/plex_login.py` & `PlexTraktSync-0.26.4/plextraktsync/commands/plex_login.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.3/plextraktsync/commands/self_update.py` & `PlexTraktSync-0.26.4/plextraktsync/commands/self_update.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.3/plextraktsync/commands/sync.py` & `PlexTraktSync-0.26.4/plextraktsync/commands/sync.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.3/plextraktsync/commands/trakt_login.py` & `PlexTraktSync-0.26.4/plextraktsync/commands/trakt_login.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.3/plextraktsync/commands/unmatched.py` & `PlexTraktSync-0.26.4/plextraktsync/commands/unmatched.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.3/plextraktsync/commands/watch.py` & `PlexTraktSync-0.26.4/plextraktsync/commands/watch.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.3/plextraktsync/commands/watched_shows.py` & `PlexTraktSync-0.26.4/plextraktsync/commands/watched_shows.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.3/plextraktsync/config/Config.py` & `PlexTraktSync-0.26.4/plextraktsync/config/Config.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.3/plextraktsync/config/ConfigLoader.py` & `PlexTraktSync-0.26.4/plextraktsync/config/ConfigLoader.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.3/plextraktsync/config/HttpCacheConfig.py` & `PlexTraktSync-0.26.4/plextraktsync/config/HttpCacheConfig.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.3/plextraktsync/config/ServerConfig.py` & `PlexTraktSync-0.26.4/plextraktsync/config/ServerConfig.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.3/plextraktsync/config/SyncConfig.py` & `PlexTraktSync-0.26.4/plextraktsync/config/SyncConfig.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.3/plextraktsync/config.default.yml` & `PlexTraktSync-0.26.4/plextraktsync/config.default.yml`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.3/plextraktsync/decorators/rate_limit.py` & `PlexTraktSync-0.26.4/plextraktsync/decorators/rate_limit.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.3/plextraktsync/decorators/retry.py` & `PlexTraktSync-0.26.4/plextraktsync/decorators/retry.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.3/plextraktsync/logger/filter.py` & `PlexTraktSync-0.26.4/plextraktsync/logger/filter.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.3/plextraktsync/logging.py` & `PlexTraktSync-0.26.4/plextraktsync/logging.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.3/plextraktsync/media.py` & `PlexTraktSync-0.26.4/plextraktsync/media.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.3/plextraktsync/mixin/ChangeNotifier.py` & `PlexTraktSync-0.26.4/plextraktsync/mixin/ChangeNotifier.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.3/plextraktsync/plex/PlexApi.py` & `PlexTraktSync-0.26.4/plextraktsync/plex/PlexApi.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.3/plextraktsync/plex/PlexAudioCodec.py` & `PlexTraktSync-0.26.4/plextraktsync/plex/PlexAudioCodec.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.3/plextraktsync/plex/PlexGuid.py` & `PlexTraktSync-0.26.4/plextraktsync/plex/PlexGuid.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.3/plextraktsync/plex/PlexLibraryItem.py` & `PlexTraktSync-0.26.4/plextraktsync/plex/PlexLibraryItem.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.3/plextraktsync/plex/PlexLibrarySection.py` & `PlexTraktSync-0.26.4/plextraktsync/plex/PlexLibrarySection.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.3/plextraktsync/plex/PlexRatings.py` & `PlexTraktSync-0.26.4/plextraktsync/plex/PlexRatings.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.3/plextraktsync/plex/PlexServerConnection.py` & `PlexTraktSync-0.26.4/plextraktsync/plex/PlexServerConnection.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         # if connection fails, it will try:
         # 1. url expected by new ssl certificate
         # 2. url without ssl
         # 3. local url (localhost)
         for url in urls:
             self.logger.debug(f"Trying url: {url}")
             try:
-                return PlexServer(baseurl=url, token=token, session=self.session)
+                return PlexServer(baseurl=url, token=token, session=self.session, timeout=self.timeout)
             except SSLError as e:
                 self.logger.error(e)
                 message = str(e.__context__)
 
                 # 1.
                 # HTTPSConnectionPool(host='127.0.0.1', port=32400):
                 # Max retries exceeded with url: / (
```

### Comparing `PlexTraktSync-0.26.3/plextraktsync/plex/PlexWatchList.py` & `PlexTraktSync-0.26.4/plextraktsync/plex/PlexWatchList.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.3/plextraktsync/plex/SessionCollection.py` & `PlexTraktSync-0.26.4/plextraktsync/plex/SessionCollection.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.3/plextraktsync/pytrakt_extensions.py` & `PlexTraktSync-0.26.4/plextraktsync/pytrakt_extensions.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.3/plextraktsync/queue/BackgroundTask.py` & `PlexTraktSync-0.26.4/plextraktsync/queue/BackgroundTask.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.3/plextraktsync/queue/Queue.py` & `PlexTraktSync-0.26.4/plextraktsync/queue/Queue.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.3/plextraktsync/queue/TraktBatchWorker.py` & `PlexTraktSync-0.26.4/plextraktsync/queue/TraktBatchWorker.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.3/plextraktsync/queue/TraktMarkWatchedWorker.py` & `PlexTraktSync-0.26.4/plextraktsync/queue/TraktMarkWatchedWorker.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.3/plextraktsync/rich_addons.py` & `PlexTraktSync-0.26.4/plextraktsync/rich_addons.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.3/plextraktsync/sync.py` & `PlexTraktSync-0.26.4/plextraktsync/sync.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.3/plextraktsync/trakt/ScrobblerCollection.py` & `PlexTraktSync-0.26.4/plextraktsync/trakt/ScrobblerCollection.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.3/plextraktsync/trakt/ScrobblerProxy.py` & `PlexTraktSync-0.26.4/plextraktsync/trakt/ScrobblerProxy.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.3/plextraktsync/trakt/TraktApi.py` & `PlexTraktSync-0.26.4/plextraktsync/trakt/TraktApi.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.3/plextraktsync/trakt/TraktItem.py` & `PlexTraktSync-0.26.4/plextraktsync/trakt/TraktItem.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.3/plextraktsync/trakt/TraktLookup.py` & `PlexTraktSync-0.26.4/plextraktsync/trakt/TraktLookup.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.3/plextraktsync/trakt/TraktRatingCollection.py` & `PlexTraktSync-0.26.4/plextraktsync/trakt/TraktRatingCollection.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.3/plextraktsync/trakt/TraktWatchlist.py` & `PlexTraktSync-0.26.4/plextraktsync/trakt/TraktWatchlist.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.3/plextraktsync/trakt_list_util.py` & `PlexTraktSync-0.26.4/plextraktsync/trakt_list_util.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.3/plextraktsync/util/Factory.py` & `PlexTraktSync-0.26.4/plextraktsync/util/Factory.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.3/plextraktsync/util/Path.py` & `PlexTraktSync-0.26.4/plextraktsync/util/Path.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.3/plextraktsync/util/Timer.py` & `PlexTraktSync-0.26.4/plextraktsync/util/Timer.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.3/plextraktsync/util/Version.py` & `PlexTraktSync-0.26.4/plextraktsync/util/Version.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.3/plextraktsync/util/expand_id.py` & `PlexTraktSync-0.26.4/plextraktsync/util/expand_id.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.3/plextraktsync/util/local_url.py` & `PlexTraktSync-0.26.4/plextraktsync/util/local_url.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.3/plextraktsync/util/openurl.py` & `PlexTraktSync-0.26.4/plextraktsync/util/openurl.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.3/plextraktsync/util/packaging.py` & `PlexTraktSync-0.26.4/plextraktsync/util/packaging.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.3/plextraktsync/util/remove_empty_values.py` & `PlexTraktSync-0.26.4/plextraktsync/util/remove_empty_values.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.3/plextraktsync/walker.py` & `PlexTraktSync-0.26.4/plextraktsync/walker.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.3/plextraktsync/watch/EventDispatcher.py` & `PlexTraktSync-0.26.4/plextraktsync/watch/EventDispatcher.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.3/plextraktsync/watch/EventFactory.py` & `PlexTraktSync-0.26.4/plextraktsync/watch/EventFactory.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.3/plextraktsync/watch/ProgressBar.py` & `PlexTraktSync-0.26.4/plextraktsync/watch/ProgressBar.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.3/plextraktsync/watch/WatchStateUpdater.py` & `PlexTraktSync-0.26.4/plextraktsync/watch/WatchStateUpdater.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.3/plextraktsync/watch/WebSocketListener.py` & `PlexTraktSync-0.26.4/plextraktsync/watch/WebSocketListener.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.3/plextraktsync/watch/events.py` & `PlexTraktSync-0.26.4/plextraktsync/watch/events.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.3/requirements.txt` & `PlexTraktSync-0.26.4/requirements.txt`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.3/setup.cfg` & `PlexTraktSync-0.26.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.3/tests/test_collection_metadata.py` & `PlexTraktSync-0.26.4/tests/test_collection_metadata.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.3/tests/test_config.py` & `PlexTraktSync-0.26.4/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.3/tests/test_events.py` & `PlexTraktSync-0.26.4/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.3/tests/test_new_agent.py` & `PlexTraktSync-0.26.4/tests/test_new_agent.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.3/tests/test_timer.py` & `PlexTraktSync-0.26.4/tests/test_timer.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.3/tests/test_trakt_progress.py` & `PlexTraktSync-0.26.4/tests/test_trakt_progress.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.3/tests/test_tv_lookup.py` & `PlexTraktSync-0.26.4/tests/test_tv_lookup.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.3/tests/test_walker.py` & `PlexTraktSync-0.26.4/tests/test_walker.py`

 * *Files identical despite different names*

