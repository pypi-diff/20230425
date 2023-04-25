# Comparing `tmp/rockalyzer-0.0.5.tar.gz` & `tmp/rockalyzer-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rockalyzer-0.0.5.tar", last modified: Thu Apr 20 16:27:25 2023, max compression
+gzip compressed data, was "rockalyzer-0.1.0.tar", last modified: Tue Apr 25 08:53:30 2023, max compression
```

## Comparing `rockalyzer-0.0.5.tar` & `rockalyzer-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 16:27:25.913489 rockalyzer-0.0.5/
--rw-rw-rw-   0        0        0     1089 2023-03-07 15:36:40.000000 rockalyzer-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     2894 2023-04-20 16:27:25.912489 rockalyzer-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     2209 2023-04-20 16:25:18.000000 rockalyzer-0.0.5/README.md
--rw-rw-rw-   0        0        0       42 2023-04-20 16:27:25.913489 rockalyzer-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1110 2023-04-20 16:25:37.000000 rockalyzer-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-20 16:27:25.908394 rockalyzer-0.0.5/src/
--rw-rw-rw-   0        0        0    32560 2023-03-30 15:25:48.000000 rockalyzer-0.0.5/src/Action.py
--rw-rw-rw-   0        0        0    66093 2023-04-20 15:27:08.000000 rockalyzer-0.0.5/src/Game.py
--rw-rw-rw-   0        0        0      205 2023-03-27 18:56:29.000000 rockalyzer-0.0.5/src/console_colors.py
--rw-rw-rw-   0        0        0     4048 2023-04-20 08:11:58.000000 rockalyzer-0.0.5/src/constants.py
-drwxrwxrwx   0        0        0        0 2023-04-20 16:27:25.911488 rockalyzer-0.0.5/src/rockalyzer.egg-info/
--rw-rw-rw-   0        0        0     2894 2023-04-20 16:27:25.000000 rockalyzer-0.0.5/src/rockalyzer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      298 2023-04-20 16:27:25.000000 rockalyzer-0.0.5/src/rockalyzer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 16:27:25.000000 rockalyzer-0.0.5/src/rockalyzer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-04-20 16:27:25.000000 rockalyzer-0.0.5/src/rockalyzer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       48 2023-04-20 16:27:25.000000 rockalyzer-0.0.5/src/rockalyzer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4948 2023-04-20 08:08:30.000000 rockalyzer-0.0.5/src/rockalyzer.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:53:30.210686 rockalyzer-0.1.0/
+-rw-rw-rw-   0        0        0     1089 2023-03-07 15:36:40.000000 rockalyzer-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0     2911 2023-04-25 08:53:30.210686 rockalyzer-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2226 2023-04-25 08:46:21.000000 rockalyzer-0.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-25 08:53:30.212188 rockalyzer-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1112 2023-04-25 08:52:48.000000 rockalyzer-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:53:30.208686 rockalyzer-0.1.0/src/
+-rw-rw-rw-   0        0        0    66227 2023-04-25 08:45:49.000000 rockalyzer-0.1.0/src/Game.py
+-rw-rw-rw-   0        0        0    33118 2023-04-25 08:38:39.000000 rockalyzer-0.1.0/src/RLObject.py
+-rw-rw-rw-   0        0        0      205 2023-03-27 18:56:29.000000 rockalyzer-0.1.0/src/console_colors.py
+-rw-rw-rw-   0        0        0     4048 2023-04-20 08:11:58.000000 rockalyzer-0.1.0/src/constants.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:53:30.210686 rockalyzer-0.1.0/src/rockalyzer.egg-info/
+-rw-rw-rw-   0        0        0     2911 2023-04-25 08:53:30.000000 rockalyzer-0.1.0/src/rockalyzer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      300 2023-04-25 08:53:30.000000 rockalyzer-0.1.0/src/rockalyzer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 08:53:30.000000 rockalyzer-0.1.0/src/rockalyzer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-04-25 08:53:30.000000 rockalyzer-0.1.0/src/rockalyzer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       50 2023-04-25 08:53:30.000000 rockalyzer-0.1.0/src/rockalyzer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5209 2023-04-25 08:45:30.000000 rockalyzer-0.1.0/src/rockalyzer.py
```

### Comparing `rockalyzer-0.0.5/LICENSE` & `rockalyzer-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rockalyzer-0.0.5/PKG-INFO` & `rockalyzer-0.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rockalyzer
-Version: 0.0.5
+Version: 0.1.0
 Summary: Rocket League Boxcars-Replay Analyzer
 Home-page: https://github.com/eliastheis/rockalyzer
 Author: Elias Theis
 Author-email: mail@eliastheis.de
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -52,19 +52,19 @@
 Make sure you parsed the replay to a json file first using one of the tools mentioned above.
 ```python
 from rockalyzer import Replayer
 
 # load replay as JSON file and set render mode
 replayer = Replayer('path/to/replay.json', render=True)
 
-# replay file
-replayer.replay()
+# print header infos
+replayer.print_header_info()
 
-# get stats
-stats = replayer.get_stats()
+# replay file
+stats = replayer.replay()
 ```
 
 ### Simple render
 If you set `render=True` when creating the `Replayer`-object, you get a simple (almost real-time) render of the game using [matplotlib](https://matplotlib.org/)
 ![Screenshot of render](https://raw.githubusercontent.com/eliastheis/rockalyzer/master/render_screenshot.png)
 
 ## Build and upload package to PyPi
```

### Comparing `rockalyzer-0.0.5/README.md` & `rockalyzer-0.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -34,19 +34,19 @@
 Make sure you parsed the replay to a json file first using one of the tools mentioned above.
 ```python
 from rockalyzer import Replayer
 
 # load replay as JSON file and set render mode
 replayer = Replayer('path/to/replay.json', render=True)
 
-# replay file
-replayer.replay()
+# print header infos
+replayer.print_header_info()
 
-# get stats
-stats = replayer.get_stats()
+# replay file
+stats = replayer.replay()
 ```
 
 ### Simple render
 If you set `render=True` when creating the `Replayer`-object, you get a simple (almost real-time) render of the game using [matplotlib](https://matplotlib.org/)
 ![Screenshot of render](https://raw.githubusercontent.com/eliastheis/rockalyzer/master/render_screenshot.png)
 
 ## Build and upload package to PyPi
```

### Comparing `rockalyzer-0.0.5/setup.py` & `rockalyzer-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 
 # read the contents of your README file for the long description
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setup(
     name='rockalyzer',
-    version='0.0.5',
+    version='0.1.0',
     description='Rocket League Boxcars-Replay Analyzer',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/eliastheis/rockalyzer',
     author='Elias Theis',
     author_email='mail@eliastheis.de',
-    py_modules=['rockalyzer', 'Game', 'Action', 'console_colors', 'constants'],
+    py_modules=['rockalyzer', 'Game', 'RLObject', 'console_colors', 'constants'],
     package_dir={'': 'src'},
     install_requires=[
         'numpy',
         'matplotlib',
     ],
     classifiers=[
         'Programming Language :: Python :: 3',
```

### Comparing `rockalyzer-0.0.5/src/Game.py` & `rockalyzer-0.1.0/src/Game.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from json import dump as json_dump
 from matplotlib import pyplot as plt
 import numpy as np
 import math
 
 from console_colors import *
 from constants import *
-from Action import Action
+from RLObject import RLObject
 
 
 class Game:
 
     def __init__(self, json_content, render, debug_print=False, event_print=False):
         self.num_frames = len(json_content['network_frames']['frames'])
         self.object_lookup = json_content['objects']
@@ -99,18 +99,14 @@
 
         # snapshot values
         self.snapshot_values()
 
         # check for events
         self.check_for_events()
 
-        #if frame_index == 4900: # (first goal)
-        #    self.dump_actors_into_json()
-        #    exit()
-
 
     def delete_actors(self, actors):
         for actor in actors:
             actor_id = actor
             object_name = self.actors[actor_id]['object_name']
             if self.debug_print:
                 print(f'[-] Deleting {object_name} ({actor_id})')
@@ -150,110 +146,110 @@
 
         for actor in actors:
             actor_id = actor['actor_id']
             object_name = self.object_lookup[actor['object_id']]
 
             match actor['object_id']:
 
-                case Action.Engine_Actor_RemoteRole:
+                case RLObject.Engine_Actor_RemoteRole:
                     self.actors[actor_id]['remote_role'] = actor['attribute']['Enum']
                 
-                case Action.Engine_Actor_DrawScale:
+                case RLObject.Engine_Actor_DrawScale:
                     self.actors[actor_id]['draw_scale'] = actor['attribute']['Float']
 
-                case Action.TAGame_CarComponent_TA_Vehicle:
+                case RLObject.TAGame_CarComponent_TA_Vehicle:
                     self.actors[actor_id]['parent_ids'].append(actor['attribute']['ActiveActor']['actor'])
                     
-                case Action.TAGame_CarComponent_TA_ReplicatedActive:
+                case RLObject.TAGame_CarComponent_TA_ReplicatedActive:
                     self.actors[actor_id]['active'] = actor['attribute']['Byte']
 
-                case Action.TAGame_CarComponent_Boost_TA_ReplicatedBoostAmount:
+                case RLObject.TAGame_CarComponent_Boost_TA_ReplicatedBoostAmount:
                     self.actors[actor_id]['boost'] = actor['attribute']['Byte']
                 
-                case Action.TAGame_GameEvent_TA_ReplicatedRoundCountDownNumber:
+                case RLObject.TAGame_GameEvent_TA_ReplicatedRoundCountDownNumber:
                     self.actors[actor_id]['round_countdown'] = actor['attribute']['Int']
                 
-                case Action.TAGame_GameEvent_TA_ReplicatedGameStateTimeRemaining:
+                case RLObject.TAGame_GameEvent_TA_ReplicatedGameStateTimeRemaining:
                     self.actors[actor_id]['time_remaining'] = actor['attribute']['Int']
                 
-                case Action.TAGame_GameEvent_TA_ReplicatedStateName:
+                case RLObject.TAGame_GameEvent_TA_ReplicatedStateName:
                     self.actors[actor_id]['stateName'] = actor['attribute']['Int']
                 
-                case Action.TAGame_GameEvent_TA_BotSkill:
+                case RLObject.TAGame_GameEvent_TA_BotSkill:
                     self.actors[actor_id]['bot_skill'] = actor['attribute']['Int']
                 
-                case Action.TAGame_GameEvent_TA_bHasLeaveMatchPenalty:
+                case RLObject.TAGame_GameEvent_TA_bHasLeaveMatchPenalty:
                     self.actors[actor_id]['has_leave_match_penalty'] = actor['attribute']['Boolean']
                 
-                case Action.TAGame_GameEvent_Team_TA_MaxTeamSize:
+                case RLObject.TAGame_GameEvent_Team_TA_MaxTeamSize:
                     self.actors[actor_id]['max_team_size'] = actor['attribute']['Int']
                 
-                case Action.TAGame_GameEvent_Soccar_TA_RoundNum:
+                case RLObject.TAGame_GameEvent_Soccar_TA_RoundNum:
                     self.actors[actor_id]['current_round'] = actor['attribute']['Int']
                 
-                case Action.TAGame_GameEvent_Soccar_TA_bBallHasBeenHit:
+                case RLObject.TAGame_GameEvent_Soccar_TA_bBallHasBeenHit:
                     # this event is not triggered when the ball is hit, but when the ball is hit at kickoff
                     # and at some random times
                     self.actors[actor_id]['ball_has_been_hit'] = actor['attribute']['Boolean']
                 
-                case Action.TAGame_GameEvent_Soccar_TA_SecondsRemaining:
+                case RLObject.TAGame_GameEvent_Soccar_TA_SecondsRemaining:
                     self.seconds_remaining = actor['attribute']['Int']
                     self.actors[actor_id]['seconds_remaining'] = actor['attribute']['Int']
                 
-                case Action.Engine_Pawn_PlayerReplicationInfo:
+                case RLObject.Engine_Pawn_PlayerReplicationInfo:
                     self.actors[actor_id]['parent_ids'].append(actor['attribute']['ActiveActor']['actor'])
                 
-                case Action.TAGame_RBActor_TA_ReplicatedRBState:
+                case RLObject.TAGame_RBActor_TA_ReplicatedRBState:
                     # if the new linear_velocity is None then we do not update the linear_velocity
                     if actor['attribute']['RigidBody']['linear_velocity'] is None:
                         del actor['attribute']['RigidBody']['linear_velocity']
                     self.actors[actor_id].update(actor['attribute']['RigidBody'])
 
-                case Action.TAGame_Vehicle_TA_ReplicatedSteer:
+                case RLObject.TAGame_Vehicle_TA_ReplicatedSteer:
                     self.actors[actor_id]['steer'] = actor['attribute']['Byte']
                 
-                case Action.TAGame_Vehicle_TA_ReplicatedThrottle:
+                case RLObject.TAGame_Vehicle_TA_ReplicatedThrottle:
                     self.actors[actor_id]['throttle'] = actor['attribute']['Byte']
                 
-                case Action.TAGame_Vehicle_TA_bReplicatedHandbrake:
+                case RLObject.TAGame_Vehicle_TA_bReplicatedHandbrake:
                     self.actors[actor_id]['handbrake'] = actor['attribute']['Boolean']
                 
-                case Action.TAGame_Vehicle_TA_bDriving:
+                case RLObject.TAGame_Vehicle_TA_bDriving:
                     self.actors[actor_id]['driving'] = actor['attribute']['Boolean']
                 
-                case Action.TAGame_Car_TA_RumblePickups:
+                case RLObject.TAGame_Car_TA_RumblePickups:
                     # IGNORE Rumble stuff
                     pass
             
-                case Action.TAGame_Car_TA_TeamPaint:
+                case RLObject.TAGame_Car_TA_TeamPaint:
                     self.actors[actor_id]['team_paint'] = actor['attribute']['TeamPaint']
                     self.actors[actor_id]['team'] = actor['attribute']['TeamPaint']['team']
                 
-                case Action.TAGame_CameraSettingsActor_TA_CameraYaw:
+                case RLObject.TAGame_CameraSettingsActor_TA_CameraYaw:
                     self.actors[actor_id]['camera_yaw'] = actor['attribute']['Byte']
                 
-                case Action.TAGame_CameraSettingsActor_TA_CameraPitch:
+                case RLObject.TAGame_CameraSettingsActor_TA_CameraPitch:
                     self.actors[actor_id]['camera_pitch'] = actor['attribute']['Byte']
                 
-                case Action.TAGame_CameraSettingsActor_TA_bMouseCameraToggleEnabled:
+                case RLObject.TAGame_CameraSettingsActor_TA_bMouseCameraToggleEnabled:
                     self.actors[actor_id]['camera_toggle'] = actor['attribute']['Boolean']
                 
-                case Action.TAGame_CameraSettingsActor_TA_bUsingSwivel:
+                case RLObject.TAGame_CameraSettingsActor_TA_bUsingSwivel:
                     self.actors[actor_id]['using_swivel'] = actor['attribute']['Boolean']
                 
-                case Action.TAGame_CameraSettingsActor_TA_bUsingBehindView:
+                case RLObject.TAGame_CameraSettingsActor_TA_bUsingBehindView:
                     self.actors[actor_id]['using_behind_view'] = actor['attribute']['Boolean']
                 
-                case Action.TAGame_CameraSettingsActor_TA_ProfileSettings:
+                case RLObject.TAGame_CameraSettingsActor_TA_ProfileSettings:
                     self.actors[actor_id]['camera_settings'] = actor['attribute']['CamSettings']
                 
-                case Action.TAGame_CameraSettingsActor_TA_bUsingSecondaryCamera:
+                case RLObject.TAGame_CameraSettingsActor_TA_bUsingSecondaryCamera:
                     self.actors[actor_id]['using_ball_cam'] = actor['attribute']['Boolean']
                 
-                case Action.Engine_PlayerReplicationInfo_UniqueId:
+                case RLObject.Engine_PlayerReplicationInfo_UniqueId:
                     self.actors[actor_id]['unique_id'] = actor['attribute']['UniqueId']
                     # check for MMR in debug_info
                     remote_id = self.actors[actor_id]['unique_id']['remote_id']
                     id = None
                     if 'Epic' in remote_id:
                         id = remote_id['Epic']
                     elif 'Steam' in remote_id:
@@ -268,91 +264,91 @@
                         for info in self.debug_info:
                             if id in info['user']:
                                 self.actors[actor_id]['mmr'] = info['text']
                     else:
                         print(WARNING, 'Unknown remote_id type ', ENDC,  str(remote_id))
                         exit()
                 
-                case Action.Engine_PlayerReplicationInfo_Team:
+                case RLObject.Engine_PlayerReplicationInfo_Team:
                     self.actors[actor_id]['team'] = actor['attribute']['ActiveActor']['actor']
                 
-                case Action.Engine_PlayerReplicationInfo_PlayerID:
+                case RLObject.Engine_PlayerReplicationInfo_PlayerID:
                     self.actors[actor_id]['player_id'] = actor['attribute']['Int']
                 
-                case Action.Engine_PlayerReplicationInfo_PlayerName:
+                case RLObject.Engine_PlayerReplicationInfo_PlayerName:
                     self.actors[actor_id]['player_name'] = actor['attribute']['String']
                 
-                case Action.Engine_PlayerReplicationInfo_Ping:
+                case RLObject.Engine_PlayerReplicationInfo_Ping:
                     self.actors[actor_id]['ping'] = actor['attribute']['Byte']
                 
-                case Action.TAGame_PRI_TA_CurrentVoiceRoom:
+                case RLObject.TAGame_PRI_TA_CurrentVoiceRoom:
                     self.actors[actor_id]['current_voice_room'] = actor['attribute']['String']
                 
-                case Action.TAGame_PRI_TA_SpectatorShortcut:
+                case RLObject.TAGame_PRI_TA_SpectatorShortcut:
                     self.actors[actor_id]['spectator_shortcut'] = actor['attribute']['Int']
                 
-                case Action.TAGame_PRI_TA_SteeringSensitivity:
+                case RLObject.TAGame_PRI_TA_SteeringSensitivity:
                     self.actors[actor_id]['steering_sensitivity'] = actor['attribute']['Float']
                 
-                case Action.TAGame_PRI_TA_Title:
+                case RLObject.TAGame_PRI_TA_Title:
                     self.actors[actor_id]['title'] = actor['attribute']['Int']
                 
-                case Action.TAGame_PRI_TA_PartyLeader:
+                case RLObject.TAGame_PRI_TA_PartyLeader:
                     self.actors[actor_id]['party_leader_id'] = actor['attribute']['PartyLeader']
                
-                case Action.TAGame_PRI_TA_ClientLoadoutsOnline:
+                case RLObject.TAGame_PRI_TA_ClientLoadoutsOnline:
                     self.actors[actor_id]['loadout_online'] = actor['attribute']['LoadoutsOnline']
                 
-                case Action.TAGame_PRI_TA_ClientLoadouts:
+                case RLObject.TAGame_PRI_TA_ClientLoadouts:
                     self.actors[actor_id]['team_loadout'] = actor['attribute']['TeamLoadout']
                 
-                case Action.TAGame_PRI_TA_ReplicatedGameEvent:
+                case RLObject.TAGame_PRI_TA_ReplicatedGameEvent:
                     other_actor_id = actor['attribute']['ActiveActor']['actor']
                     if other_actor_id != -1:
                         if 'frames_with_event' not in self.actors[other_actor_id]:
                             self.actors[other_actor_id]['frames_with_event'] = []
                         self.actors[other_actor_id]['frames_with_event'].append(self.frame_index)
                 
-                case Action.TAGame_PRI_TA_PlayerHistoryValid:
+                case RLObject.TAGame_PRI_TA_PlayerHistoryValid:
                     self.actors[actor_id]['player_history_valid'] = actor['attribute']['Boolean']
                 
-                case Action.TAGame_PRI_TA_MatchScore:
+                case RLObject.TAGame_PRI_TA_MatchScore:
                     self.actors[actor_id]['score'] = actor['attribute']['Int']
                 
-                case Action.TAGame_Ball_TA_HitTeamNum:
+                case RLObject.TAGame_Ball_TA_HitTeamNum:
                     self.actors[actor_id]['hit_team_num'] = actor['attribute']['Byte']
                 
-                case Action.TAGame_CarComponent_Dodge_TA_DodgeTorque:
+                case RLObject.TAGame_CarComponent_Dodge_TA_DodgeTorque:
                     self.actors[actor_id]['location'] = actor['attribute']['Location']
                 
-                case Action.Engine_GameReplicationInfo_ServerName:
+                case RLObject.Engine_GameReplicationInfo_ServerName:
                     self.actors[actor_id]['server'] = actor['attribute']['String']
                 
-                case Action.ProjectX_GRI_X_MatchGuid:
+                case RLObject.ProjectX_GRI_X_MatchGuid:
                     self.actors[actor_id]['match_guid'] = actor['attribute']['String']
                 
-                case Action.ProjectX_GRI_X_bGameStarted:
+                case RLObject.ProjectX_GRI_X_bGameStarted:
                     self.actors[actor_id]['game_started'] = actor['attribute']['Boolean']
                 
-                case Action.ProjectX_GRI_X_GameServerID:
+                case RLObject.ProjectX_GRI_X_GameServerID:
                     if 'QWord' in actor['attribute']:
                         self.actors[actor_id]['server_id'] = actor['attribute']['QWord']
                     elif 'String' in actor['attribute']:
                         self.actors[actor_id]['server_id'] = actor['attribute']['String']
                     else:
                         print(WARNING, 'Unknown GameServerID type (should be String or QWord)', ENDC, str(actor['attribute']))
                         exit()
 
-                case Action.ProjectX_GRI_X_Reservations:
+                case RLObject.ProjectX_GRI_X_Reservations:
                     self.actors[actor_id]['reservation'] = actor['attribute']['Reservation']
                 
-                case Action.ProjectX_GRI_X_ReplicatedServerRegion:
+                case RLObject.ProjectX_GRI_X_ReplicatedServerRegion:
                     self.actors[actor_id]['region'] = actor['attribute']['String']
 
-                case Action.ProjectX_GRI_X_ReplicatedGamePlaylist:
+                case RLObject.ProjectX_GRI_X_ReplicatedGamePlaylist:
 
                     game_playlist_id = actor['attribute']['Int']
                     game_playlist = 'unknown'
 
                     if game_playlist_id == GAME_PLAYLIST_CASUAL_DUEL:
                         game_playlist = 'casual_duel'
                     elif game_playlist_id == GAME_PLAYLIST_CASUAL_DOUBLE:
@@ -376,307 +372,307 @@
                     
                     if self.game_playlist is not None and self.game_playlist != game_playlist:
                         print(WARNING, 'Game playlist changed from', self.game_playlist, 'to', game_playlist, ENDC)
                         exit()
                     else:
                         self.game_playlist = game_playlist
                 
-                case Action.TAGame_Team_TA_GameEvent:
+                case RLObject.TAGame_Team_TA_GameEvent:
                     other_actor_id = actor['attribute']['ActiveActor']['actor']
                     if 'frames_with_event' not in self.actors[other_actor_id]:
                         self.actors[other_actor_id]['frames_with_event'] = []
                     self.actors[other_actor_id]['frames_with_event'].append(self.frame_index)
                 
-                case Action.TAGame_VehiclePickup_TA_NewReplicatedPickupData:
+                case RLObject.TAGame_VehiclePickup_TA_NewReplicatedPickupData:
                     instigator_id = actor['attribute']['PickupNew']['instigator']
                     if instigator_id is not None: # for whatever reason, instigator_id can be None
                         if instigator_id != -1: # for whatever reason, instigator_id can be -1
                             if 'boost_pickups' not in self.actors[instigator_id]:
                                 self.actors[instigator_id]['boost_pickups'] = []
                             picked_up = actor['attribute']['PickupNew']['picked_up']
                             boost_actor_id = actor['actor_id']
                             data = {'picked_up': picked_up, 'frame_index': self.time, 'boost_actor_id': boost_actor_id}
                             self.actors[instigator_id]['boost_pickups'].append(data)
 
-                case Action.TAGame_PRI_TA_PersistentCamera:
+                case RLObject.TAGame_PRI_TA_PersistentCamera:
                     self.actors[actor_id]['parent_ids'].append(actor['attribute']['ActiveActor']['actor'])
                 
-                case Action.TAGame_CameraSettingsActor_TA_PRI:
+                case RLObject.TAGame_CameraSettingsActor_TA_PRI:
                     self.actors[actor_id]['parent_ids'].append(actor['attribute']['ActiveActor']['actor'])
                 
-                case Action.TAGame_Ball_TA_GameEvent:
+                case RLObject.TAGame_Ball_TA_GameEvent:
                     self.actors[actor_id]['parent_ids'].append(actor['attribute']['ActiveActor']['actor'])
                 
-                case Action.TAGame_PRI_TA_MatchGoals:
+                case RLObject.TAGame_PRI_TA_MatchGoals:
                     event_goal = True
                     self.actors[actor_id]['match_goals'] = actor['attribute']['Int']
                 
-                case Action.TAGame_PRI_TA_MatchAssists:
+                case RLObject.TAGame_PRI_TA_MatchAssists:
                     self.actors[actor_id]['match_assists'] = actor['attribute']['Int']
                 
-                case Action.TAGame_PRI_TA_MatchSaves:
+                case RLObject.TAGame_PRI_TA_MatchSaves:
                     self.actors[actor_id]['match_saves'] = actor['attribute']['Int']
                 
-                case Action.TAGame_PRI_TA_MatchShots:
+                case RLObject.TAGame_PRI_TA_MatchShots:
                     self.actors[actor_id]['match_shots'] = actor['attribute']['Int']
                 
-                case Action.Engine_PlayerReplicationInfo_Score:
+                case RLObject.Engine_PlayerReplicationInfo_Score:
                     self.actors[actor_id]['score'] = actor['attribute']['Int']
                 
-                case Action.Engine_TeamInfo_Score:
+                case RLObject.Engine_TeamInfo_Score:
                     self.actors[actor_id]['score'] = actor['attribute']['Int']
                 
-                case Action.TAGame_GameEvent_TA_bCanVoteToForfeit:
+                case RLObject.TAGame_GameEvent_TA_bCanVoteToForfeit:
                     self.actors[actor_id]['can_vote_to_forfeit'] = actor['attribute']['Boolean']
                 
-                case Action.TAGame_Car_TA_ReplicatedDemolishGoalExplosion:
+                case RLObject.TAGame_Car_TA_ReplicatedDemolishGoalExplosion:
                     self.actors[actor_id]['demolish_fx'] = actor['attribute']['DemolishFx']
                 
-                case Action.TAGame_GameEvent_Soccar_TA_ReplicatedScoredOnTeam:
+                case RLObject.TAGame_GameEvent_Soccar_TA_ReplicatedScoredOnTeam:
                     self.actors[actor_id]['scored_on_team'] = actor['attribute']['Byte']
                 
-                case Action.Engine_Actor_bCollideActors:
+                case RLObject.Engine_Actor_bCollideActors:
                     self.actors[actor_id]['collide_actors'] = actor['attribute']['Boolean']
                 
-                case Action.Engine_Actor_bBlockActors:
+                case RLObject.Engine_Actor_bBlockActors:
                     self.actors[actor_id]['block_actors'] = actor['attribute']['Boolean']
                 
-                case Action.TAGame_Ball_TA_ReplicatedExplosionDataExtended:
+                case RLObject.TAGame_Ball_TA_ReplicatedExplosionDataExtended:
                     self.actors[actor_id]['extended_explosion'] = actor['attribute']['ExtendedExplosion']
                 
-                case Action.Engine_Actor_bHidden:
+                case RLObject.Engine_Actor_bHidden:
                     if actor['attribute']['Boolean'] != True:
                         print(WARNING + 'Actor ' + str(actor_id) + ' is not hidden' + ENDC)
                         exit()
                     self.actors[actor_id]['hidden_since_frame'] = self.frame_index
                 
-                case Action.TAGame_PRI_TA_bReady:
+                case RLObject.TAGame_PRI_TA_bReady:
                     self.actors[actor_id]['ready'] = actor['attribute']['Boolean']
 
-                case Action.TAGame_PRI_TA_ReplicatedWorstNetQualityBeyondLatency:
+                case RLObject.TAGame_PRI_TA_ReplicatedWorstNetQualityBeyondLatency:
                     self.actors[actor_id]['worst_net_quality_beyond_latency'] = actor['attribute']['Byte']
                 
-                case Action.TAGame_CarComponent_FlipCar_TA_FlipCarTime:
+                case RLObject.TAGame_CarComponent_FlipCar_TA_FlipCarTime:
                     self.actors[actor_id]['flip_car_time'] = actor['attribute']['Float']
                 
-                case Action.TAGame_GameEvent_Soccar_TA_MaxScore:
+                case RLObject.TAGame_GameEvent_Soccar_TA_MaxScore:
                     self.actors[actor_id]['max_score'] = actor['attribute']['Int']
                 
-                case Action.TAGame_Team_TA_ClubColors:
+                case RLObject.TAGame_Team_TA_ClubColors:
                     self.actors[actor_id]['club_colors'] = actor['attribute']['ClubColors']
 
-                case Action.TAGame_Car_TA_ClubColors:
+                case RLObject.TAGame_Car_TA_ClubColors:
                     self.actors[actor_id]['club_colors'] = actor['attribute']['ClubColors']
                 
-                case Action.ProjectX_GRI_X_ReplicatedGameMutatorIndex:
+                case RLObject.ProjectX_GRI_X_ReplicatedGameMutatorIndex:
                     self.actors[actor_id]['game_mutator_index'] = actor['attribute']['Int']
                 
-                case Action.TAGame_CarComponent_FlipCar_TA_bFlipRight:
+                case RLObject.TAGame_CarComponent_FlipCar_TA_bFlipRight:
                     self.actors[actor_id]['flip_right'] = actor['attribute']['Boolean']
                 
-                case Action.TAGame_PRI_TA_bIsDistracted:
+                case RLObject.TAGame_PRI_TA_bIsDistracted:
                     self.actors[actor_id]['is_distracted'] = actor['attribute']['Boolean']
                 
-                case Action.TAGame_Team_TA_Difficulty:
+                case RLObject.TAGame_Team_TA_Difficulty:
                     self.actors[actor_id]['difficulty'] = actor['attribute']['Int']
                 
-                case Action.TAGame_Team_TA_CustomTeamName:
+                case RLObject.TAGame_Team_TA_CustomTeamName:
                     self.actors[actor_id]['custom_team_name'] = actor['attribute']['String']
                 
-                case Action.ProjectX_GRI_X_MatchGUID:
+                case RLObject.ProjectX_GRI_X_MatchGUID:
                     self.actors[actor_id]['match_guid'] = actor['attribute']['String']
                 
-                case Action.TAGame_GameEvent_Soccar_TA_SeriesLength:
+                case RLObject.TAGame_GameEvent_Soccar_TA_SeriesLength:
                     self.actors[actor_id]['series_length'] = actor['attribute']['Int']
                 
-                case Action.TAGame_CarComponent_Dodge_TA_DodgeImpulse:
+                case RLObject.TAGame_CarComponent_Dodge_TA_DodgeImpulse:
                     self.actors[actor_id]['dodge_impulse_location'] = actor['attribute']['Location']
 
-                case Action.Engine_PlayerReplicationInfo_RemoteUserData:
+                case RLObject.Engine_PlayerReplicationInfo_RemoteUserData:
                     self.actors[actor_id]['remote_user_data'] = actor['attribute']['String']
                 
-                case Action.TAGame_GameEvent_Soccar_TA_bOverTime:
+                case RLObject.TAGame_GameEvent_Soccar_TA_bOverTime:
                     if actor['attribute']['Boolean']:
                         self.actors[actor_id]['over_time_at_frame'] = self.frame_index
                         if self.event_print:
                             print('Overtime!' + ENDC)
                     else:
                         print(WARNING + 'Actor ' + str(actor_id) + ' is not in overtime' + ENDC)
                         exit()
                 
-                case Action.TAGame_GameEvent_Soccar_TA_bClubMatch:
+                case RLObject.TAGame_GameEvent_Soccar_TA_bClubMatch:
                     self.actors[actor_id]['club_match'] = actor['attribute']['Boolean']
                 
-                case Action.TAGame_Team_TA_ClubID:
+                case RLObject.TAGame_Team_TA_ClubID:
                     self.actors[actor_id]['club_id'] = actor['attribute']['Int64']
                 
-                case Action.Engine_PlayerReplicationInfo_bBot:
+                case RLObject.Engine_PlayerReplicationInfo_bBot:
                     self.actors[actor_id]['is_bot'] = actor['attribute']['Boolean']
                 
-                case Action.TAGame_PRI_TA_BotProductName:
+                case RLObject.TAGame_PRI_TA_BotProductName:
                     self.actors[actor_id]['bot_product_name'] = actor['attribute']['Int']
 
-                case Action.TAGame_PRI_TA_ClubID:
+                case RLObject.TAGame_PRI_TA_ClubID:
                     self.actors[actor_id]['club_id'] = actor['attribute']['Int64']
                 
-                case Action.TAGame_GameEvent_Team_TA_bForfeit:
+                case RLObject.TAGame_GameEvent_Team_TA_bForfeit:
                     if actor['attribute']['Boolean']:
                         self.actors[actor_id]['forfeit_at_frame'] = self.frame_index
                     else:
                         print(WARNING + 'Actor ' + str(actor_id) + ' did not forfeit' + ENDC)
                         exit()
                 
-                case Action.TAGame_PRI_TA_PlayerHistoryKey:
+                case RLObject.TAGame_PRI_TA_PlayerHistoryKey:
                     self.actors[actor_id]['player_history_key'] = actor['attribute']['PlayerHistoryKey']
                 
-                case Action.Engine_PlayerReplicationInfo_bTimedOut:
+                case RLObject.Engine_PlayerReplicationInfo_bTimedOut:
                     if actor['attribute']['Boolean']:
                         self.actors[actor_id]['timed_out_at_frame'] = self.frame_index
                     else:
                         print(WARNING + 'Actor ' + str(actor_id) + ' did not time out' + ENDC)
                         exit()
                 
-                case Action.Engine_ReplicatedActor_ORS_ReplicatedOwner:
+                case RLObject.Engine_ReplicatedActor_ORS_ReplicatedOwner:
                     if 'ActiveActor' not in actor['attribute']:
                         print(WARNING, 'Unknown Replicated Owner (should be ActiveActor)', ENDC, str(actor['attribute']))
                         exit()
                     else:
                         self.actors[actor_id]['parent_ids'].append(actor['attribute']['ActiveActor']['actor'])
                 
-                case Action.TAGame_MaxTimeWarningData_TA_EndGameWarningEpochTime:
+                case RLObject.TAGame_MaxTimeWarningData_TA_EndGameWarningEpochTime:
                     #print(WARNING + 'End game warning at frame ' + str(frame_index) + ENDC)
                     self.actors[actor_id]['end_game_warning_epoch_time'] = actor['attribute']['Int64']
                 
-                case Action.TAGame_MaxTimeWarningData_TA_EndGameEpochTime:
+                case RLObject.TAGame_MaxTimeWarningData_TA_EndGameEpochTime:
                     self.actors[actor_id]['end_game_epoch_time'] = actor['attribute']['Int64']
                 
-                case Action.TAGame_Ball_TA_ReplicatedWorldBounceScale:
+                case RLObject.TAGame_Ball_TA_ReplicatedWorldBounceScale:
                     self.actors[actor_id]['world_bounce_scale'] = actor['attribute']['Float']
                 
-                case Action.TAGame_PRI_TA_bIsInSplitScreen:
+                case RLObject.TAGame_PRI_TA_bIsInSplitScreen:
                     self.actors[actor_id]['is_in_split_screen'] = actor['attribute']['Boolean']
                 
-                case Action.TAGame_RBActor_TA_bReplayActor:
+                case RLObject.TAGame_RBActor_TA_bReplayActor:
                     self.actors[actor_id]['is_replay_actor'] = actor['attribute']['Boolean']
                 
-                case Action.TAGame_GameEvent_Soccar_TA_bUnlimitedTime:
+                case RLObject.TAGame_GameEvent_Soccar_TA_bUnlimitedTime:
                     if not actor['attribute']['Boolean']:
                         print(WARNING + 'Actor ' + str(actor_id) + ' is not in unlimited time' + ENDC)
                         exit()
                     self.actors[actor_id]['unlimited_time'] = actor['attribute']['Boolean']
                 
-                case Action.TAGame_CarComponent_Boost_TA_UnlimitedBoostRefCount:
+                case RLObject.TAGame_CarComponent_Boost_TA_UnlimitedBoostRefCount:
                     self.actors[actor_id]['unlimited_boost_ref_count'] = actor['attribute']['Int']
                 
-                case Action.TAGame_VehiclePickup_TA_bNoPickup:
+                case RLObject.TAGame_VehiclePickup_TA_bNoPickup:
                     self.actors[actor_id]['no_pickup'] = actor['attribute']['Boolean']
                 
-                case Action.TAGame_PRI_TA_PawnType:
+                case RLObject.TAGame_PRI_TA_PawnType:
                     self.actors[actor_id]['pawn_type'] = actor['attribute']['Byte']
 
-                case Action.TAGame_CarComponent_Boost_TA_RechargeDelay:
+                case RLObject.TAGame_CarComponent_Boost_TA_RechargeDelay:
                     self.actors[actor_id]['recharge_delay'] = actor['attribute']['Float']
 
-                case Action.TAGame_CarComponent_Boost_TA_RechargeRate:
+                case RLObject.TAGame_CarComponent_Boost_TA_RechargeRate:
                     self.actors[actor_id]['recharge_rate'] = actor['attribute']['Float']
 
-                case Action.TAGame_BreakOutActor_Platform_TA_DamageState:
+                case RLObject.TAGame_BreakOutActor_Platform_TA_DamageState:
                     self.actors[actor_id]['damage_state'] = actor['attribute']['DamageState']
                 
-                case Action.TAGame_Ball_Breakout_TA_LastTeamTouch:
+                case RLObject.TAGame_Ball_Breakout_TA_LastTeamTouch:
                     self.actors[actor_id]['last_team_touch'] = actor['attribute']['Byte']
 
-                case Action.TAGame_PRI_TA_MatchBreakoutDamage:
+                case RLObject.TAGame_PRI_TA_MatchBreakoutDamage:
                     self.actors[actor_id]['match_breakout_damage'] = actor['attribute']['Int']
 
-                case Action.TAGame_Ball_Breakout_TA_AppliedDamage:
+                case RLObject.TAGame_Ball_Breakout_TA_AppliedDamage:
                     self.actors[actor_id]['applied_damage'] = actor['attribute']['AppliedDamage']
                 
-                case Action.TAGame_Ball_Breakout_TA_DamageIndex:
+                case RLObject.TAGame_Ball_Breakout_TA_DamageIndex:
                     self.actors[actor_id]['damage_index'] = actor['attribute']['Int']
 
-                case Action.TAGame_PRI_TA_bUsingItems:
+                case RLObject.TAGame_PRI_TA_bUsingItems:
                     self.actors[actor_id]['using_items'] = actor['attribute']['Boolean']
 
-                case Action.TAGame_RumblePickups_TA_ConcurrentItemCount:
+                case RLObject.TAGame_RumblePickups_TA_ConcurrentItemCount:
                     self.actors[actor_id]['concurrent_item_count'] = actor['attribute']['Int']
                 
-                case Action.TAGame_RumblePickups_TA_PickupInfo:
+                case RLObject.TAGame_RumblePickups_TA_PickupInfo:
                     pickup_info = actor['attribute']['PickupInfo']
                     # IGNORE Rumble stuff
                 
-                case Action.TAGame_CarComponent_TA_ReplicatedActivityTime:
+                case RLObject.TAGame_CarComponent_TA_ReplicatedActivityTime:
                     # probably Rumble stuff
                     self.actors[actor_id]['replicated_activity_time'] = actor['attribute']['Float']
                 
-                case Action.TAGame_SpecialPickup_Targeted_TA_Targeted:
+                case RLObject.TAGame_SpecialPickup_Targeted_TA_Targeted:
                     # IGNORE Rumble stuff
                     pass
             
-                case Action.TAGame_SpecialPickup_BallFreeze_TA_RepOrigSpeed:
+                case RLObject.TAGame_SpecialPickup_BallFreeze_TA_RepOrigSpeed:
                     # IGNORE Rumble stuff
                     pass
 
-                case Action.TAGame_Car_TA_AddedCarForceMultiplier:
+                case RLObject.TAGame_Car_TA_AddedCarForceMultiplier:
                     # IGNORE Rumble stuff
                     pass
             
-                case Action.TAGame_Car_TA_AddedBallForceMultiplier:
+                case RLObject.TAGame_Car_TA_AddedBallForceMultiplier:
                     # IGNORE Rumble stuff
                     pass
             
-                case Action.TAGame_Car_TA_AddedBallForceMultiplier:
+                case RLObject.TAGame_Car_TA_AddedBallForceMultiplier:
                     # IGNORE Rumble stuff
                     pass
 
-                case Action.TAGame_Team_Soccar_TA_GameScore:
+                case RLObject.TAGame_Team_Soccar_TA_GameScore:
                     self.actors[actor_id]['game_score'] = actor['attribute']['Int']
 
-                case Action.TAGame_RBActor_TA_bIgnoreSyncing:
+                case RLObject.TAGame_RBActor_TA_bIgnoreSyncing:
                     self.actors[actor_id]['ignore_syncing'] = actor['attribute']['Boolean']
                 
-                case Action.TAGame_RBActor_TA_WeldedInfo:
+                case RLObject.TAGame_RBActor_TA_WeldedInfo:
                     # probably spikes?
                     self.actors[actor_id]['welded_info'] = actor['attribute']['Welded']
                 
-                case Action.TAGame_SpecialPickup_BallVelcro_TA_AttachTime:
+                case RLObject.TAGame_SpecialPickup_BallVelcro_TA_AttachTime:
                     # probably spikes?
                     self.actors[actor_id]['attach_time'] = actor['attribute']['Float']
                 
-                case Action.TAGame_SpecialPickup_BallVelcro_TA_bHit:
+                case RLObject.TAGame_SpecialPickup_BallVelcro_TA_bHit:
                     # probably spikes?
                     self.actors[actor_id]['hit'] = actor['attribute']['Boolean']
 
-                case Action.TAGame_SpecialPickup_BallVelcro_TA_BreakTime:
+                case RLObject.TAGame_SpecialPickup_BallVelcro_TA_BreakTime:
                     # probably spikes?
                     self.actors[actor_id]['break_time'] = actor['attribute']['Float']
 
-                case Action.TAGame_SpecialPickup_BallVelcro_TA_bBroken:
+                case RLObject.TAGame_SpecialPickup_BallVelcro_TA_bBroken:
                     # probably spikes?
                     self.actors[actor_id]['broken'] = actor['attribute']['Boolean']
                 
-                case Action.TAGame_Car_TA_ReplicatedDemolish_CustomFX:
+                case RLObject.TAGame_Car_TA_ReplicatedDemolish_CustomFX:
                     self.actors[actor_id]['demolish_custom_fx'] = actor['attribute']['DemolishFx']
                 
-                case Action.TAGame_Car_TA_ReplicatedDemolish:
+                case RLObject.TAGame_Car_TA_ReplicatedDemolish:
                     self.actors[actor_id]['demolish'] = actor['attribute']['Demolish']
 
-                case Action.TAGame_GameEvent_TA_MatchTypeClass:
+                case RLObject.TAGame_GameEvent_TA_MatchTypeClass:
                     # pretty weird event
                     pass
             
-                case Action.Engine_GameReplicationInfo_GameClass:
+                case RLObject.Engine_GameReplicationInfo_GameClass:
                     # pretty weird event
                     pass
             
-                case Action.TAGame_GameEvent_Soccar_TA_ReplicatedStatEvent:
+                case RLObject.TAGame_GameEvent_Soccar_TA_ReplicatedStatEvent:
                     # pretty weird event
                     pass
 
-                case Action.TAGame_GameEvent_Soccar_TA_SubRulesArchetype:
+                case RLObject.TAGame_GameEvent_Soccar_TA_SubRulesArchetype:
                     # pretty weird event
                     pass
             
                 case _:
 
                     target_id = actor_id
                     target_object_name = object_name
@@ -955,20 +951,20 @@
             exit(0)
 
 
     def get_player_car_pairs(self):
         player_car_pairs = []
 
         # get all actor_ids from objects with object_id 264
-        players = [actor_id for actor_id, actor in self.actors.items() if actor['object_id'] == Action.TAGame_Default__PRI_TA]
+        players = [actor_id for actor_id, actor in self.actors.items() if actor['object_id'] == RLObject.TAGame_Default__PRI_TA]
 
         for player in players:
             
             # get all children of the player (car)
-            car = [actor_id for actor_id, actor in self.actors.items() if player in actor['parent_ids'] and actor['object_id'] == Action.Archetypes_Car_Car_Default]
+            car = [actor_id for actor_id, actor in self.actors.items() if player in actor['parent_ids'] and actor['object_id'] == RLObject.Archetypes_Car_Car_Default]
             if len(car) == 0:
                 pass
             elif len(car) == 1:
                 car = car[0]
                 player_car_pairs.append((player, car))
             else:
                 # if there are more than one car, the player was probably demoed
@@ -976,19 +972,18 @@
                 car = car[-1]
                 player_car_pairs.append((player, car))
         return player_car_pairs
 
 
     def get_ball(self):
 
-        # get all actor_ids from objects with object_id 264
         ball_types = [
-            Action.Archetypes_Ball_Ball_Default,
-            Action.Archetypes_GameEvent_GameEvent_Basketball,
-            Action.Archetypes_GameEvent_GameEvent_Hockey,
+            RLObject.Archetypes_Ball_Ball_Default,
+            RLObject.Archetypes_GameEvent_GameEvent_Basketball,
+            RLObject.Archetypes_GameEvent_GameEvent_Hockey,
         ]
         ball = [actor_id for actor_id, actor in self.actors.items() if actor['object_id'] in ball_types]
 
         if len(ball) == 0:
             return None
         elif len(ball) == 1:
             return ball[0]
@@ -1194,19 +1189,21 @@
 
 
 #########
 # STATS #
 #########
 
 
-    def get_stats(self, properties):
+    def get_stats(self):
 
         # prepare stats dict
         stats = {}
 
+        properties = self.properties
+
         # general stuff
         stats['datetime'] = properties['Date']
         stats['team_size'] = properties['TeamSize']
         stats['scores'] = {}
         stats['scores']['Blue'] = 0 if 'Team0Score' not in properties else properties['Team0Score']
         stats['scores']['Orange'] = 0 if 'Team1Score' not in properties else properties['Team1Score']
         stats['replay_name'] = None if 'replay_name' not in properties else properties['ReplayName']
```

### Comparing `rockalyzer-0.0.5/src/constants.py` & `rockalyzer-0.1.0/src/constants.py`

 * *Files identical despite different names*

### Comparing `rockalyzer-0.0.5/src/rockalyzer.egg-info/PKG-INFO` & `rockalyzer-0.1.0/src/rockalyzer.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rockalyzer
-Version: 0.0.5
+Version: 0.1.0
 Summary: Rocket League Boxcars-Replay Analyzer
 Home-page: https://github.com/eliastheis/rockalyzer
 Author: Elias Theis
 Author-email: mail@eliastheis.de
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -52,19 +52,19 @@
 Make sure you parsed the replay to a json file first using one of the tools mentioned above.
 ```python
 from rockalyzer import Replayer
 
 # load replay as JSON file and set render mode
 replayer = Replayer('path/to/replay.json', render=True)
 
-# replay file
-replayer.replay()
+# print header infos
+replayer.print_header_info()
 
-# get stats
-stats = replayer.get_stats()
+# replay file
+stats = replayer.replay()
 ```
 
 ### Simple render
 If you set `render=True` when creating the `Replayer`-object, you get a simple (almost real-time) render of the game using [matplotlib](https://matplotlib.org/)
 ![Screenshot of render](https://raw.githubusercontent.com/eliastheis/rockalyzer/master/render_screenshot.png)
 
 ## Build and upload package to PyPi
```

### Comparing `rockalyzer-0.0.5/src/rockalyzer.py` & `rockalyzer-0.1.0/src/rockalyzer.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,58 +1,73 @@
 from json import load as json_load
-from pprint import pprint
-from time import perf_counter
-from matplotlib import pyplot as plt
-import os
-import gc
+from os.path import isfile as os_isfile
+from gc import collect as gc_collect
 
 from console_colors import *
 from constants import *
 from Game import Game
-from Action import Action
+from RLObject import RLObject
 
 
 class Replayer:
 
     def __init__(self, file_name, render=True):
+        """Create a new Replayer object."""
 
         self.file_name = file_name
         self.render = render
-        #print(HEADER + f'[+] Start Replaying "{self.file_name}"' + ENDC)
 
+        # check if file exists
+        if not os_isfile(self.file_name):
+            raise FileNotFoundError(f'File "{self.file_name}" does not exist')
+        
+        # check if file is json
+        if not self.file_name.lower().endswith('.json'):
+            raise ValueError(f'File "{self.file_name}" is not a json file')
+        
         # load json content
-        with open(self.file_name, mode='r', encoding='utf-8') as f:
-            self.json_content = json_load(f)
+        try:
+            with open(self.file_name, mode='r', encoding='utf-8') as f:
+                self.json_content = json_load(f)
+        except Exception as e:
+            raise ValueError(f'File "{self.file_name}" is not a valid json file') from e
         self.object_lookup = self.json_content['objects']
         self.name_lookup = self.json_content['names']
+        self.__check_json_content()
 
-        # prepare game object
+        # create game object
         self.game = Game(self.json_content, self.render)
 
-        # print simple header
-        #self.print_header_info()
-
         # load actions
-        Action.set_values(self.json_content['objects'])
+        RLObject.set_values(self.json_content['objects'])
 
 
-    def print_header_info(self):
+    def __check_json_content(self):
+        """Check if all keys are present in json file."""
+        keys = ['header_size', 'header_crc', 'major_version', 'minor_version',
+                'net_version', 'game_type', 'properties', 'content_size', 'content_crc',
+                'network_frames', 'levels', 'keyframes', 'tick_marks', 'packages',
+                'objects', 'names', 'class_indices', 'net_cache']
+        for key in keys:
+            if key not in self.json_content:
+                raise ValueError(f'Key "{key}" not found in json file')
+        
 
+    def print_header_info(self):
+        """Print header info of json file."""
         prop = self.json_content['properties']
         replay_name = None if 'ReplayName' not in prop else prop['ReplayName']
         date = prop['Date']
         team_size = prop['TeamSize']
         fps = prop['RecordFPS']
 
-
         # GENERAL STATS
         print(HEADER + f'\n=== {replay_name} ===' + ENDC)
         print(OKGREEN + f' {team_size}v{team_size} on {date} ({len(self.json_content["network_frames"]["frames"])} frames)' + ENDC)
 
-
         # PLAYER STATS
         print(HEADER + '\n=== Players ===' + ENDC)
         team0 = []
         team1 = []
         for player in prop['PlayerStats']:
             name = player['Name']
             b_bot = player['bBot']
@@ -75,15 +90,14 @@
         for player in team1:
             print(f' ORANGE\t\t"{player["name"]}"\t{player["score"]}\t{player["goals"]}\t{player["assists"]}\t{player["saves"]}\t{player["shots"]}')
         print(OKCYAN, end='')
         for player in team0:
             print(f' BLUE\t\t"{player["name"]}"\t{player["score"]}\t{player["goals"]}\t{player["assists"]}\t{player["saves"]}\t{player["shots"]}')
         print(ENDC, end='')
 
-
         # EVENTS
         print(HEADER + '\n=== Events ===' + ENDC)
         for tick_mark in self.json_content['tick_marks']:
 
             frame = tick_mark['frame']
             description = tick_mark['description']
             elapsed_time = self.json_content['network_frames']['frames'][frame]['time']
@@ -94,58 +108,28 @@
                 print(OKRED, end='')
             else:
                 print(OKCYAN, end='')
             print(f' {elapsed_time // 60:02.0f}:{elapsed_time % 60:02.0f} {description}' + ENDC)
 
 
     def replay(self):
-
-        start_time = perf_counter()
-
+        """Replay the game."""
         frames = self.json_content['network_frames']['frames']
         for i, frame in enumerate(frames):
 
             # update game
             self.game.update(i, frame)
 
             # render game
             if self.render:
                 self.game.render()
-
-        diff = perf_counter() - start_time
-        #print(HEADER + f'\n[+] Finished Replaying "{self.file_name}" in {diff:.3f} seconds' + ENDC)
-
-
-    def get_stats(self):
-        return self.game.get_stats(self.json_content['properties'])
+        
+        return self.game.get_stats()
 
 
     def dispose(self):
-        # delete all objects
+        """Dispose the replayer object."""
         del self.game
         del self.json_content
         del self.object_lookup
         del self.name_lookup
-        gc.collect()
-
-
-def file_generator(folder):
-    for entry in os.scandir(folder):
-        if entry.is_file():
-            yield entry.path
-
-
-if __name__ == '__main__':
-
-    # iterate over all files in folder
-    for i, file in enumerate(file_generator('RocketLeagueReplays/json')):
-
-        print(HEADER, i, ENDC)
-        replayer = Replayer(file, render=False)
-        replayer.replay()
-        stats = replayer.get_stats()
-        replayer.dispose()
-
-        # delete all objects
-        del replayer
-        del stats
-        gc.collect()
+        gc_collect()
```

