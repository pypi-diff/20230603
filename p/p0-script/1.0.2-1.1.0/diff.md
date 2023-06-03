# Comparing `tmp/p0-script-1.0.2.zip` & `tmp/p0_script-1.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,1069 +1,918 @@
-Zip file size: 1690078 bytes, number of entries: 1067
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/application/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/domain/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/infra/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/p0_script.egg-info/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/shared/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/tests/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/venv/
--rw-rw-rw-  2.0 fat     1091 b- defN 23-Jun-03 05:39 p0-script-1.0.2/LICENSE.rst
--rw-rw-rw-  2.0 fat     7989 b- defN 23-Jun-03 06:22 p0-script-1.0.2/PKG-INFO
--rw-rw-rw-  2.0 fat     1778 b- defN 23-Jun-03 06:22 p0-script-1.0.2/pyproject.toml
--rw-rw-rw-  2.0 fat     6120 b- defN 23-May-16 19:22 p0-script-1.0.2/README.md
--rw-rw-rw-  2.0 fat       42 b- defN 23-Jun-03 06:22 p0-script-1.0.2/setup.cfg
--rw-rw-rw-  2.0 fat       39 b- defN 23-Jun-03 05:37 p0-script-1.0.2/setup.py
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/application/command/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/application/command_handler/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/application/control_surface/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/application/error/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/application/push2/
--rw-rw-rw-  2.0 fat     4293 b- defN 23-Jun-03 05:51 p0-script-1.0.2/application/CommandBus.py
--rw-rw-rw-  2.0 fat     1400 b- defN 23-Jun-03 05:51 p0-script-1.0.2/application/CommandBusHistory.py
--rw-rw-rw-  2.0 fat    11970 b- defN 23-Jun-03 05:51 p0-script-1.0.2/application/Container.py
--rw-rw-rw-  2.0 fat      186 b- defN 23-Jun-03 05:51 p0-script-1.0.2/application/ContainerInterface.py
--rw-rw-rw-  2.0 fat     2122 b- defN 23-Jun-03 05:51 p0-script-1.0.2/application/main.py
--rw-rw-rw-  2.0 fat     1868 b- defN 23-Jun-03 06:05 p0-script-1.0.2/application/Protocol0.py
--rw-rw-rw-  2.0 fat     1880 b- defN 23-Jun-03 05:51 p0-script-1.0.2/application/Protocol0Midi.py
--rw-rw-rw-  2.0 fat       50 b- defN 22-Oct-29 17:31 p0-script-1.0.2/application/ScriptDisconnectedEvent.py
--rw-rw-rw-  2.0 fat       52 b- defN 22-Oct-29 17:31 p0-script-1.0.2/application/ScriptResetActivatedEvent.py
--rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 17:31 p0-script-1.0.2/application/__init__.py
--rw-rw-rw-  2.0 fat      142 b- defN 23-Jun-03 05:51 p0-script-1.0.2/application/command/BounceTrackToAudioCommand.py
--rw-rw-rw-  2.0 fat      145 b- defN 23-Jun-03 05:51 p0-script-1.0.2/application/command/CheckAudioExportValidCommand.py
--rw-rw-rw-  2.0 fat      141 b- defN 23-Jun-03 05:51 p0-script-1.0.2/application/command/DrumRackToSimplerCommand.py
--rw-rw-rw-  2.0 fat      346 b- defN 23-Jun-03 05:51 p0-script-1.0.2/application/command/EmitBackendEventCommand.py
--rw-rw-rw-  2.0 fat      346 b- defN 23-Jun-03 05:51 p0-script-1.0.2/application/command/FireSceneToPositionCommand.py
--rw-rw-rw-  2.0 fat      141 b- defN 23-Jun-03 05:51 p0-script-1.0.2/application/command/FireSelectedSceneCommand.py
--rw-rw-rw-  2.0 fat      135 b- defN 23-Jun-03 05:51 p0-script-1.0.2/application/command/GetSetStateCommand.py
--rw-rw-rw-  2.0 fat      138 b- defN 23-Jun-03 05:51 p0-script-1.0.2/application/command/GoToGroupTrackCommand.py
--rw-rw-rw-  2.0 fat      278 b- defN 23-Jun-03 05:51 p0-script-1.0.2/application/command/LoadDeviceCommand.py
--rw-rw-rw-  2.0 fat      379 b- defN 23-Jun-03 05:51 p0-script-1.0.2/application/command/LoadDrumRackCommand.py
--rw-rw-rw-  2.0 fat      141 b- defN 23-Jun-03 05:51 p0-script-1.0.2/application/command/LoadMatchingTrackCommand.py
--rw-rw-rw-  2.0 fat      136 b- defN 23-Jun-03 05:51 p0-script-1.0.2/application/command/LoadMinitaurCommand.py
--rw-rw-rw-  2.0 fat      132 b- defN 23-Jun-03 05:51 p0-script-1.0.2/application/command/LoadRev2Command.py
--rw-rw-rw-  2.0 fat      305 b- defN 23-Jun-03 05:51 p0-script-1.0.2/application/command/MidiNoteCommand.py
--rw-rw-rw-  2.0 fat      137 b- defN 23-Jun-03 05:51 p0-script-1.0.2/application/command/PlayPauseSongCommand.py
--rw-rw-rw-  2.0 fat      139 b- defN 23-Jun-03 05:51 p0-script-1.0.2/application/command/RecordUnlimitedCommand.py
--rw-rw-rw-  2.0 fat      136 b- defN 23-Jun-03 05:51 p0-script-1.0.2/application/command/ReloadScriptCommand.py
--rw-rw-rw-  2.0 fat      137 b- defN 23-Jun-03 05:51 p0-script-1.0.2/application/command/ResetPlaybackCommand.py
--rw-rw-rw-  2.0 fat      517 b- defN 23-Jun-03 05:51 p0-script-1.0.2/application/command/ScrollScenePositionCommand.py
--rw-rw-rw-  2.0 fat      283 b- defN 23-Jun-03 05:51 p0-script-1.0.2/application/command/ScrollScenesCommand.py
--rw-rw-rw-  2.0 fat      293 b- defN 23-Jun-03 05:51 p0-script-1.0.2/application/command/ScrollSceneTracksCommand.py
--rw-rw-rw-  2.0 fat      293 b- defN 23-Jun-03 05:51 p0-script-1.0.2/application/command/ScrollTrackVolumeCommand.py
--rw-rw-rw-  2.0 fat      300 b- defN 23-Jun-03 05:51 p0-script-1.0.2/application/command/SelectOrLoadDeviceCommand.py
--rw-rw-rw-  2.0 fat      281 b- defN 23-Jun-03 05:51 p0-script-1.0.2/application/command/SelectTrackCommand.py
--rw-rw-rw-  2.0 fat     1621 b- defN 23-Jun-03 05:51 p0-script-1.0.2/application/command/SerializableCommand.py
--rw-rw-rw-  2.0 fat      287 b- defN 23-Jun-03 05:51 p0-script-1.0.2/application/command/ShowAutomationCommand.py
--rw-rw-rw-  2.0 fat      138 b- defN 23-Jun-03 05:51 p0-script-1.0.2/application/command/ShowInstrumentCommand.py
--rw-rw-rw-  2.0 fat      274 b- defN 23-Jun-03 05:51 p0-script-1.0.2/application/command/ShowMessageCommand.py
--rw-rw-rw-  2.0 fat      133 b- defN 23-Jun-03 05:51 p0-script-1.0.2/application/command/ToggleArmCommand.py
--rw-rw-rw-  2.0 fat      135 b- defN 23-Jun-03 05:51 p0-script-1.0.2/application/command/ToggleNotesCommand.py
--rw-rw-rw-  2.0 fat      144 b- defN 23-Jun-03 05:51 p0-script-1.0.2/application/command/ToggleReferenceTrackCommand.py
--rw-rw-rw-  2.0 fat      139 b- defN 23-Jun-03 05:51 p0-script-1.0.2/application/command/ToggleSceneLoopCommand.py
--rw-rw-rw-  2.0 fat      143 b- defN 23-Jun-03 05:51 p0-script-1.0.2/application/command/UnfoldSelectedSceneCommand.py
--rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 17:31 p0-script-1.0.2/application/command/__init__.py
--rw-rw-rw-  2.0 fat      509 b- defN 23-Jun-03 05:51 p0-script-1.0.2/application/command_handler/BounceTrackToAudioCommandHandler.py
--rw-rw-rw-  2.0 fat      776 b- defN 23-Jun-03 05:51 p0-script-1.0.2/application/command_handler/CheckAudioExportValidCommandHandler.py
--rw-rw-rw-  2.0 fat      423 b- defN 23-Jun-03 05:51 p0-script-1.0.2/application/command_handler/CommandHandlerInterface.py
--rw-rw-rw-  2.0 fat      502 b- defN 23-Jun-03 05:51 p0-script-1.0.2/application/command_handler/DrumRackToSimplerCommandHandler.py
--rw-rw-rw-  2.0 fat      528 b- defN 23-Jun-03 05:51 p0-script-1.0.2/application/command_handler/EmitBackendEventCommandHandler.py
--rw-rw-rw-  2.0 fat     1858 b- defN 23-Jun-03 05:51 p0-script-1.0.2/application/command_handler/FireSceneToPositionCommandHandler.py
--rw-rw-rw-  2.0 fat      506 b- defN 23-Jun-03 05:51 p0-script-1.0.2/application/command_handler/FireSelectedSceneCommandHandler.py
--rw-rw-rw-  2.0 fat      405 b- defN 23-Jun-03 05:51 p0-script-1.0.2/application/command_handler/GetSetStateCommandHandler.py
--rw-rw-rw-  2.0 fat      426 b- defN 23-Jun-03 05:51 p0-script-1.0.2/application/command_handler/GoToGroupTrackCommandHandler.py
--rw-rw-rw-  2.0 fat      489 b- defN 23-Jun-03 05:51 p0-script-1.0.2/application/command_handler/LoadDeviceCommandHandler.py
--rw-rw-rw-  2.0 fat      664 b- defN 23-Jun-03 05:51 p0-script-1.0.2/application/command_handler/LoadDrumRackCommandHandler.py
--rw-rw-rw-  2.0 fat      505 b- defN 23-Jun-03 05:51 p0-script-1.0.2/application/command_handler/LoadMatchingTrackCommandHandler.py
--rw-rw-rw-  2.0 fat      517 b- defN 23-Jun-03 05:51 p0-script-1.0.2/application/command_handler/LoadMinitaurCommandHandler.py
--rw-rw-rw-  2.0 fat      491 b- defN 23-Jun-03 05:51 p0-script-1.0.2/application/command_handler/LoadRev2CommandHandler.py
--rw-rw-rw-  2.0 fat     1581 b- defN 23-Jun-03 05:51 p0-script-1.0.2/application/command_handler/MidiNoteCommandHandler.py
--rw-rw-rw-  2.0 fat      453 b- defN 23-Jun-03 05:51 p0-script-1.0.2/application/command_handler/PlayPauseSongCommandHandler.py
--rw-rw-rw-  2.0 fat      620 b- defN 23-Jun-03 05:51 p0-script-1.0.2/application/command_handler/RecordUnlimitedCommandHandler.py
--rw-rw-rw-  2.0 fat      736 b- defN 23-Jun-03 05:51 p0-script-1.0.2/application/command_handler/ReloadScriptCommandHandler.py
--rw-rw-rw-  2.0 fat      435 b- defN 23-Jun-03 05:51 p0-script-1.0.2/application/command_handler/ResetPlaybackCommandHandler.py
--rw-rw-rw-  2.0 fat      560 b- defN 23-Jun-03 05:51 p0-script-1.0.2/application/command_handler/ScrollScenePositionCommandHandler.py
--rw-rw-rw-  2.0 fat      451 b- defN 23-Jun-03 05:51 p0-script-1.0.2/application/command_handler/ScrollScenesCommandHandler.py
--rw-rw-rw-  2.0 fat      417 b- defN 23-Jun-03 05:51 p0-script-1.0.2/application/command_handler/ScrollSceneTracksCommandHandler.py
--rw-rw-rw-  2.0 fat      427 b- defN 23-Jun-03 05:51 p0-script-1.0.2/application/command_handler/ScrollTrackVolumeCommandHandler.py
--rw-rw-rw-  2.0 fat      574 b- defN 23-Jun-03 05:51 p0-script-1.0.2/application/command_handler/SelectOrLoadDeviceCommandHandler.py
--rw-rw-rw-  2.0 fat      571 b- defN 23-Jun-03 05:51 p0-script-1.0.2/application/command_handler/SelectTrackCommandHandler.py
--rw-rw-rw-  2.0 fat      475 b- defN 23-Jun-03 05:51 p0-script-1.0.2/application/command_handler/ShowAutomationCommandHandler.py
--rw-rw-rw-  2.0 fat      515 b- defN 23-Jun-03 05:51 p0-script-1.0.2/application/command_handler/ShowInstrumentCommandHandler.py
--rw-rw-rw-  2.0 fat      398 b- defN 23-Jun-03 05:51 p0-script-1.0.2/application/command_handler/ShowMessageCommandHandler.py
--rw-rw-rw-  2.0 fat      465 b- defN 23-Jun-03 05:51 p0-script-1.0.2/application/command_handler/ToggleArmCommandJHandler.py
--rw-rw-rw-  2.0 fat      370 b- defN 23-Jun-03 05:51 p0-script-1.0.2/application/command_handler/ToggleNotesCommandHandler.py
--rw-rw-rw-  2.0 fat      402 b- defN 23-Jun-03 05:51 p0-script-1.0.2/application/command_handler/ToggleReferenceTrackCommandHandler.py
--rw-rw-rw-  2.0 fat      457 b- defN 23-Jun-03 05:51 p0-script-1.0.2/application/command_handler/ToggleSceneLoopCommandHandler.py
--rw-rw-rw-  2.0 fat      397 b- defN 23-Jun-03 05:51 p0-script-1.0.2/application/command_handler/UnfoldSelectedSceneCommandHandler.py
--rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 17:31 p0-script-1.0.2/application/command_handler/__init__.py
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/application/control_surface/group/
--rw-rw-rw-  2.0 fat      742 b- defN 23-Jun-03 05:51 p0-script-1.0.2/application/control_surface/ActionGroupFactory.py
--rw-rw-rw-  2.0 fat     2700 b- defN 23-Jun-03 05:51 p0-script-1.0.2/application/control_surface/ActionGroupInterface.py
--rw-rw-rw-  2.0 fat     2923 b- defN 23-Jun-03 05:51 p0-script-1.0.2/application/control_surface/EncoderAction.py
--rw-rw-rw-  2.0 fat      163 b- defN 23-Jun-03 05:51 p0-script-1.0.2/application/control_surface/EncoderMoveEnum.py
--rw-rw-rw-  2.0 fat     5418 b- defN 23-Jun-03 05:51 p0-script-1.0.2/application/control_surface/MultiEncoder.py
--rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 17:31 p0-script-1.0.2/application/control_surface/__init__.py
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/application/control_surface/group/legacy/
--rw-rw-rw-  2.0 fat     1296 b- defN 23-Jun-03 05:51 p0-script-1.0.2/application/control_surface/group/ActionGroupClip.py
--rw-rw-rw-  2.0 fat     1238 b- defN 23-Jun-03 05:51 p0-script-1.0.2/application/control_surface/group/ActionGroupCut.py
--rw-rw-rw-  2.0 fat      852 b- defN 23-Jun-03 05:51 p0-script-1.0.2/application/control_surface/group/ActionGroupFix.py
--rw-rw-rw-  2.0 fat     1200 b- defN 23-Jun-03 05:51 p0-script-1.0.2/application/control_surface/group/ActionGroupLog.py
--rw-rw-rw-  2.0 fat     3890 b- defN 23-Jun-03 05:51 p0-script-1.0.2/application/control_surface/group/ActionGroupMain.py
--rw-rw-rw-  2.0 fat      575 b- defN 23-Jun-03 05:51 p0-script-1.0.2/application/control_surface/group/ActionGroupSample.py
--rw-rw-rw-  2.0 fat      945 b- defN 23-Jun-03 05:51 p0-script-1.0.2/application/control_surface/group/ActionGroupSet.py
--rw-rw-rw-  2.0 fat     2040 b- defN 23-Jun-03 05:51 p0-script-1.0.2/application/control_surface/group/ActionGroupTest.py
--rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 17:31 p0-script-1.0.2/application/control_surface/group/__init__.py
--rw-rw-rw-  2.0 fat     1060 b- defN 23-Jun-03 05:51 p0-script-1.0.2/application/control_surface/group/legacy/ActionGroupPreset.py
--rw-rw-rw-  2.0 fat        0 b- defN 23-May-16 19:22 p0-script-1.0.2/application/control_surface/group/legacy/__init__.py
--rw-rw-rw-  2.0 fat     6026 b- defN 23-Jun-03 05:51 p0-script-1.0.2/application/error/ErrorService.py
--rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 17:31 p0-script-1.0.2/application/error/__init__.py
--rw-rw-rw-  2.0 fat     5848 b- defN 23-Jun-03 05:51 p0-script-1.0.2/application/push2/P0Push2.py
--rw-rw-rw-  2.0 fat     4028 b- defN 23-Jun-03 05:51 p0-script-1.0.2/application/push2/P0SessionRingTrackProvider.py
--rw-rw-rw-  2.0 fat      658 b- defN 23-Jun-03 05:51 p0-script-1.0.2/application/push2/P0ShowInstrumentMode.py
--rw-rw-rw-  2.0 fat      555 b- defN 23-Jun-03 05:51 p0-script-1.0.2/application/push2/P0TrackListComponent.py
--rw-rw-rw-  2.0 fat      476 b- defN 22-Oct-29 17:31 p0-script-1.0.2/application/push2/P0TransportComponent.py
--rw-rw-rw-  2.0 fat       64 b- defN 22-Oct-29 17:31 p0-script-1.0.2/application/push2/__init__.py
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/domain/audit/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/domain/lom/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/domain/shared/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/domain/track_recorder/
--rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 17:31 p0-script-1.0.2/domain/__init__.py
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/domain/audit/stats/
--rw-rw-rw-  2.0 fat     4797 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/audit/AudioLatencyAnalyzerService.py
--rw-rw-rw-  2.0 fat     8527 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/audit/LogService.py
--rw-rw-rw-  2.0 fat     1297 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/audit/LOMAnalyzerService.py
--rw-rw-rw-  2.0 fat     2333 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/audit/SetFixerService.py
--rw-rw-rw-  2.0 fat     3209 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/audit/SetUpgradeService.py
--rw-rw-rw-  2.0 fat      382 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/audit/SongStatsService.py
--rw-rw-rw-  2.0 fat      327 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/audit/utils.py
--rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 17:31 p0-script-1.0.2/domain/audit/__init__.py
--rw-rw-rw-  2.0 fat     1389 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/audit/stats/ClipStats.py
--rw-rw-rw-  2.0 fat     3296 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/audit/stats/DeviceStats.py
--rw-rw-rw-  2.0 fat     2245 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/audit/stats/SampleStats.py
--rw-rw-rw-  2.0 fat      994 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/audit/stats/SceneStats.py
--rw-rw-rw-  2.0 fat      945 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/audit/stats/SongStats.py
--rw-rw-rw-  2.0 fat      180 b- defN 23-May-16 19:22 p0-script-1.0.2/domain/audit/stats/Stats.py
--rw-rw-rw-  2.0 fat      870 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/audit/stats/TrackStats.py
--rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 17:31 p0-script-1.0.2/domain/audit/stats/__init__.py
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/domain/lom/clip/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/domain/lom/clip_slot/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/domain/lom/device/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/domain/lom/device_parameter/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/domain/lom/instrument/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/domain/lom/loop/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/domain/lom/note/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/domain/lom/sample/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/domain/lom/scene/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/domain/lom/set/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/domain/lom/song/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/domain/lom/track/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/domain/lom/validation/
--rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 17:31 p0-script-1.0.2/domain/lom/__init__.py
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/domain/lom/clip/automation/
--rw-rw-rw-  2.0 fat     2351 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/clip/AudioClip.py
--rw-rw-rw-  2.0 fat     7726 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/clip/Clip.py
--rw-rw-rw-  2.0 fat      893 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/clip/ClipAppearance.py
--rw-rw-rw-  2.0 fat      150 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/clip/ClipColorEnum.py
--rw-rw-rw-  2.0 fat      183 b- defN 23-Mar-14 17:41 p0-script-1.0.2/domain/lom/clip/ClipConfig.py
--rw-rw-rw-  2.0 fat      287 b- defN 22-Oct-29 17:31 p0-script-1.0.2/domain/lom/clip/ClipCreatedOrDeletedEvent.py
--rw-rw-rw-  2.0 fat       50 b- defN 22-Oct-29 17:31 p0-script-1.0.2/domain/lom/clip/ClipEnvelopeShowedEvent.py
--rw-rw-rw-  2.0 fat     4139 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/clip/ClipInfo.py
--rw-rw-rw-  2.0 fat     5508 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/clip/ClipLoop.py
--rw-rw-rw-  2.0 fat     4037 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/clip/ClipName.py
--rw-rw-rw-  2.0 fat      900 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/clip/ClipPlayingPosition.py
--rw-rw-rw-  2.0 fat      192 b- defN 22-Oct-29 17:31 p0-script-1.0.2/domain/lom/clip/ClipSlotSelectedEvent.py
--rw-rw-rw-  2.0 fat     2060 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/clip/ClipTail.py
--rw-rw-rw-  2.0 fat     7258 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/clip/MidiClip.py
--rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 17:31 p0-script-1.0.2/domain/lom/clip/__init__.py
--rw-rw-rw-  2.0 fat     3649 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/clip/automation/ClipAutomation.py
--rw-rw-rw-  2.0 fat     1868 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/clip/automation/ClipAutomationEnvelope.py
--rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 17:31 p0-script-1.0.2/domain/lom/clip/automation/__init__.py
--rw-rw-rw-  2.0 fat     2594 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/clip_slot/AudioClipSlot.py
--rw-rw-rw-  2.0 fat     5589 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/clip_slot/ClipSlot.py
--rw-rw-rw-  2.0 fat      736 b- defN 22-Oct-30 14:44 p0-script-1.0.2/domain/lom/clip_slot/ClipSlotAppearance.py
--rw-rw-rw-  2.0 fat      171 b- defN 23-Feb-12 01:17 p0-script-1.0.2/domain/lom/clip_slot/ClipSlotHasClipEvent.py
--rw-rw-rw-  2.0 fat      381 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/clip_slot/MidiClipSlot.py
--rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 17:31 p0-script-1.0.2/domain/lom/clip_slot/__init__.py
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/domain/lom/device/Sample/
--rw-rw-rw-  2.0 fat     4627 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/device/Device.py
--rw-rw-rw-  2.0 fat     1405 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/device/DeviceChain.py
--rw-rw-rw-  2.0 fat     6758 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/device/DeviceDisplayService.py
--rw-rw-rw-  2.0 fat    12653 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/device/DeviceEnum.py
--rw-rw-rw-  2.0 fat      575 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/device/DeviceEnumGroup.py
--rw-rw-rw-  2.0 fat      207 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/device/DeviceLoadedEvent.py
--rw-rw-rw-  2.0 fat     4488 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/device/DeviceService.py
--rw-rw-rw-  2.0 fat     2106 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/device/DrumPad.py
--rw-rw-rw-  2.0 fat     1163 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/device/DrumRackDevice.py
--rw-rw-rw-  2.0 fat       46 b- defN 22-Oct-29 17:31 p0-script-1.0.2/domain/lom/device/DrumRackLoadedEvent.py
--rw-rw-rw-  2.0 fat     1541 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/device/DrumRackSampleService.py
--rw-rw-rw-  2.0 fat     7134 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/device/DrumRackService.py
--rw-rw-rw-  2.0 fat     1383 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/device/MixerDevice.py
--rw-rw-rw-  2.0 fat     1280 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/device/PluginDevice.py
--rw-rw-rw-  2.0 fat     1782 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/device/RackDevice.py
--rw-rw-rw-  2.0 fat     1772 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/device/SimplerDevice.py
--rw-rw-rw-  2.0 fat     5336 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/device/SimpleTrackDevices.py
--rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 17:31 p0-script-1.0.2/domain/lom/device/__init__.py
--rw-rw-rw-  2.0 fat     1409 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/device/Sample/Sample.py
--rw-rw-rw-  2.0 fat      336 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/device/Sample/SampleNotFoundError.py
--rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 17:31 p0-script-1.0.2/domain/lom/device/Sample/__init__.py
--rw-rw-rw-  2.0 fat     4569 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/device_parameter/DeviceParameter.py
--rw-rw-rw-  2.0 fat     4094 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/device_parameter/DeviceParameterEnum.py
--rw-rw-rw-  2.0 fat      895 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/device_parameter/DeviceParameterValue.py
--rw-rw-rw-  2.0 fat     1391 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/device_parameter/LinkedDeviceParameters.py
--rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 17:31 p0-script-1.0.2/domain/lom/device_parameter/__init__.py
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/domain/lom/instrument/instrument/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/domain/lom/instrument/preset/
--rw-rw-rw-  2.0 fat      242 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/instrument/InstrumentActivatedEvent.py
--rw-rw-rw-  2.0 fat      227 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/instrument/InstrumentColorEnum.py
--rw-rw-rw-  2.0 fat     4335 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/instrument/InstrumentDisplayService.py
--rw-rw-rw-  2.0 fat     4153 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/instrument/InstrumentFactory.py
--rw-rw-rw-  2.0 fat     4330 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/instrument/InstrumentInterface.py
--rw-rw-rw-  2.0 fat       50 b- defN 22-Oct-29 17:31 p0-script-1.0.2/domain/lom/instrument/InstrumentSelectedEvent.py
--rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 17:31 p0-script-1.0.2/domain/lom/instrument/__init__.py
--rw-rw-rw-  2.0 fat      564 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/instrument/instrument/InstrumentAddictiveKeys.py
--rw-rw-rw-  2.0 fat      470 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/instrument/instrument/InstrumentDrumRack.py
--rw-rw-rw-  2.0 fat      364 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/instrument/instrument/InstrumentKontakt.py
--rw-rw-rw-  2.0 fat      707 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/instrument/instrument/InstrumentMinitaur.py
--rw-rw-rw-  2.0 fat      352 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/instrument/instrument/InstrumentOpus.py
--rw-rw-rw-  2.0 fat      352 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/instrument/instrument/InstrumentPlay.py
--rw-rw-rw-  2.0 fat     2894 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/instrument/instrument/InstrumentRev2.py
--rw-rw-rw-  2.0 fat      270 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/instrument/instrument/InstrumentSampler.py
--rw-rw-rw-  2.0 fat      475 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/instrument/instrument/InstrumentSerum.py
--rw-rw-rw-  2.0 fat      953 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/instrument/instrument/InstrumentSimpler.py
--rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 17:31 p0-script-1.0.2/domain/lom/instrument/instrument/__init__.py
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/domain/lom/instrument/preset/preset_changer/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/domain/lom/instrument/preset/preset_importer/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/domain/lom/instrument/preset/preset_initializer/
--rw-rw-rw-  2.0 fat      953 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/instrument/preset/InstrumentPreset.py
--rw-rw-rw-  2.0 fat     3149 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/instrument/preset/InstrumentPresetList.py
--rw-rw-rw-  2.0 fat     1877 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/instrument/preset/InstrumentPresetScrollerService.py
--rw-rw-rw-  2.0 fat      161 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/instrument/preset/PresetDisplayOptionEnum.py
--rw-rw-rw-  2.0 fat      155 b- defN 22-Dec-30 12:40 p0-script-1.0.2/domain/lom/instrument/preset/PresetProgramSelectedEvent.py
--rw-rw-rw-  2.0 fat      145 b- defN 22-Oct-29 17:31 p0-script-1.0.2/domain/lom/instrument/preset/SampleSelectedEvent.py
--rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 17:31 p0-script-1.0.2/domain/lom/instrument/preset/__init__.py
--rw-rw-rw-  2.0 fat      772 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/instrument/preset/preset_changer/InstrumentRackPresetChanger.py
--rw-rw-rw-  2.0 fat      478 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/instrument/preset/preset_changer/PresetChangerInterface.py
--rw-rw-rw-  2.0 fat      761 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/instrument/preset/preset_changer/ProgramChangePresetChanger.py
--rw-rw-rw-  2.0 fat      541 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/instrument/preset/preset_changer/SamplePresetChanger.py
--rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 17:31 p0-script-1.0.2/domain/lom/instrument/preset/preset_changer/__init__.py
--rw-rw-rw-  2.0 fat     1962 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/instrument/preset/preset_importer/DirectoryPresetImporter.py
--rw-rw-rw-  2.0 fat      593 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/instrument/preset/preset_importer/FilePresetImporter.py
--rw-rw-rw-  2.0 fat      367 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/instrument/preset/preset_importer/NullPresetImporter.py
--rw-rw-rw-  2.0 fat      669 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/instrument/preset/preset_importer/PluginDevicePresetImporter.py
--rw-rw-rw-  2.0 fat     1754 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/instrument/preset/preset_importer/PresetImporterFactory.py
--rw-rw-rw-  2.0 fat      802 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/instrument/preset/preset_importer/PresetImportInterface.py
--rw-rw-rw-  2.0 fat      656 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/instrument/preset/preset_importer/RackDevicePresetImporter.py
--rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 17:31 p0-script-1.0.2/domain/lom/instrument/preset/preset_importer/__init__.py
--rw-rw-rw-  2.0 fat      597 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/instrument/preset/preset_initializer/PresetInitializerDevicePresetName.py
--rw-rw-rw-  2.0 fat      545 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/instrument/preset/preset_initializer/PresetInitializerGroupTrackName.py
--rw-rw-rw-  2.0 fat      591 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/instrument/preset/preset_initializer/PresetInitializerInterface.py
--rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 17:31 p0-script-1.0.2/domain/lom/instrument/preset/preset_initializer/__init__.py
--rw-rw-rw-  2.0 fat      915 b- defN 22-Oct-29 17:31 p0-script-1.0.2/domain/lom/loop/LoopableInterface.py
--rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 17:31 p0-script-1.0.2/domain/lom/loop/__init__.py
--rw-rw-rw-  2.0 fat     3558 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/note/Note.py
--rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 17:31 p0-script-1.0.2/domain/lom/note/__init__.py
--rw-rw-rw-  2.0 fat     3412 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/sample/SampleCategory.py
--rw-rw-rw-  2.0 fat     1205 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/sample/SampleCategoryEnum.py
--rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 17:31 p0-script-1.0.2/domain/lom/sample/__init__.py
--rw-rw-rw-  2.0 fat     1149 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/scene/LoopingSceneToggler.py
--rw-rw-rw-  2.0 fat      372 b- defN 22-Oct-29 17:31 p0-script-1.0.2/domain/lom/scene/NextSceneStartedEvent.py
--rw-rw-rw-  2.0 fat       51 b- defN 22-Oct-29 17:31 p0-script-1.0.2/domain/lom/scene/PlayingSceneChangedEvent.py
--rw-rw-rw-  2.0 fat     2833 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/scene/PlayingSceneFacade.py
--rw-rw-rw-  2.0 fat     8331 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/scene/Scene.py
--rw-rw-rw-  2.0 fat      867 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/scene/SceneAppearance.py
--rw-rw-rw-  2.0 fat     3382 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/scene/SceneClips.py
--rw-rw-rw-  2.0 fat      715 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/scene/SceneCropScroller.py
--rw-rw-rw-  2.0 fat      202 b- defN 22-Oct-29 17:31 p0-script-1.0.2/domain/lom/scene/SceneFiredEvent.py
--rw-rw-rw-  2.0 fat      263 b- defN 22-Oct-29 17:31 p0-script-1.0.2/domain/lom/scene/SceneLastBarPassedEvent.py
--rw-rw-rw-  2.0 fat     2307 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/scene/SceneLength.py
--rw-rw-rw-  2.0 fat     3470 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/scene/SceneName.py
--rw-rw-rw-  2.0 fat     5613 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/scene/ScenePlaybackService.py
--rw-rw-rw-  2.0 fat     1947 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/scene/ScenePlayingState.py
--rw-rw-rw-  2.0 fat       53 b- defN 22-Oct-29 17:31 p0-script-1.0.2/domain/lom/scene/ScenePositionScrolledEvent.py
--rw-rw-rw-  2.0 fat     1707 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/scene/ScenePositionScroller.py
--rw-rw-rw-  2.0 fat     6000 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/scene/SceneService.py
--rw-rw-rw-  2.0 fat       44 b- defN 22-Oct-29 17:31 p0-script-1.0.2/domain/lom/scene/ScenesMappedEvent.py
--rw-rw-rw-  2.0 fat     3315 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/scene/SceneWindow.py
--rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 17:31 p0-script-1.0.2/domain/lom/scene/__init__.py
--rw-rw-rw-  2.0 fat     4479 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/set/AbletonSet.py
--rw-rw-rw-  2.0 fat      260 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/set/AbletonSetChangedEvent.py
--rw-rw-rw-  2.0 fat      400 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/set/MixingService.py
--rw-rw-rw-  2.0 fat     6017 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/set/SessionToArrangementService.py
--rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 17:31 p0-script-1.0.2/domain/lom/set/__init__.py
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/domain/lom/song/components/
--rw-rw-rw-  2.0 fat       47 b- defN 22-Oct-29 17:31 p0-script-1.0.2/domain/lom/song/SongInitializedEvent.py
--rw-rw-rw-  2.0 fat     1972 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/song/SongInitService.py
--rw-rw-rw-  2.0 fat       43 b- defN 22-Oct-29 17:31 p0-script-1.0.2/domain/lom/song/SongStartedEvent.py
--rw-rw-rw-  2.0 fat       43 b- defN 22-Oct-29 17:31 p0-script-1.0.2/domain/lom/song/SongStoppedEvent.py
--rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 17:31 p0-script-1.0.2/domain/lom/song/__init__.py
--rw-rw-rw-  2.0 fat     2428 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/song/components/ClipComponent.py
--rw-rw-rw-  2.0 fat     2410 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/song/components/DeviceComponent.py
--rw-rw-rw-  2.0 fat     5120 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/song/components/PlaybackComponent.py
--rw-rw-rw-  2.0 fat     1167 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/song/components/QuantizationComponent.py
--rw-rw-rw-  2.0 fat     2880 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/song/components/RecordingComponent.py
--rw-rw-rw-  2.0 fat     2208 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/song/components/SceneComponent.py
--rw-rw-rw-  2.0 fat     2483 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/song/components/SceneCrudComponent.py
--rw-rw-rw-  2.0 fat     1159 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/song/components/TempoComponent.py
--rw-rw-rw-  2.0 fat     4670 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/song/components/TrackComponent.py
--rw-rw-rw-  2.0 fat     1978 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/song/components/TrackCrudComponent.py
--rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 17:31 p0-script-1.0.2/domain/lom/song/components/__init__.py
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/domain/lom/track/abstract_track/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/domain/lom/track/group_track/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/domain/lom/track/routing/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/domain/lom/track/simple_track/
--rw-rw-rw-  2.0 fat      125 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/track/CurrentMonitoringStateEnum.py
--rw-rw-rw-  2.0 fat      205 b- defN 23-May-16 19:22 p0-script-1.0.2/domain/lom/track/P0TrackInterface.py
--rw-rw-rw-  2.0 fat       52 b- defN 22-Oct-29 17:31 p0-script-1.0.2/domain/lom/track/SelectedTrackChangedEvent.py
--rw-rw-rw-  2.0 fat       42 b- defN 22-Oct-29 17:31 p0-script-1.0.2/domain/lom/track/TrackAddedEvent.py
--rw-rw-rw-  2.0 fat     5976 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/track/TrackAutomationService.py
--rw-rw-rw-  2.0 fat      156 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/track/TrackColorEnum.py
--rw-rw-rw-  2.0 fat      276 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/track/TrackDisconnectedEvent.py
--rw-rw-rw-  2.0 fat     4541 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/track/TrackFactory.py
--rw-rw-rw-  2.0 fat     8569 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/track/TrackMapperService.py
--rw-rw-rw-  2.0 fat     1014 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/track/TrackService.py
--rw-rw-rw-  2.0 fat       44 b- defN 22-Oct-29 17:31 p0-script-1.0.2/domain/lom/track/TracksMappedEvent.py
--rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 17:31 p0-script-1.0.2/domain/lom/track/__init__.py
--rw-rw-rw-  2.0 fat     1469 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/track/abstract_track/AbstrackTrackArmState.py
--rw-rw-rw-  2.0 fat     5998 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/track/abstract_track/AbstractTrack.py
--rw-rw-rw-  2.0 fat     2133 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/track/abstract_track/AbstractTrackAppearance.py
--rw-rw-rw-  2.0 fat       56 b- defN 22-Oct-29 17:31 p0-script-1.0.2/domain/lom/track/abstract_track/AbstractTrackNameUpdatedEvent.py
--rw-rw-rw-  2.0 fat      179 b- defN 22-Oct-29 17:31 p0-script-1.0.2/domain/lom/track/abstract_track/AbstractTrackSelectedEvent.py
--rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 17:31 p0-script-1.0.2/domain/lom/track/abstract_track/__init__.py
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/domain/lom/track/group_track/ext_track/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/domain/lom/track/group_track/matching_track/
--rw-rw-rw-  2.0 fat     3757 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/track/group_track/AbstractGroupTrack.py
--rw-rw-rw-  2.0 fat      365 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/track/group_track/DrumsTrack.py
--rw-rw-rw-  2.0 fat      957 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/track/group_track/NormalGroupMatchingTrack.py
--rw-rw-rw-  2.0 fat     1522 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/track/group_track/NormalGroupMatchingTrackCreator.py
--rw-rw-rw-  2.0 fat     3653 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/track/group_track/NormalGroupTrack.py
--rw-rw-rw-  2.0 fat      145 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/track/group_track/VocalsTrack.py
--rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 17:31 p0-script-1.0.2/domain/lom/track/group_track/__init__.py
--rw-rw-rw-  2.0 fat      261 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/track/group_track/ext_track/ExtArmedEvent.py
--rw-rw-rw-  2.0 fat     2214 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/track/group_track/ext_track/ExtArmState.py
--rw-rw-rw-  2.0 fat     4200 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/track/group_track/ext_track/ExternalSynthTrack.py
--rw-rw-rw-  2.0 fat     2519 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/track/group_track/ext_track/ExtMatchingTrack.py
--rw-rw-rw-  2.0 fat     2900 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/track/group_track/ext_track/ExtMatchingTrackCreator.py
--rw-rw-rw-  2.0 fat     1912 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/track/group_track/ext_track/ExtMonitoringState.py
--rw-rw-rw-  2.0 fat     2095 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/track/group_track/ext_track/ExtSoloState.py
--rw-rw-rw-  2.0 fat      642 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/track/group_track/ext_track/SimpleAudioExtTrack.py
--rw-rw-rw-  2.0 fat      807 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/track/group_track/ext_track/SimpleBaseExtTrack.py
--rw-rw-rw-  2.0 fat      729 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/track/group_track/ext_track/SimpleMidiExtTrack.py
--rw-rw-rw-  2.0 fat        0 b- defN 23-Feb-12 01:17 p0-script-1.0.2/domain/lom/track/group_track/ext_track/__init__.py
--rw-rw-rw-  2.0 fat     1962 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/track/group_track/matching_track/MatchingTrackClipColorManager.py
--rw-rw-rw-  2.0 fat     3554 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/track/group_track/matching_track/MatchingTrackClipManager.py
--rw-rw-rw-  2.0 fat      615 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/track/group_track/matching_track/MatchingTrackCreatorInterface.py
--rw-rw-rw-  2.0 fat     1965 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/track/group_track/matching_track/MatchingTrackInterface.py
--rw-rw-rw-  2.0 fat     2230 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/track/group_track/matching_track/MatchingTrackRouter.py
--rw-rw-rw-  2.0 fat     6979 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/track/group_track/matching_track/MatchingTrackService.py
--rw-rw-rw-  2.0 fat      926 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/track/group_track/matching_track/MatchingTrackSoloState.py
--rw-rw-rw-  2.0 fat     2049 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/track/group_track/matching_track/utils.py
--rw-rw-rw-  2.0 fat        0 b- defN 23-Feb-12 01:17 p0-script-1.0.2/domain/lom/track/group_track/matching_track/__init__.py
--rw-rw-rw-  2.0 fat      227 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/track/routing/InputRoutingChannelEnum.py
--rw-rw-rw-  2.0 fat      241 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/track/routing/InputRoutingTypeEnum.py
--rw-rw-rw-  2.0 fat      241 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/track/routing/OutputRoutingTypeEnum.py
--rw-rw-rw-  2.0 fat     1746 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/track/routing/RoutingDisplayNameDescriptor.py
--rw-rw-rw-  2.0 fat     3516 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/track/routing/RoutingTrackDescriptor.py
--rw-rw-rw-  2.0 fat      729 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/track/routing/TrackInputRouting.py
--rw-rw-rw-  2.0 fat      555 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/track/routing/TrackOutputRouting.py
--rw-rw-rw-  2.0 fat      441 b- defN 22-Oct-29 17:31 p0-script-1.0.2/domain/lom/track/routing/TrackRoutingInterface.py
--rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 17:31 p0-script-1.0.2/domain/lom/track/routing/__init__.py
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/domain/lom/track/simple_track/audio/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/domain/lom/track/simple_track/midi/
--rw-rw-rw-  2.0 fat     2882 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/track/simple_track/AudioToMidiClipMapping.py
--rw-rw-rw-  2.0 fat     2562 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/track/simple_track/SimpleMatchingTrack.py
--rw-rw-rw-  2.0 fat     1498 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/track/simple_track/SimpleMatchingTrackCreator.py
--rw-rw-rw-  2.0 fat    15916 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/track/simple_track/SimpleTrack.py
--rw-rw-rw-  2.0 fat      174 b- defN 22-Oct-29 17:31 p0-script-1.0.2/domain/lom/track/simple_track/SimpleTrackArmedEvent.py
--rw-rw-rw-  2.0 fat     1365 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/track/simple_track/SimpleTrackArmState.py
--rw-rw-rw-  2.0 fat     1357 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/track/simple_track/SimpleTrackClipColorManager.py
--rw-rw-rw-  2.0 fat      998 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/track/simple_track/SimpleTrackClips.py
--rw-rw-rw-  2.0 fat     4608 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/track/simple_track/SimpleTrackClipSlots.py
--rw-rw-rw-  2.0 fat      269 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/track/simple_track/SimpleTrackCreatedEvent.py
--rw-rw-rw-  2.0 fat      269 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/track/simple_track/SimpleTrackDeletedEvent.py
--rw-rw-rw-  2.0 fat      237 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/track/simple_track/SimpleTrackFlattenedEvent.py
--rw-rw-rw-  2.0 fat     1179 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/track/simple_track/SimpleTrackMonitoringState.py
--rw-rw-rw-  2.0 fat       54 b- defN 23-Mar-07 00:47 p0-script-1.0.2/domain/lom/track/simple_track/SimpleTrackSaveStartedEvent.py
--rw-rw-rw-  2.0 fat      854 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/track/simple_track/SimpleTrackService.py
--rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 17:31 p0-script-1.0.2/domain/lom/track/simple_track/__init__.py
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/domain/lom/track/simple_track/audio/master/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/domain/lom/track/simple_track/audio/special/
--rw-rw-rw-  2.0 fat     4827 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/track/simple_track/audio/SimpleAudioTrack.py
--rw-rw-rw-  2.0 fat      620 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/track/simple_track/audio/SimpleReturnTrack.py
--rw-rw-rw-  2.0 fat        0 b- defN 23-Feb-12 01:17 p0-script-1.0.2/domain/lom/track/simple_track/audio/__init__.py
--rw-rw-rw-  2.0 fat     1901 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/track/simple_track/audio/master/MasterTrack.py
--rw-rw-rw-  2.0 fat        0 b- defN 23-Feb-12 01:17 p0-script-1.0.2/domain/lom/track/simple_track/audio/master/__init__.py
--rw-rw-rw-  2.0 fat     1223 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/track/simple_track/audio/special/ReferenceTrack.py
--rw-rw-rw-  2.0 fat      387 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/track/simple_track/audio/special/ResamplingTrack.py
--rw-rw-rw-  2.0 fat        0 b- defN 23-Feb-12 01:17 p0-script-1.0.2/domain/lom/track/simple_track/audio/special/__init__.py
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/domain/lom/track/simple_track/midi/special/
--rw-rw-rw-  2.0 fat     1496 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/track/simple_track/midi/SimpleMidiTrack.py
--rw-rw-rw-  2.0 fat        0 b- defN 23-Feb-12 01:17 p0-script-1.0.2/domain/lom/track/simple_track/midi/__init__.py
--rw-rw-rw-  2.0 fat     2627 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/track/simple_track/midi/special/UsamoTrack.py
--rw-rw-rw-  2.0 fat        0 b- defN 23-Feb-12 01:17 p0-script-1.0.2/domain/lom/track/simple_track/midi/special/__init__.py
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/domain/lom/validation/object_validators/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/domain/lom/validation/sub_validators/
--rw-rw-rw-  2.0 fat     2043 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/validation/ValidatorFactory.py
--rw-rw-rw-  2.0 fat      549 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/validation/ValidatorInterface.py
--rw-rw-rw-  2.0 fat     1827 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/validation/ValidatorService.py
--rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 17:31 p0-script-1.0.2/domain/lom/validation/__init__.py
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/domain/lom/validation/object_validators/external_synth_track/
--rw-rw-rw-  2.0 fat      365 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/validation/object_validators/AbstractGroupTrackValidator.py
--rw-rw-rw-  2.0 fat      910 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/validation/object_validators/SceneValidator.py
--rw-rw-rw-  2.0 fat      898 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/validation/object_validators/SimpleAudioTrackValidator.py
--rw-rw-rw-  2.0 fat      393 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/validation/object_validators/SimpleTrackValidator.py
--rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 17:31 p0-script-1.0.2/domain/lom/validation/object_validators/__init__.py
--rw-rw-rw-  2.0 fat     2017 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/validation/object_validators/external_synth_track/ExternalSynthTrackValidator.py
--rw-rw-rw-  2.0 fat     1665 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/validation/object_validators/external_synth_track/SimpleAudioExtTrackValidator.py
--rw-rw-rw-  2.0 fat     2036 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/validation/object_validators/external_synth_track/SimpleMidiExtTrackValidator.py
--rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 17:31 p0-script-1.0.2/domain/lom/validation/object_validators/external_synth_track/__init__.py
--rw-rw-rw-  2.0 fat     1033 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/validation/sub_validators/AggregateValidator.py
--rw-rw-rw-  2.0 fat     1086 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/validation/sub_validators/CallbackValidator.py
--rw-rw-rw-  2.0 fat     1530 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/validation/sub_validators/DeviceParameterValidator.py
--rw-rw-rw-  2.0 fat     1872 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/validation/sub_validators/PropertyValueValidator.py
--rw-rw-rw-  2.0 fat     1305 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/lom/validation/sub_validators/SimpleTrackHasDeviceValidator.py
--rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 17:31 p0-script-1.0.2/domain/lom/validation/sub_validators/__init__.py
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/domain/shared/backend/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/domain/shared/errors/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/domain/shared/event/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/domain/shared/scheduler/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/domain/shared/script/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/domain/shared/ui/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/domain/shared/utils/
--rw-rw-rw-  2.0 fat     3690 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/shared/ApplicationView.py
--rw-rw-rw-  2.0 fat      624 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/shared/BrowserServiceInterface.py
--rw-rw-rw-  2.0 fat      118 b- defN 22-Oct-29 17:31 p0-script-1.0.2/domain/shared/InterfaceClicksServiceInterface.py
--rw-rw-rw-  2.0 fat      570 b- defN 23-May-16 19:22 p0-script-1.0.2/domain/shared/LiveObject.py
--rw-rw-rw-  2.0 fat     1946 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/shared/LiveObjectMapping.py
--rw-rw-rw-  2.0 fat      139 b- defN 22-Oct-29 17:31 p0-script-1.0.2/domain/shared/SessionServiceInterface.py
--rw-rw-rw-  2.0 fat     2207 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/shared/ValueScroller.py
--rw-rw-rw-  2.0 fat      993 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/shared/ValueToggler.py
--rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 17:31 p0-script-1.0.2/domain/shared/__init__.py
--rw-rw-rw-  2.0 fat     1287 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/shared/backend/Backend.py
--rw-rw-rw-  2.0 fat      190 b- defN 23-Mar-07 00:47 p0-script-1.0.2/domain/shared/backend/BackendEvent.py
--rw-rw-rw-  2.0 fat      103 b- defN 22-Oct-29 17:31 p0-script-1.0.2/domain/shared/backend/NotificationColorEnum.py
--rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 17:31 p0-script-1.0.2/domain/shared/backend/__init__.py
--rw-rw-rw-  2.0 fat      178 b- defN 22-Oct-29 17:31 p0-script-1.0.2/domain/shared/errors/ErrorRaisedEvent.py
--rw-rw-rw-  2.0 fat      575 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/shared/errors/error_handler.py
--rw-rw-rw-  2.0 fat       47 b- defN 22-Oct-29 17:31 p0-script-1.0.2/domain/shared/errors/Protocol0Error.py
--rw-rw-rw-  2.0 fat      349 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/shared/errors/Protocol0Warning.py
--rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 17:31 p0-script-1.0.2/domain/shared/errors/__init__.py
--rw-rw-rw-  2.0 fat     4585 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/shared/event/DomainEventBus.py
--rw-rw-rw-  2.0 fat      200 b- defN 23-May-16 19:22 p0-script-1.0.2/domain/shared/event/HasEmitter.py
--rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 17:31 p0-script-1.0.2/domain/shared/event/__init__.py
--rw-rw-rw-  2.0 fat       42 b- defN 22-Oct-29 17:31 p0-script-1.0.2/domain/shared/scheduler/BarChangedEvent.py
--rw-rw-rw-  2.0 fat       41 b- defN 22-Oct-29 17:31 p0-script-1.0.2/domain/shared/scheduler/BarEndingEvent.py
--rw-rw-rw-  2.0 fat      309 b- defN 22-Oct-29 17:31 p0-script-1.0.2/domain/shared/scheduler/BeatSchedulerInterface.py
--rw-rw-rw-  2.0 fat       46 b- defN 22-Oct-29 17:31 p0-script-1.0.2/domain/shared/scheduler/Last16thPassedEvent.py
--rw-rw-rw-  2.0 fat       46 b- defN 22-Oct-29 17:31 p0-script-1.0.2/domain/shared/scheduler/Last32thPassedEvent.py
--rw-rw-rw-  2.0 fat       45 b- defN 22-Oct-29 17:31 p0-script-1.0.2/domain/shared/scheduler/Last8thPassedEvent.py
--rw-rw-rw-  2.0 fat       46 b- defN 22-Oct-29 17:31 p0-script-1.0.2/domain/shared/scheduler/LastBeatPassedEvent.py
--rw-rw-rw-  2.0 fat     2500 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/shared/scheduler/Scheduler.py
--rw-rw-rw-  2.0 fat       47 b- defN 22-Oct-29 17:31 p0-script-1.0.2/domain/shared/scheduler/ThirdBeatPassedEvent.py
--rw-rw-rw-  2.0 fat      130 b- defN 22-Oct-29 17:31 p0-script-1.0.2/domain/shared/scheduler/TickSchedulerEventInterface.py
--rw-rw-rw-  2.0 fat      555 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/shared/scheduler/TickSchedulerInterface.py
--rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 17:31 p0-script-1.0.2/domain/shared/scheduler/__init__.py
--rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 17:31 p0-script-1.0.2/domain/shared/script/__init__.py
--rw-rw-rw-  2.0 fat      118 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/shared/ui/ColorEnum.py
--rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 17:31 p0-script-1.0.2/domain/shared/ui/__init__.py
--rw-rw-rw-  2.0 fat      954 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/shared/utils/concurrency.py
--rw-rw-rw-  2.0 fat      914 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/shared/utils/debug.py
--rw-rw-rw-  2.0 fat     1607 b- defN 22-Oct-29 17:31 p0-script-1.0.2/domain/shared/utils/forward_to.py
--rw-rw-rw-  2.0 fat     3193 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/shared/utils/func.py
--rw-rw-rw-  2.0 fat      260 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/shared/utils/list.py
--rw-rw-rw-  2.0 fat      545 b- defN 23-May-16 19:22 p0-script-1.0.2/domain/shared/utils/string.py
--rw-rw-rw-  2.0 fat     4769 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/shared/utils/timing.py
--rw-rw-rw-  2.0 fat     3475 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/shared/utils/utils.py
--rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 17:31 p0-script-1.0.2/domain/shared/utils/__init__.py
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/domain/track_recorder/config/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/domain/track_recorder/count_in/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/domain/track_recorder/event/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/domain/track_recorder/external_synth/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/domain/track_recorder/recording_bar_length/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/domain/track_recorder/simple/
--rw-rw-rw-  2.0 fat      647 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/track_recorder/AbstractRecorderFactory.py
--rw-rw-rw-  2.0 fat     3192 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/track_recorder/BaseRecorder.py
--rw-rw-rw-  2.0 fat      640 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/track_recorder/RecordProcessorInterface.py
--rw-rw-rw-  2.0 fat     7566 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/track_recorder/RecordService.py
--rw-rw-rw-  2.0 fat      859 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/track_recorder/RecordTypeEnum.py
--rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 17:31 p0-script-1.0.2/domain/track_recorder/__init__.py
--rw-rw-rw-  2.0 fat     1769 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/track_recorder/config/RecordConfig.py
--rw-rw-rw-  2.0 fat     1192 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/track_recorder/config/RecordProcessors.py
--rw-rw-rw-  2.0 fat        0 b- defN 23-Feb-12 01:17 p0-script-1.0.2/domain/track_recorder/config/__init__.py
--rw-rw-rw-  2.0 fat      382 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/track_recorder/count_in/CountInInterface.py
--rw-rw-rw-  2.0 fat     1603 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/track_recorder/count_in/CountInOneBar.py
--rw-rw-rw-  2.0 fat      605 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/track_recorder/count_in/CountInShort.py
--rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 17:31 p0-script-1.0.2/domain/track_recorder/count_in/__init__.py
--rw-rw-rw-  2.0 fat       47 b- defN 23-Feb-12 01:17 p0-script-1.0.2/domain/track_recorder/event/RecordCancelledEvent.py
--rw-rw-rw-  2.0 fat       41 b- defN 23-Feb-12 01:17 p0-script-1.0.2/domain/track_recorder/event/RecordEndedEvent.py
--rw-rw-rw-  2.0 fat      265 b- defN 23-Feb-12 01:17 p0-script-1.0.2/domain/track_recorder/event/RecordStartedEvent.py
--rw-rw-rw-  2.0 fat        0 b- defN 23-Feb-12 01:17 p0-script-1.0.2/domain/track_recorder/event/__init__.py
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/domain/track_recorder/external_synth/record_audio/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/domain/track_recorder/external_synth/record_midi/
--rw-rw-rw-  2.0 fat       47 b- defN 23-Feb-12 01:17 p0-script-1.0.2/domain/track_recorder/external_synth/AudioClipSilentEvent.py
--rw-rw-rw-  2.0 fat      255 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/track_recorder/external_synth/ExtAudioRecordingEndedEvent.py
--rw-rw-rw-  2.0 fat      257 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/track_recorder/external_synth/ExtAudioRecordingStartedEvent.py
--rw-rw-rw-  2.0 fat     2986 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/track_recorder/external_synth/OnRecordEndClipTail.py
--rw-rw-rw-  2.0 fat     4630 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/track_recorder/external_synth/TrackRecorderExternalSynthFactory.py
--rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 17:31 p0-script-1.0.2/domain/track_recorder/external_synth/__init__.py
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/domain/track_recorder/external_synth/record_audio/record_multi/
--rw-rw-rw-  2.0 fat     1868 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/track_recorder/external_synth/record_audio/PostRecordAudio.py
--rw-rw-rw-  2.0 fat      944 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/track_recorder/external_synth/record_audio/PostRecordAudioFull.py
--rw-rw-rw-  2.0 fat      955 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/track_recorder/external_synth/record_audio/PreRecordAudio.py
--rw-rw-rw-  2.0 fat        0 b- defN 23-Feb-12 01:17 p0-script-1.0.2/domain/track_recorder/external_synth/record_audio/__init__.py
--rw-rw-rw-  2.0 fat     2496 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/track_recorder/external_synth/record_audio/record_multi/PreRecordAudioMulti.py
--rw-rw-rw-  2.0 fat     2131 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/track_recorder/external_synth/record_audio/record_multi/RecordAudioMulti.py
--rw-rw-rw-  2.0 fat        0 b- defN 23-Feb-12 01:17 p0-script-1.0.2/domain/track_recorder/external_synth/record_audio/record_multi/__init__.py
--rw-rw-rw-  2.0 fat     1421 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/track_recorder/external_synth/record_midi/PostRecordMidi.py
--rw-rw-rw-  2.0 fat      443 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/track_recorder/external_synth/record_midi/PreRecordMidi.py
--rw-rw-rw-  2.0 fat        0 b- defN 23-Feb-12 01:17 p0-script-1.0.2/domain/track_recorder/external_synth/record_midi/__init__.py
--rw-rw-rw-  2.0 fat      555 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/track_recorder/recording_bar_length/RecordingBarLengthEnum.py
--rw-rw-rw-  2.0 fat      840 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/track_recorder/recording_bar_length/RecordingBarLengthScroller.py
--rw-rw-rw-  2.0 fat       65 b- defN 22-Oct-29 17:31 p0-script-1.0.2/domain/track_recorder/recording_bar_length/SelectedRecordingBarLengthUpdatedEvent.py
--rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 17:31 p0-script-1.0.2/domain/track_recorder/recording_bar_length/__init__.py
--rw-rw-rw-  2.0 fat      663 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/track_recorder/simple/PostRecordSimple.py
--rw-rw-rw-  2.0 fat     2150 b- defN 23-Jun-03 05:51 p0-script-1.0.2/domain/track_recorder/simple/RecorderSimpleFactory.py
--rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 17:31 p0-script-1.0.2/domain/track_recorder/simple/__init__.py
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/infra/interface/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/infra/logging/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/infra/midi/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/infra/persistence/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/infra/scheduler/
--rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 17:31 p0-script-1.0.2/infra/__init__.py
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/infra/interface/session/
--rw-rw-rw-  2.0 fat     5533 b- defN 23-Jun-03 05:51 p0-script-1.0.2/infra/interface/BrowserLoaderService.py
--rw-rw-rw-  2.0 fat     2712 b- defN 23-Jun-03 05:51 p0-script-1.0.2/infra/interface/BrowserService.py
--rw-rw-rw-  2.0 fat      397 b- defN 23-Jun-03 05:51 p0-script-1.0.2/infra/interface/InterfaceClicksService.py
--rw-rw-rw-  2.0 fat      252 b- defN 23-Jun-03 05:51 p0-script-1.0.2/infra/interface/PixelEnum.py
--rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 17:31 p0-script-1.0.2/infra/interface/__init__.py
--rw-rw-rw-  2.0 fat     2678 b- defN 23-Jun-03 05:51 p0-script-1.0.2/infra/interface/session/SessionService.py
--rw-rw-rw-  2.0 fat      226 b- defN 22-Oct-29 17:31 p0-script-1.0.2/infra/interface/session/SessionUpdatedEvent.py
--rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 17:31 p0-script-1.0.2/infra/interface/session/__init__.py
--rw-rw-rw-  2.0 fat     2140 b- defN 23-Jun-03 05:51 p0-script-1.0.2/infra/logging/LoggerService.py
--rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 17:31 p0-script-1.0.2/infra/logging/__init__.py
--rw-rw-rw-  2.0 fat      177 b- defN 22-Oct-29 17:31 p0-script-1.0.2/infra/midi/MidiBytesReceivedEvent.py
--rw-rw-rw-  2.0 fat      173 b- defN 22-Nov-09 01:32 p0-script-1.0.2/infra/midi/MidiBytesSentEvent.py
--rw-rw-rw-  2.0 fat     3146 b- defN 23-Jun-03 05:51 p0-script-1.0.2/infra/midi/MidiService.py
--rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 17:31 p0-script-1.0.2/infra/midi/__init__.py
--rw-rw-rw-  2.0 fat      244 b- defN 23-Jun-03 05:51 p0-script-1.0.2/infra/persistence/SongDataEnum.py
--rw-rw-rw-  2.0 fat     3008 b- defN 23-Jun-03 05:51 p0-script-1.0.2/infra/persistence/SongDataService.py
--rw-rw-rw-  2.0 fat     1189 b- defN 23-Jun-03 05:51 p0-script-1.0.2/infra/persistence/TrackData.py
--rw-rw-rw-  2.0 fat      121 b- defN 23-Jun-03 05:51 p0-script-1.0.2/infra/persistence/TrackDataEnum.py
--rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 17:31 p0-script-1.0.2/infra/persistence/__init__.py
--rw-rw-rw-  2.0 fat     5010 b- defN 23-Jun-03 05:51 p0-script-1.0.2/infra/scheduler/BeatScheduler.py
--rw-rw-rw-  2.0 fat      850 b- defN 23-Jun-03 05:51 p0-script-1.0.2/infra/scheduler/BeatSchedulerEvent.py
--rw-rw-rw-  2.0 fat     3796 b- defN 23-Jun-03 05:51 p0-script-1.0.2/infra/scheduler/BeatTime.py
--rw-rw-rw-  2.0 fat     2928 b- defN 23-Jun-03 05:51 p0-script-1.0.2/infra/scheduler/TickScheduler.py
--rw-rw-rw-  2.0 fat     1011 b- defN 23-Jun-03 05:51 p0-script-1.0.2/infra/scheduler/TickSchedulerEvent.py
--rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 17:31 p0-script-1.0.2/infra/scheduler/__init__.py
--rw-rw-rw-  2.0 fat        1 b- defN 23-Jun-03 06:22 p0-script-1.0.2/p0_script.egg-info/dependency_links.txt
--rw-rw-rw-  2.0 fat     7989 b- defN 23-Jun-03 06:22 p0-script-1.0.2/p0_script.egg-info/PKG-INFO
--rw-rw-rw-  2.0 fat       64 b- defN 23-Jun-03 06:22 p0-script-1.0.2/p0_script.egg-info/requires.txt
--rw-rw-rw-  2.0 fat    45597 b- defN 23-Jun-03 06:22 p0-script-1.0.2/p0_script.egg-info/SOURCES.txt
--rw-rw-rw-  2.0 fat       48 b- defN 23-Jun-03 06:22 p0-script-1.0.2/p0_script.egg-info/top_level.txt
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/shared/logging/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/shared/observer/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/shared/sequence/
--rw-rw-rw-  2.0 fat      803 b- defN 23-Jun-03 05:51 p0-script-1.0.2/shared/AbstractEnum.py
--rw-rw-rw-  2.0 fat      915 b- defN 23-Jun-03 05:51 p0-script-1.0.2/shared/Config.py
--rw-rw-rw-  2.0 fat    13682 b- defN 23-Jun-03 05:51 p0-script-1.0.2/shared/Song.py
--rw-rw-rw-  2.0 fat      127 b- defN 23-Mar-07 00:47 p0-script-1.0.2/shared/types.py
--rw-rw-rw-  2.0 fat      596 b- defN 23-Feb-12 01:17 p0-script-1.0.2/shared/UndoFacade.py
--rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 17:31 p0-script-1.0.2/shared/__init__.py
--rw-rw-rw-  2.0 fat     1877 b- defN 23-Jun-03 05:51 p0-script-1.0.2/shared/logging/Logger.py
--rw-rw-rw-  2.0 fat      261 b- defN 23-Jun-03 05:51 p0-script-1.0.2/shared/logging/LoggerServiceInterface.py
--rw-rw-rw-  2.0 fat      144 b- defN 23-Jun-03 05:51 p0-script-1.0.2/shared/logging/LogLevelEnum.py
--rw-rw-rw-  2.0 fat      714 b- defN 23-Jun-03 05:51 p0-script-1.0.2/shared/logging/StatusBar.py
--rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 17:31 p0-script-1.0.2/shared/logging/__init__.py
--rw-rw-rw-  2.0 fat      692 b- defN 23-Jun-03 05:51 p0-script-1.0.2/shared/observer/Observable.py
--rw-rw-rw-  2.0 fat      249 b- defN 23-Jun-03 05:51 p0-script-1.0.2/shared/observer/Observer.py
--rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 17:31 p0-script-1.0.2/shared/observer/__init__.py
--rw-rw-rw-  2.0 fat      688 b- defN 23-Jun-03 05:51 p0-script-1.0.2/shared/sequence/HasSequenceState.py
--rw-rw-rw-  2.0 fat     2023 b- defN 23-Jun-03 05:51 p0-script-1.0.2/shared/sequence/ParallelSequence.py
--rw-rw-rw-  2.0 fat    11927 b- defN 23-Jun-03 05:51 p0-script-1.0.2/shared/sequence/Sequence.py
--rw-rw-rw-  2.0 fat     1646 b- defN 23-Jun-03 05:51 p0-script-1.0.2/shared/sequence/SequenceState.py
--rw-rw-rw-  2.0 fat     2789 b- defN 23-Jun-03 05:51 p0-script-1.0.2/shared/sequence/SequenceStep.py
--rw-rw-rw-  2.0 fat      851 b- defN 23-Jun-03 05:51 p0-script-1.0.2/shared/sequence/SequenceTransition.py
--rw-rw-rw-  2.0 fat     1761 b- defN 23-Jun-03 05:51 p0-script-1.0.2/shared/sequence/TimeoutLimit.py
--rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 17:31 p0-script-1.0.2/shared/sequence/__init__.py
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/tests/application/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/tests/domain/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/tests/infra/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/tests/shared/
--rw-rw-rw-  2.0 fat      210 b- defN 23-Jun-03 05:51 p0-script-1.0.2/tests/__init__.py
--rw-rw-rw-  2.0 fat     2750 b- defN 23-Jun-03 05:51 p0-script-1.0.2/tests/application/test_multi_encoder.py
--rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 17:31 p0-script-1.0.2/tests/application/__init__.py
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/tests/domain/clip/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/tests/domain/fixtures/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/tests/domain/scene/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/tests/domain/shared/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/tests/domain/track/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/tests/domain/validation/
--rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 17:31 p0-script-1.0.2/tests/domain/__init__.py
--rw-rw-rw-  2.0 fat      803 b- defN 23-Jun-03 05:51 p0-script-1.0.2/tests/domain/clip/test_clip_playing_position.py
--rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 17:31 p0-script-1.0.2/tests/domain/clip/__init__.py
--rw-rw-rw-  2.0 fat     1007 b- defN 23-Jun-03 05:51 p0-script-1.0.2/tests/domain/fixtures/clip.py
--rw-rw-rw-  2.0 fat      437 b- defN 23-Jun-03 05:51 p0-script-1.0.2/tests/domain/fixtures/clip_slot.py
--rw-rw-rw-  2.0 fat       72 b- defN 22-Oct-29 17:31 p0-script-1.0.2/tests/domain/fixtures/clip_view.py
--rw-rw-rw-  2.0 fat      241 b- defN 23-Jun-03 05:51 p0-script-1.0.2/tests/domain/fixtures/container.py
--rw-rw-rw-  2.0 fat      645 b- defN 23-Jun-03 05:51 p0-script-1.0.2/tests/domain/fixtures/device.py
--rw-rw-rw-  2.0 fat      319 b- defN 23-Feb-12 01:17 p0-script-1.0.2/tests/domain/fixtures/device_parameter.py
--rw-rw-rw-  2.0 fat      842 b- defN 23-Jun-03 05:51 p0-script-1.0.2/tests/domain/fixtures/group_track.py
--rw-rw-rw-  2.0 fat     2436 b- defN 23-Jun-03 05:51 p0-script-1.0.2/tests/domain/fixtures/p0.py
--rw-rw-rw-  2.0 fat      264 b- defN 22-Oct-29 17:31 p0-script-1.0.2/tests/domain/fixtures/scene.py
--rw-rw-rw-  2.0 fat     3007 b- defN 23-Jun-03 05:51 p0-script-1.0.2/tests/domain/fixtures/simple_track.py
--rw-rw-rw-  2.0 fat     2701 b- defN 23-Jun-03 05:51 p0-script-1.0.2/tests/domain/fixtures/song.py
--rw-rw-rw-  2.0 fat      308 b- defN 22-Oct-29 17:31 p0-script-1.0.2/tests/domain/fixtures/song_view.py
--rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 17:31 p0-script-1.0.2/tests/domain/fixtures/__init__.py
--rw-rw-rw-  2.0 fat      547 b- defN 23-Jun-03 05:51 p0-script-1.0.2/tests/domain/scene/test_scene_clips.py
--rw-rw-rw-  2.0 fat     1168 b- defN 23-Jun-03 05:51 p0-script-1.0.2/tests/domain/scene/test_scene_length.py
--rw-rw-rw-  2.0 fat     1291 b- defN 23-Jun-03 05:51 p0-script-1.0.2/tests/domain/scene/test_scene_playing_position.py
--rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 17:31 p0-script-1.0.2/tests/domain/scene/__init__.py
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/tests/domain/shared/event/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/tests/domain/shared/utils/
--rw-rw-rw-  2.0 fat      223 b- defN 23-Jun-03 05:51 p0-script-1.0.2/tests/domain/shared/test_decorators.py
--rw-rw-rw-  2.0 fat      933 b- defN 23-Jun-03 05:51 p0-script-1.0.2/tests/domain/shared/test_live_object_mapping.py
--rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 17:31 p0-script-1.0.2/tests/domain/shared/__init__.py
--rw-rw-rw-  2.0 fat     1187 b- defN 23-Jun-03 05:51 p0-script-1.0.2/tests/domain/shared/event/test_domain_event_bus.py
--rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 17:31 p0-script-1.0.2/tests/domain/shared/event/__init__.py
--rw-rw-rw-  2.0 fat      597 b- defN 23-Jun-03 05:51 p0-script-1.0.2/tests/domain/shared/utils/test_func.py
--rw-rw-rw-  2.0 fat     1457 b- defN 23-Jun-03 05:51 p0-script-1.0.2/tests/domain/shared/utils/test_utils.py
--rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 17:31 p0-script-1.0.2/tests/domain/shared/utils/__init__.py
--rw-rw-rw-  2.0 fat      787 b- defN 23-Jun-03 05:51 p0-script-1.0.2/tests/domain/track/test_audio_to_midi_clip_mapping.py
--rw-rw-rw-  2.0 fat      846 b- defN 23-Jun-03 05:51 p0-script-1.0.2/tests/domain/track/test_instantiation.py
--rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 17:31 p0-script-1.0.2/tests/domain/track/__init__.py
--rw-rw-rw-  2.0 fat     1349 b- defN 23-Jun-03 05:51 p0-script-1.0.2/tests/domain/validation/test_aggregate_validator.py
--rw-rw-rw-  2.0 fat     1021 b- defN 23-Jun-03 05:51 p0-script-1.0.2/tests/domain/validation/test_callback_validator.py
--rw-rw-rw-  2.0 fat     1066 b- defN 23-Jun-03 05:51 p0-script-1.0.2/tests/domain/validation/test_property_validator.py
--rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 17:31 p0-script-1.0.2/tests/domain/validation/__init__.py
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/tests/infra/listeners/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/tests/infra/scheduler/
--rw-rw-rw-  2.0 fat     1948 b- defN 23-Jun-03 05:51 p0-script-1.0.2/tests/infra/test_scheduler.py
--rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 17:31 p0-script-1.0.2/tests/infra/__init__.py
--rw-rw-rw-  2.0 fat     1301 b- defN 22-Oct-29 17:31 p0-script-1.0.2/tests/infra/listeners/test_subject_slot.py
--rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 17:31 p0-script-1.0.2/tests/infra/listeners/__init__.py
--rw-rw-rw-  2.0 fat      494 b- defN 23-Jun-03 05:51 p0-script-1.0.2/tests/infra/scheduler/TickSchedulerEventTest.py
--rw-rw-rw-  2.0 fat      735 b- defN 23-Jun-03 05:51 p0-script-1.0.2/tests/infra/scheduler/TickSchedulerTest.py
--rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 17:31 p0-script-1.0.2/tests/infra/scheduler/__init__.py
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/tests/shared/sequence/
--rw-rw-rw-  2.0 fat      555 b- defN 23-Jun-03 05:51 p0-script-1.0.2/tests/shared/test_container.py
--rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 17:31 p0-script-1.0.2/tests/shared/__init__.py
--rw-rw-rw-  2.0 fat     1405 b- defN 23-Jun-03 05:51 p0-script-1.0.2/tests/shared/sequence/test_sanity_sequence.py
--rw-rw-rw-  2.0 fat     3270 b- defN 23-Jun-03 05:51 p0-script-1.0.2/tests/shared/sequence/test_sequence.py
--rw-rw-rw-  2.0 fat     1692 b- defN 23-Jun-03 05:51 p0-script-1.0.2/tests/shared/sequence/test_sequence_parallel.py
--rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 17:31 p0-script-1.0.2/tests/shared/sequence/__init__.py
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/venv/Lib/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/venv/Lib/site-packages/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/venv/Lib/site-packages/pip/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/venv/Lib/site-packages/pkg_resources/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/venv/Lib/site-packages/setuptools/
--rw-rw-rw-  2.0 fat      126 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/easy_install.py
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/
--rw-rw-rw-  2.0 fat       24 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/__init__.py
--rw-rw-rw-  2.0 fat      629 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/__main__.py
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/commands/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/models/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/operations/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/req/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/utils/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/vcs/
--rw-rw-rw-  2.0 fat    14014 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/basecommand.py
--rw-rw-rw-  2.0 fat     8764 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/baseparser.py
--rw-rw-rw-  2.0 fat     2773 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/build_env.py
--rw-rw-rw-  2.0 fat     7023 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/cache.py
--rw-rw-rw-  2.0 fat    16679 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/cmdoptions.py
--rw-rw-rw-  2.0 fat     7912 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/compat.py
--rw-rw-rw-  2.0 fat    13330 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/configuration.py
--rw-rw-rw-  2.0 fat    34257 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/download.py
--rw-rw-rw-  2.0 fat     8470 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/exceptions.py
--rw-rw-rw-  2.0 fat    41718 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/index.py
--rw-rw-rw-  2.0 fat     6504 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/locations.py
--rw-rw-rw-  2.0 fat    11115 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/pep425tags.py
--rw-rw-rw-  2.0 fat    13939 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/resolve.py
--rw-rw-rw-  2.0 fat      164 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/status_codes.py
--rw-rw-rw-  2.0 fat    31967 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/wheel.py
--rw-rw-rw-  2.0 fat     8675 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/__init__.py
--rw-rw-rw-  2.0 fat     1500 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/commands/check.py
--rw-rw-rw-  2.0 fat     3018 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/commands/completion.py
--rw-rw-rw-  2.0 fat     7343 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/commands/configuration.py
--rw-rw-rw-  2.0 fat     9092 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/commands/download.py
--rw-rw-rw-  2.0 fat     3320 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/commands/freeze.py
--rw-rw-rw-  2.0 fat     1729 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/commands/hash.py
--rw-rw-rw-  2.0 fat     1079 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/commands/help.py
--rw-rw-rw-  2.0 fat    20270 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/commands/install.py
--rw-rw-rw-  2.0 fat    11957 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/commands/list.py
--rw-rw-rw-  2.0 fat     4842 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/commands/search.py
--rw-rw-rw-  2.0 fat     6378 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/commands/show.py
--rw-rw-rw-  2.0 fat     2786 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/commands/uninstall.py
--rw-rw-rw-  2.0 fat     6986 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/commands/wheel.py
--rw-rw-rw-  2.0 fat     2297 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/commands/__init__.py
--rw-rw-rw-  2.0 fat      433 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/models/index.py
--rw-rw-rw-  2.0 fat       85 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/models/__init__.py
--rw-rw-rw-  2.0 fat     3776 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/operations/check.py
--rw-rw-rw-  2.0 fat    10277 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/operations/freeze.py
--rw-rw-rw-  2.0 fat    15496 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/operations/prepare.py
--rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/operations/__init__.py
--rw-rw-rw-  2.0 fat    12248 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/req/req_file.py
--rw-rw-rw-  2.0 fat    43930 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/req/req_install.py
--rw-rw-rw-  2.0 fat     7268 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/req/req_set.py
--rw-rw-rw-  2.0 fat    17002 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/req/req_uninstall.py
--rw-rw-rw-  2.0 fat     2152 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/req/__init__.py
--rw-rw-rw-  2.0 fat     9372 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/utils/appdirs.py
--rw-rw-rw-  2.0 fat     2374 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/utils/deprecation.py
--rw-rw-rw-  2.0 fat     1058 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/utils/encoding.py
--rw-rw-rw-  2.0 fat      937 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/utils/filesystem.py
--rw-rw-rw-  2.0 fat     3088 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/utils/glibc.py
--rw-rw-rw-  2.0 fat     2994 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/utils/hashes.py
--rw-rw-rw-  2.0 fat     3586 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/utils/logging.py
--rw-rw-rw-  2.0 fat    28053 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/utils/misc.py
--rw-rw-rw-  2.0 fat     5951 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/utils/outdated.py
--rw-rw-rw-  2.0 fat     2347 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/utils/packaging.py
--rw-rw-rw-  2.0 fat      286 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/utils/setuptools_build.py
--rw-rw-rw-  2.0 fat     2697 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/utils/temp_dir.py
--rw-rw-rw-  2.0 fat     1144 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/utils/typing.py
--rw-rw-rw-  2.0 fat    14058 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/utils/ui.py
--rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/utils/__init__.py
--rw-rw-rw-  2.0 fat     3848 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/vcs/bazaar.py
--rw-rw-rw-  2.0 fat    11743 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/vcs/git.py
--rw-rw-rw-  2.0 fat     3708 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/vcs/mercurial.py
--rw-rw-rw-  2.0 fat     9826 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/vcs/subversion.py
--rw-rw-rw-  2.0 fat    15755 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/vcs/__init__.py
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/certifi/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/colorama/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/distlib/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/idna/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/lockfile/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/msgpack/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/packaging/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/pkg_resources/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/progress/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/pytoml/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/requests/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/webencodings/
--rw-rw-rw-  2.0 fat    25151 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/appdirs.py
--rw-rw-rw-  2.0 fat    40565 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/distro.py
--rw-rw-rw-  2.0 fat    82271 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/ipaddress.py
--rw-rw-rw-  2.0 fat   231068 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/pyparsing.py
--rw-rw-rw-  2.0 fat    10239 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/retrying.py
--rw-rw-rw-  2.0 fat    31779 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/six.py
--rw-rw-rw-  2.0 fat     4841 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/__init__.py
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/
--rw-rw-rw-  2.0 fat     5156 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/adapter.py
--rw-rw-rw-  2.0 fat      829 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/cache.py
--rw-rw-rw-  2.0 fat      724 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/compat.py
--rw-rw-rw-  2.0 fat    14232 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/controller.py
--rw-rw-rw-  2.0 fat     2609 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/filewrapper.py
--rw-rw-rw-  2.0 fat     4282 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/heuristics.py
--rw-rw-rw-  2.0 fat     7249 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/serialize.py
--rw-rw-rw-  2.0 fat      781 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/wrapper.py
--rw-rw-rw-  2.0 fat     1380 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/_cmd.py
--rw-rw-rw-  2.0 fat      313 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/__init__.py
--rw-rw-rw-  2.0 fat     4202 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py
--rw-rw-rw-  2.0 fat     1145 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py
--rw-rw-rw-  2.0 fat       88 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/__init__.py
--rw-rw-rw-  2.0 fat      873 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/certifi/core.py
--rw-rw-rw-  2.0 fat       66 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/certifi/__init__.py
--rw-rw-rw-  2.0 fat       43 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/certifi/__main__.py
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/cli/
--rw-rw-rw-  2.0 fat    31640 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/big5freq.py
--rw-rw-rw-  2.0 fat     1804 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/big5prober.py
--rw-rw-rw-  2.0 fat     9644 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/chardistribution.py
--rw-rw-rw-  2.0 fat     3893 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/charsetgroupprober.py
--rw-rw-rw-  2.0 fat     5255 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/charsetprober.py
--rw-rw-rw-  2.0 fat     3678 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/codingstatemachine.py
--rw-rw-rw-  2.0 fat     1168 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/compat.py
--rw-rw-rw-  2.0 fat     1904 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/cp949prober.py
--rw-rw-rw-  2.0 fat     1737 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/enums.py
--rw-rw-rw-  2.0 fat     4051 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/escprober.py
--rw-rw-rw-  2.0 fat    10756 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/escsm.py
--rw-rw-rw-  2.0 fat     3841 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/eucjpprober.py
--rw-rw-rw-  2.0 fat    13741 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/euckrfreq.py
--rw-rw-rw-  2.0 fat     1795 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/euckrprober.py
--rw-rw-rw-  2.0 fat    32008 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/euctwfreq.py
--rw-rw-rw-  2.0 fat     1793 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/euctwprober.py
--rw-rw-rw-  2.0 fat    20998 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/gb2312freq.py
--rw-rw-rw-  2.0 fat     1800 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/gb2312prober.py
--rw-rw-rw-  2.0 fat    14130 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/hebrewprober.py
--rw-rw-rw-  2.0 fat    26102 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/jisfreq.py
--rw-rw-rw-  2.0 fat    19876 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/jpcntx.py
--rw-rw-rw-  2.0 fat    13067 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/langbulgarianmodel.py
--rw-rw-rw-  2.0 fat    18281 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/langcyrillicmodel.py
--rw-rw-rw-  2.0 fat    12913 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/langgreekmodel.py
--rw-rw-rw-  2.0 fat    11545 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/langhebrewmodel.py
--rw-rw-rw-  2.0 fat    12817 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/langhungarianmodel.py
--rw-rw-rw-  2.0 fat    11489 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/langthaimodel.py
--rw-rw-rw-  2.0 fat    11295 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/langturkishmodel.py
--rw-rw-rw-  2.0 fat     5515 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/latin1prober.py
--rw-rw-rw-  2.0 fat     3504 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/mbcharsetprober.py
--rw-rw-rw-  2.0 fat     2066 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/mbcsgroupprober.py
--rw-rw-rw-  2.0 fat    26053 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/mbcssm.py
--rw-rw-rw-  2.0 fat     5789 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/sbcharsetprober.py
--rw-rw-rw-  2.0 fat     3619 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/sbcsgroupprober.py
--rw-rw-rw-  2.0 fat     3866 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/sjisprober.py
--rw-rw-rw-  2.0 fat    12771 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/universaldetector.py
--rw-rw-rw-  2.0 fat     2848 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/utf8prober.py
--rw-rw-rw-  2.0 fat      251 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/version.py
--rw-rw-rw-  2.0 fat     1598 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/__init__.py
--rw-rw-rw-  2.0 fat     2859 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/cli/chardetect.py
--rw-rw-rw-  2.0 fat        2 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/cli/__init__.py
--rw-rw-rw-  2.0 fat     2626 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/colorama/ansi.py
--rw-rw-rw-  2.0 fat     9904 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/colorama/ansitowin32.py
--rw-rw-rw-  2.0 fat     1999 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/colorama/initialise.py
--rw-rw-rw-  2.0 fat     5582 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/colorama/win32.py
--rw-rw-rw-  2.0 fat     6452 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/colorama/winterm.py
--rw-rw-rw-  2.0 fat      247 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/colorama/__init__.py
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/distlib/_backport/
--rw-rw-rw-  2.0 fat    42524 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/distlib/compat.py
--rw-rw-rw-  2.0 fat    52204 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/distlib/database.py
--rw-rw-rw-  2.0 fat    21589 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/distlib/index.py
--rw-rw-rw-  2.0 fat    52949 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/distlib/locators.py
--rw-rw-rw-  2.0 fat    15204 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/distlib/manifest.py
--rw-rw-rw-  2.0 fat     4518 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/distlib/markers.py
--rw-rw-rw-  2.0 fat    41077 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/distlib/metadata.py
--rw-rw-rw-  2.0 fat    11121 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/distlib/resources.py
--rw-rw-rw-  2.0 fat    17000 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/distlib/scripts.py
--rw-rw-rw-  2.0 fat    61249 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/distlib/util.py
--rw-rw-rw-  2.0 fat    24127 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/distlib/version.py
--rw-rw-rw-  2.0 fat    40490 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/distlib/wheel.py
--rw-rw-rw-  2.0 fat      604 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/distlib/__init__.py
--rw-rw-rw-  2.0 fat     1012 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/distlib/_backport/misc.py
--rw-rw-rw-  2.0 fat    26408 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/distlib/_backport/shutil.py
--rw-rw-rw-  2.0 fat    27752 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/distlib/_backport/sysconfig.py
--rw-rw-rw-  2.0 fat    95235 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/distlib/_backport/tarfile.py
--rw-rw-rw-  2.0 fat      280 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/distlib/_backport/__init__.py
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/filters/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/treeadapters/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/treebuilders/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/treewalkers/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/_trie/
--rw-rw-rw-  2.0 fat    86465 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/constants.py
--rw-rw-rw-  2.0 fat   121754 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/html5parser.py
--rw-rw-rw-  2.0 fat    16167 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/serializer.py
--rw-rw-rw-  2.0 fat    16993 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/_ihatexml.py
--rw-rw-rw-  2.0 fat    33475 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/_inputstream.py
--rw-rw-rw-  2.0 fat    78301 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/_tokenizer.py
--rw-rw-rw-  2.0 fat     4139 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/_utils.py
--rw-rw-rw-  2.0 fat     1197 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/__init__.py
--rw-rw-rw-  2.0 fat      948 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/filters/alphabeticalattributes.py
--rw-rw-rw-  2.0 fat      298 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/filters/base.py
--rw-rw-rw-  2.0 fat     3018 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/filters/inject_meta_charset.py
--rw-rw-rw-  2.0 fat     3736 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/filters/lint.py
--rw-rw-rw-  2.0 fat    10795 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/filters/optionaltags.py
--rw-rw-rw-  2.0 fat    27144 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/filters/sanitizer.py
--rw-rw-rw-  2.0 fat     1252 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/filters/whitespace.py
--rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/filters/__init__.py
--rw-rw-rw-  2.0 fat     1769 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/treeadapters/genshi.py
--rw-rw-rw-  2.0 fat     1826 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/treeadapters/sax.py
--rw-rw-rw-  2.0 fat      709 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/treeadapters/__init__.py
--rw-rw-rw-  2.0 fat    14996 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/treebuilders/base.py
--rw-rw-rw-  2.0 fat     9071 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/treebuilders/dom.py
--rw-rw-rw-  2.0 fat    13104 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/treebuilders/etree.py
--rw-rw-rw-  2.0 fat    14488 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/treebuilders/etree_lxml.py
--rw-rw-rw-  2.0 fat     3680 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/treebuilders/__init__.py
--rw-rw-rw-  2.0 fat     7728 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/treewalkers/base.py
--rw-rw-rw-  2.0 fat     1456 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/treewalkers/dom.py
--rw-rw-rw-  2.0 fat     4680 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/treewalkers/etree.py
--rw-rw-rw-  2.0 fat     6522 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/treewalkers/etree_lxml.py
--rw-rw-rw-  2.0 fat     2378 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/treewalkers/genshi.py
--rw-rw-rw-  2.0 fat     5868 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/treewalkers/__init__.py
--rw-rw-rw-  2.0 fat     1222 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/_trie/datrie.py
--rw-rw-rw-  2.0 fat     1842 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/_trie/py.py
--rw-rw-rw-  2.0 fat      967 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/_trie/_base.py
--rw-rw-rw-  2.0 fat      303 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/_trie/__init__.py
--rw-rw-rw-  2.0 fat     3417 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/idna/codec.py
--rw-rw-rw-  2.0 fat      244 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/idna/compat.py
--rw-rw-rw-  2.0 fat    11777 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/idna/core.py
--rw-rw-rw-  2.0 fat    34584 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/idna/idnadata.py
--rw-rw-rw-  2.0 fat     1802 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/idna/intranges.py
--rw-rw-rw-  2.0 fat       23 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/idna/package_data.py
--rw-rw-rw-  2.0 fat   192578 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/idna/uts46data.py
--rw-rw-rw-  2.0 fat       60 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/idna/__init__.py
--rw-rw-rw-  2.0 fat     2725 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/lockfile/linklockfile.py
--rw-rw-rw-  2.0 fat     3180 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/lockfile/mkdirlockfile.py
--rw-rw-rw-  2.0 fat     6280 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/lockfile/pidlockfile.py
--rw-rw-rw-  2.0 fat     5662 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/lockfile/sqlitelockfile.py
--rw-rw-rw-  2.0 fat     2686 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/lockfile/symlinklockfile.py
--rw-rw-rw-  2.0 fat     9718 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/lockfile/__init__.py
--rw-rw-rw-  2.0 fat     1097 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/msgpack/exceptions.py
--rw-rw-rw-  2.0 fat    37388 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/msgpack/fallback.py
--rw-rw-rw-  2.0 fat       21 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/msgpack/_version.py
--rw-rw-rw-  2.0 fat     1743 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/msgpack/__init__.py
--rw-rw-rw-  2.0 fat     8522 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/packaging/markers.py
--rw-rw-rw-  2.0 fat     4571 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/packaging/requirements.py
--rw-rw-rw-  2.0 fat    28800 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/packaging/specifiers.py
--rw-rw-rw-  2.0 fat     1643 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/packaging/utils.py
--rw-rw-rw-  2.0 fat    12660 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/packaging/version.py
--rw-rw-rw-  2.0 fat      890 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/packaging/_compat.py
--rw-rw-rw-  2.0 fat     1488 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/packaging/_structures.py
--rw-rw-rw-  2.0 fat      741 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/packaging/__about__.py
--rw-rw-rw-  2.0 fat      527 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/packaging/__init__.py
--rw-rw-rw-  2.0 fat      622 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/pkg_resources/py31compat.py
--rw-rw-rw-  2.0 fat   106604 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/pkg_resources/__init__.py
--rw-rw-rw-  2.0 fat     2924 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/progress/bar.py
--rw-rw-rw-  2.0 fat     1576 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/progress/counter.py
--rw-rw-rw-  2.0 fat     2945 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/progress/helpers.py
--rw-rw-rw-  2.0 fat     1483 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/progress/spinner.py
--rw-rw-rw-  2.0 fat     3315 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/progress/__init__.py
--rw-rw-rw-  2.0 fat      522 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/pytoml/core.py
--rw-rw-rw-  2.0 fat    10916 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/pytoml/parser.py
--rw-rw-rw-  2.0 fat     3942 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/pytoml/writer.py
--rw-rw-rw-  2.0 fat       95 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/pytoml/__init__.py
--rw-rw-rw-  2.0 fat    21541 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/requests/adapters.py
--rw-rw-rw-  2.0 fat     6389 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/requests/api.py
--rw-rw-rw-  2.0 fat    10021 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/requests/auth.py
--rw-rw-rw-  2.0 fat      483 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/requests/certs.py
--rw-rw-rw-  2.0 fat     1943 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/requests/compat.py
--rw-rw-rw-  2.0 fat    18750 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/requests/cookies.py
--rw-rw-rw-  2.0 fat     3237 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/requests/exceptions.py
--rw-rw-rw-  2.0 fat     3787 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/requests/help.py
--rw-rw-rw-  2.0 fat      801 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/requests/hooks.py
--rw-rw-rw-  2.0 fat    35016 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/requests/models.py
--rw-rw-rw-  2.0 fat      711 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/requests/packages.py
--rw-rw-rw-  2.0 fat    28283 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/requests/sessions.py
--rw-rw-rw-  2.0 fat     3414 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/requests/status_codes.py
--rw-rw-rw-  2.0 fat     3117 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/requests/structures.py
--rw-rw-rw-  2.0 fat    28556 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/requests/utils.py
--rw-rw-rw-  2.0 fat     1138 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/requests/_internal_utils.py
--rw-rw-rw-  2.0 fat     3765 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/requests/__init__.py
--rw-rw-rw-  2.0 fat      450 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/requests/__version__.py
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/packages/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/
--rw-rw-rw-  2.0 fat    13376 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/connection.py
--rw-rw-rw-  2.0 fat    36263 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/connectionpool.py
--rw-rw-rw-  2.0 fat     6849 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/exceptions.py
--rw-rw-rw-  2.0 fat     6121 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/fields.py
--rw-rw-rw-  2.0 fat     2415 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/filepost.py
--rw-rw-rw-  2.0 fat    16785 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/poolmanager.py
--rw-rw-rw-  2.0 fat     6094 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/request.py
--rw-rw-rw-  2.0 fat    23529 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/response.py
--rw-rw-rw-  2.0 fat    10523 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/_collections.py
--rw-rw-rw-  2.0 fat     2950 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/__init__.py
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/
--rw-rw-rw-  2.0 fat    11185 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/appengine.py
--rw-rw-rw-  2.0 fat     4590 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py
--rw-rw-rw-  2.0 fat    15826 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py
--rw-rw-rw-  2.0 fat    31311 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/securetransport.py
--rw-rw-rw-  2.0 fat     6383 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/socks.py
--rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/__init__.py
--rw-rw-rw-  2.0 fat    18153 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
--rw-rw-rw-  2.0 fat    12405 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
--rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/packages/ssl_match_hostname/
--rw-rw-rw-  2.0 fat     9194 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/packages/ordered_dict.py
--rw-rw-rw-  2.0 fat    30966 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/packages/six.py
--rw-rw-rw-  2.0 fat      114 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/packages/__init__.py
--rw-rw-rw-  2.0 fat     1514 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py
--rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/__init__.py
--rw-rw-rw-  2.0 fat     5876 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/packages/ssl_match_hostname/_implementation.py
--rw-rw-rw-  2.0 fat      707 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/packages/ssl_match_hostname/__init__.py
--rw-rw-rw-  2.0 fat     4367 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/connection.py
--rw-rw-rw-  2.0 fat     3823 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/request.py
--rw-rw-rw-  2.0 fat     2424 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/response.py
--rw-rw-rw-  2.0 fat    15002 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/retry.py
--rw-rw-rw-  2.0 fat    21728 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/selectors.py
--rw-rw-rw-  2.0 fat    12561 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/ssl_.py
--rw-rw-rw-  2.0 fat     9999 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/timeout.py
--rw-rw-rw-  2.0 fat     6717 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/url.py
--rw-rw-rw-  2.0 fat     1491 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/wait.py
--rw-rw-rw-  2.0 fat     1098 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/__init__.py
--rw-rw-rw-  2.0 fat     9210 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/webencodings/labels.py
--rw-rw-rw-  2.0 fat     1364 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/webencodings/mklabels.py
--rw-rw-rw-  2.0 fat     6716 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/webencodings/tests.py
--rw-rw-rw-  2.0 fat     4632 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/webencodings/x_user_defined.py
--rw-rw-rw-  2.0 fat    10921 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/webencodings/__init__.py
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/venv/Lib/site-packages/pkg_resources/extern/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/venv/Lib/site-packages/pkg_resources/_vendor/
--rw-rw-rw-  2.0 fat      600 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pkg_resources/py31compat.py
--rw-rw-rw-  2.0 fat   103551 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pkg_resources/__init__.py
--rw-rw-rw-  2.0 fat     2487 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pkg_resources/extern/__init__.py
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/venv/Lib/site-packages/pkg_resources/_vendor/packaging/
--rw-rw-rw-  2.0 fat    22374 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pkg_resources/_vendor/appdirs.py
--rw-rw-rw-  2.0 fat   229867 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing.py
--rw-rw-rw-  2.0 fat    30098 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pkg_resources/_vendor/six.py
--rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pkg_resources/_vendor/__init__.py
--rw-rw-rw-  2.0 fat     8248 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pkg_resources/_vendor/packaging/markers.py
--rw-rw-rw-  2.0 fat     4355 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pkg_resources/_vendor/packaging/requirements.py
--rw-rw-rw-  2.0 fat    28025 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pkg_resources/_vendor/packaging/specifiers.py
--rw-rw-rw-  2.0 fat      421 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pkg_resources/_vendor/packaging/utils.py
--rw-rw-rw-  2.0 fat    11556 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pkg_resources/_vendor/packaging/version.py
--rw-rw-rw-  2.0 fat      860 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_compat.py
--rw-rw-rw-  2.0 fat     1416 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_structures.py
--rw-rw-rw-  2.0 fat      720 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pkg_resources/_vendor/packaging/__about__.py
--rw-rw-rw-  2.0 fat      513 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/pkg_resources/_vendor/packaging/__init__.py
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/venv/Lib/site-packages/setuptools/command/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/venv/Lib/site-packages/setuptools/extern/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/venv/Lib/site-packages/setuptools/_vendor/
--rw-rw-rw-  2.0 fat     6592 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/setuptools/archive_util.py
--rw-rw-rw-  2.0 fat     5671 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/setuptools/build_meta.py
--rw-rw-rw-  2.0 fat    16381 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/setuptools/config.py
--rw-rw-rw-  2.0 fat     5837 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/setuptools/depends.py
--rw-rw-rw-  2.0 fat      935 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/setuptools/dep_util.py
--rw-rw-rw-  2.0 fat    42514 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/setuptools/dist.py
--rw-rw-rw-  2.0 fat     1729 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/setuptools/extension.py
--rw-rw-rw-  2.0 fat     3146 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/setuptools/glibc.py
--rw-rw-rw-  2.0 fat     5207 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/setuptools/glob.py
--rw-rw-rw-  2.0 fat      787 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/setuptools/launch.py
--rw-rw-rw-  2.0 fat     2013 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/setuptools/lib2to3_ex.py
--rw-rw-rw-  2.0 fat     5789 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/setuptools/monkey.py
--rw-rw-rw-  2.0 fat    40877 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/setuptools/msvc.py
--rw-rw-rw-  2.0 fat     3199 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/setuptools/namespaces.py
--rw-rw-rw-  2.0 fat    40142 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/setuptools/package_index.py
--rw-rw-rw-  2.0 fat    10882 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/setuptools/pep425tags.py
--rw-rw-rw-  2.0 fat      536 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/setuptools/py27compat.py
--rw-rw-rw-  2.0 fat     1192 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/setuptools/py31compat.py
--rw-rw-rw-  2.0 fat     1182 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/setuptools/py33compat.py
--rw-rw-rw-  2.0 fat     2891 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/setuptools/py36compat.py
--rw-rw-rw-  2.0 fat    14276 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/setuptools/sandbox.py
--rw-rw-rw-  2.0 fat     2307 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/setuptools/site-patch.py
--rw-rw-rw-  2.0 fat     8492 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/setuptools/ssl_support.py
--rw-rw-rw-  2.0 fat      996 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/setuptools/unicode_utils.py
--rw-rw-rw-  2.0 fat      144 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/setuptools/version.py
--rw-rw-rw-  2.0 fat     7230 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/setuptools/wheel.py
--rw-rw-rw-  2.0 fat      714 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/setuptools/windows_support.py
--rw-rw-rw-  2.0 fat     5700 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/setuptools/__init__.py
--rw-rw-rw-  2.0 fat     2426 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/setuptools/command/alias.py
--rw-rw-rw-  2.0 fat    18185 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/setuptools/command/bdist_egg.py
--rw-rw-rw-  2.0 fat     1508 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/setuptools/command/bdist_rpm.py
--rw-rw-rw-  2.0 fat      637 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/setuptools/command/bdist_wininst.py
--rw-rw-rw-  2.0 fat     4484 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/setuptools/command/build_clib.py
--rw-rw-rw-  2.0 fat    13173 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/setuptools/command/build_ext.py
--rw-rw-rw-  2.0 fat     9596 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/setuptools/command/build_py.py
--rw-rw-rw-  2.0 fat     8046 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/setuptools/command/develop.py
--rw-rw-rw-  2.0 fat      960 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/setuptools/command/dist_info.py
--rw-rw-rw-  2.0 fat    87054 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/setuptools/command/easy_install.py
--rw-rw-rw-  2.0 fat    24800 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/setuptools/command/egg_info.py
--rw-rw-rw-  2.0 fat     4683 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/setuptools/command/install.py
--rw-rw-rw-  2.0 fat     2203 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/setuptools/command/install_egg_info.py
--rw-rw-rw-  2.0 fat     3840 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/setuptools/command/install_lib.py
--rw-rw-rw-  2.0 fat     2439 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/setuptools/command/install_scripts.py
--rw-rw-rw-  2.0 fat     4986 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/setuptools/command/py36compat.py
--rw-rw-rw-  2.0 fat      270 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/setuptools/command/register.py
--rw-rw-rw-  2.0 fat     2164 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/setuptools/command/rotate.py
--rw-rw-rw-  2.0 fat      658 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/setuptools/command/saveopts.py
--rw-rw-rw-  2.0 fat     6711 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/setuptools/command/sdist.py
--rw-rw-rw-  2.0 fat     5085 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/setuptools/command/setopt.py
--rw-rw-rw-  2.0 fat     9214 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/setuptools/command/test.py
--rw-rw-rw-  2.0 fat     1172 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/setuptools/command/upload.py
--rw-rw-rw-  2.0 fat     7311 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/setuptools/command/upload_docs.py
--rw-rw-rw-  2.0 fat      594 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/setuptools/command/__init__.py
--rw-rw-rw-  2.0 fat     2499 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/setuptools/extern/__init__.py
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-03 06:22 p0-script-1.0.2/venv/Lib/site-packages/setuptools/_vendor/packaging/
--rw-rw-rw-  2.0 fat   229867 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/setuptools/_vendor/pyparsing.py
--rw-rw-rw-  2.0 fat    30098 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/setuptools/_vendor/six.py
--rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/setuptools/_vendor/__init__.py
--rw-rw-rw-  2.0 fat     8239 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/setuptools/_vendor/packaging/markers.py
--rw-rw-rw-  2.0 fat     4343 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/setuptools/_vendor/packaging/requirements.py
--rw-rw-rw-  2.0 fat    28025 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/setuptools/_vendor/packaging/specifiers.py
--rw-rw-rw-  2.0 fat      421 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/setuptools/_vendor/packaging/utils.py
--rw-rw-rw-  2.0 fat    11556 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/setuptools/_vendor/packaging/version.py
--rw-rw-rw-  2.0 fat      860 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/setuptools/_vendor/packaging/_compat.py
--rw-rw-rw-  2.0 fat     1416 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/setuptools/_vendor/packaging/_structures.py
--rw-rw-rw-  2.0 fat      720 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/setuptools/_vendor/packaging/__about__.py
--rw-rw-rw-  2.0 fat      513 b- defN 23-Jun-03 05:42 p0-script-1.0.2/venv/Lib/site-packages/setuptools/_vendor/packaging/__init__.py
-1067 files, 5533173 bytes uncompressed, 1476222 bytes compressed:  73.3%
+Zip file size: 1660134 bytes, number of entries: 916
+-rw-rw-rw-  2.0 fat     4293 b- defN 23-Jun-03 03:51 application/CommandBus.py
+-rw-rw-rw-  2.0 fat     1400 b- defN 23-Jun-03 03:51 application/CommandBusHistory.py
+-rw-rw-rw-  2.0 fat    11970 b- defN 23-Jun-03 03:51 application/Container.py
+-rw-rw-rw-  2.0 fat      186 b- defN 23-Jun-03 03:51 application/ContainerInterface.py
+-rw-rw-rw-  2.0 fat     1868 b- defN 23-Jun-03 04:05 application/Protocol0.py
+-rw-rw-rw-  2.0 fat     1880 b- defN 23-Jun-03 03:51 application/Protocol0Midi.py
+-rw-rw-rw-  2.0 fat       50 b- defN 22-Oct-29 15:31 application/ScriptDisconnectedEvent.py
+-rw-rw-rw-  2.0 fat       52 b- defN 22-Oct-29 15:31 application/ScriptResetActivatedEvent.py
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 15:31 application/__init__.py
+-rw-rw-rw-  2.0 fat     2122 b- defN 23-Jun-03 03:51 application/main.py
+-rw-rw-rw-  2.0 fat      142 b- defN 23-Jun-03 03:51 application/command/BounceTrackToAudioCommand.py
+-rw-rw-rw-  2.0 fat      145 b- defN 23-Jun-03 03:51 application/command/CheckAudioExportValidCommand.py
+-rw-rw-rw-  2.0 fat      141 b- defN 23-Jun-03 03:51 application/command/DrumRackToSimplerCommand.py
+-rw-rw-rw-  2.0 fat      346 b- defN 23-Jun-03 03:51 application/command/EmitBackendEventCommand.py
+-rw-rw-rw-  2.0 fat      346 b- defN 23-Jun-03 03:51 application/command/FireSceneToPositionCommand.py
+-rw-rw-rw-  2.0 fat      141 b- defN 23-Jun-03 03:51 application/command/FireSelectedSceneCommand.py
+-rw-rw-rw-  2.0 fat      135 b- defN 23-Jun-03 03:51 application/command/GetSetStateCommand.py
+-rw-rw-rw-  2.0 fat      138 b- defN 23-Jun-03 03:51 application/command/GoToGroupTrackCommand.py
+-rw-rw-rw-  2.0 fat      278 b- defN 23-Jun-03 03:51 application/command/LoadDeviceCommand.py
+-rw-rw-rw-  2.0 fat      379 b- defN 23-Jun-03 03:51 application/command/LoadDrumRackCommand.py
+-rw-rw-rw-  2.0 fat      141 b- defN 23-Jun-03 03:51 application/command/LoadMatchingTrackCommand.py
+-rw-rw-rw-  2.0 fat      136 b- defN 23-Jun-03 03:51 application/command/LoadMinitaurCommand.py
+-rw-rw-rw-  2.0 fat      132 b- defN 23-Jun-03 03:51 application/command/LoadRev2Command.py
+-rw-rw-rw-  2.0 fat      305 b- defN 23-Jun-03 03:51 application/command/MidiNoteCommand.py
+-rw-rw-rw-  2.0 fat      137 b- defN 23-Jun-03 03:51 application/command/PlayPauseSongCommand.py
+-rw-rw-rw-  2.0 fat      139 b- defN 23-Jun-03 03:51 application/command/RecordUnlimitedCommand.py
+-rw-rw-rw-  2.0 fat      136 b- defN 23-Jun-03 03:51 application/command/ReloadScriptCommand.py
+-rw-rw-rw-  2.0 fat      137 b- defN 23-Jun-03 03:51 application/command/ResetPlaybackCommand.py
+-rw-rw-rw-  2.0 fat      517 b- defN 23-Jun-03 03:51 application/command/ScrollScenePositionCommand.py
+-rw-rw-rw-  2.0 fat      293 b- defN 23-Jun-03 03:51 application/command/ScrollSceneTracksCommand.py
+-rw-rw-rw-  2.0 fat      283 b- defN 23-Jun-03 03:51 application/command/ScrollScenesCommand.py
+-rw-rw-rw-  2.0 fat      293 b- defN 23-Jun-03 03:51 application/command/ScrollTrackVolumeCommand.py
+-rw-rw-rw-  2.0 fat      300 b- defN 23-Jun-03 03:51 application/command/SelectOrLoadDeviceCommand.py
+-rw-rw-rw-  2.0 fat      281 b- defN 23-Jun-03 03:51 application/command/SelectTrackCommand.py
+-rw-rw-rw-  2.0 fat     1621 b- defN 23-Jun-03 03:51 application/command/SerializableCommand.py
+-rw-rw-rw-  2.0 fat      287 b- defN 23-Jun-03 03:51 application/command/ShowAutomationCommand.py
+-rw-rw-rw-  2.0 fat      138 b- defN 23-Jun-03 03:51 application/command/ShowInstrumentCommand.py
+-rw-rw-rw-  2.0 fat      274 b- defN 23-Jun-03 03:51 application/command/ShowMessageCommand.py
+-rw-rw-rw-  2.0 fat      133 b- defN 23-Jun-03 03:51 application/command/ToggleArmCommand.py
+-rw-rw-rw-  2.0 fat      135 b- defN 23-Jun-03 03:51 application/command/ToggleNotesCommand.py
+-rw-rw-rw-  2.0 fat      144 b- defN 23-Jun-03 03:51 application/command/ToggleReferenceTrackCommand.py
+-rw-rw-rw-  2.0 fat      139 b- defN 23-Jun-03 03:51 application/command/ToggleSceneLoopCommand.py
+-rw-rw-rw-  2.0 fat      143 b- defN 23-Jun-03 03:51 application/command/UnfoldSelectedSceneCommand.py
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 15:31 application/command/__init__.py
+-rw-rw-rw-  2.0 fat      509 b- defN 23-Jun-03 03:51 application/command_handler/BounceTrackToAudioCommandHandler.py
+-rw-rw-rw-  2.0 fat      776 b- defN 23-Jun-03 03:51 application/command_handler/CheckAudioExportValidCommandHandler.py
+-rw-rw-rw-  2.0 fat      423 b- defN 23-Jun-03 03:51 application/command_handler/CommandHandlerInterface.py
+-rw-rw-rw-  2.0 fat      502 b- defN 23-Jun-03 03:51 application/command_handler/DrumRackToSimplerCommandHandler.py
+-rw-rw-rw-  2.0 fat      528 b- defN 23-Jun-03 03:51 application/command_handler/EmitBackendEventCommandHandler.py
+-rw-rw-rw-  2.0 fat     1858 b- defN 23-Jun-03 03:51 application/command_handler/FireSceneToPositionCommandHandler.py
+-rw-rw-rw-  2.0 fat      506 b- defN 23-Jun-03 03:51 application/command_handler/FireSelectedSceneCommandHandler.py
+-rw-rw-rw-  2.0 fat      405 b- defN 23-Jun-03 03:51 application/command_handler/GetSetStateCommandHandler.py
+-rw-rw-rw-  2.0 fat      426 b- defN 23-Jun-03 03:51 application/command_handler/GoToGroupTrackCommandHandler.py
+-rw-rw-rw-  2.0 fat      489 b- defN 23-Jun-03 03:51 application/command_handler/LoadDeviceCommandHandler.py
+-rw-rw-rw-  2.0 fat      664 b- defN 23-Jun-03 03:51 application/command_handler/LoadDrumRackCommandHandler.py
+-rw-rw-rw-  2.0 fat      505 b- defN 23-Jun-03 03:51 application/command_handler/LoadMatchingTrackCommandHandler.py
+-rw-rw-rw-  2.0 fat      517 b- defN 23-Jun-03 03:51 application/command_handler/LoadMinitaurCommandHandler.py
+-rw-rw-rw-  2.0 fat      491 b- defN 23-Jun-03 03:51 application/command_handler/LoadRev2CommandHandler.py
+-rw-rw-rw-  2.0 fat     1581 b- defN 23-Jun-03 03:51 application/command_handler/MidiNoteCommandHandler.py
+-rw-rw-rw-  2.0 fat      453 b- defN 23-Jun-03 03:51 application/command_handler/PlayPauseSongCommandHandler.py
+-rw-rw-rw-  2.0 fat      620 b- defN 23-Jun-03 03:51 application/command_handler/RecordUnlimitedCommandHandler.py
+-rw-rw-rw-  2.0 fat      736 b- defN 23-Jun-03 03:51 application/command_handler/ReloadScriptCommandHandler.py
+-rw-rw-rw-  2.0 fat      435 b- defN 23-Jun-03 03:51 application/command_handler/ResetPlaybackCommandHandler.py
+-rw-rw-rw-  2.0 fat      560 b- defN 23-Jun-03 03:51 application/command_handler/ScrollScenePositionCommandHandler.py
+-rw-rw-rw-  2.0 fat      417 b- defN 23-Jun-03 03:51 application/command_handler/ScrollSceneTracksCommandHandler.py
+-rw-rw-rw-  2.0 fat      451 b- defN 23-Jun-03 03:51 application/command_handler/ScrollScenesCommandHandler.py
+-rw-rw-rw-  2.0 fat      427 b- defN 23-Jun-03 03:51 application/command_handler/ScrollTrackVolumeCommandHandler.py
+-rw-rw-rw-  2.0 fat      574 b- defN 23-Jun-03 03:51 application/command_handler/SelectOrLoadDeviceCommandHandler.py
+-rw-rw-rw-  2.0 fat      571 b- defN 23-Jun-03 03:51 application/command_handler/SelectTrackCommandHandler.py
+-rw-rw-rw-  2.0 fat      475 b- defN 23-Jun-03 03:51 application/command_handler/ShowAutomationCommandHandler.py
+-rw-rw-rw-  2.0 fat      515 b- defN 23-Jun-03 03:51 application/command_handler/ShowInstrumentCommandHandler.py
+-rw-rw-rw-  2.0 fat      398 b- defN 23-Jun-03 03:51 application/command_handler/ShowMessageCommandHandler.py
+-rw-rw-rw-  2.0 fat      465 b- defN 23-Jun-03 03:51 application/command_handler/ToggleArmCommandJHandler.py
+-rw-rw-rw-  2.0 fat      370 b- defN 23-Jun-03 03:51 application/command_handler/ToggleNotesCommandHandler.py
+-rw-rw-rw-  2.0 fat      402 b- defN 23-Jun-03 03:51 application/command_handler/ToggleReferenceTrackCommandHandler.py
+-rw-rw-rw-  2.0 fat      457 b- defN 23-Jun-03 03:51 application/command_handler/ToggleSceneLoopCommandHandler.py
+-rw-rw-rw-  2.0 fat      397 b- defN 23-Jun-03 03:51 application/command_handler/UnfoldSelectedSceneCommandHandler.py
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 15:31 application/command_handler/__init__.py
+-rw-rw-rw-  2.0 fat      742 b- defN 23-Jun-03 03:51 application/control_surface/ActionGroupFactory.py
+-rw-rw-rw-  2.0 fat     2700 b- defN 23-Jun-03 03:51 application/control_surface/ActionGroupInterface.py
+-rw-rw-rw-  2.0 fat     2923 b- defN 23-Jun-03 03:51 application/control_surface/EncoderAction.py
+-rw-rw-rw-  2.0 fat      163 b- defN 23-Jun-03 03:51 application/control_surface/EncoderMoveEnum.py
+-rw-rw-rw-  2.0 fat     5418 b- defN 23-Jun-03 03:51 application/control_surface/MultiEncoder.py
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 15:31 application/control_surface/__init__.py
+-rw-rw-rw-  2.0 fat     1296 b- defN 23-Jun-03 03:51 application/control_surface/group/ActionGroupClip.py
+-rw-rw-rw-  2.0 fat     1238 b- defN 23-Jun-03 03:51 application/control_surface/group/ActionGroupCut.py
+-rw-rw-rw-  2.0 fat      852 b- defN 23-Jun-03 03:51 application/control_surface/group/ActionGroupFix.py
+-rw-rw-rw-  2.0 fat     1200 b- defN 23-Jun-03 03:51 application/control_surface/group/ActionGroupLog.py
+-rw-rw-rw-  2.0 fat     3890 b- defN 23-Jun-03 03:51 application/control_surface/group/ActionGroupMain.py
+-rw-rw-rw-  2.0 fat      575 b- defN 23-Jun-03 03:51 application/control_surface/group/ActionGroupSample.py
+-rw-rw-rw-  2.0 fat      945 b- defN 23-Jun-03 03:51 application/control_surface/group/ActionGroupSet.py
+-rw-rw-rw-  2.0 fat     2040 b- defN 23-Jun-03 03:51 application/control_surface/group/ActionGroupTest.py
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 15:31 application/control_surface/group/__init__.py
+-rw-rw-rw-  2.0 fat     1060 b- defN 23-Jun-03 03:51 application/control_surface/group/legacy/ActionGroupPreset.py
+-rw-rw-rw-  2.0 fat        0 b- defN 23-May-16 17:22 application/control_surface/group/legacy/__init__.py
+-rw-rw-rw-  2.0 fat     6026 b- defN 23-Jun-03 03:51 application/error/ErrorService.py
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 15:31 application/error/__init__.py
+-rw-rw-rw-  2.0 fat     5848 b- defN 23-Jun-03 03:51 application/push2/P0Push2.py
+-rw-rw-rw-  2.0 fat     4028 b- defN 23-Jun-03 03:51 application/push2/P0SessionRingTrackProvider.py
+-rw-rw-rw-  2.0 fat      658 b- defN 23-Jun-03 03:51 application/push2/P0ShowInstrumentMode.py
+-rw-rw-rw-  2.0 fat      555 b- defN 23-Jun-03 03:51 application/push2/P0TrackListComponent.py
+-rw-rw-rw-  2.0 fat      476 b- defN 22-Oct-29 15:31 application/push2/P0TransportComponent.py
+-rw-rw-rw-  2.0 fat       64 b- defN 22-Oct-29 15:31 application/push2/__init__.py
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 15:31 domain/__init__.py
+-rw-rw-rw-  2.0 fat     4797 b- defN 23-Jun-03 03:51 domain/audit/AudioLatencyAnalyzerService.py
+-rw-rw-rw-  2.0 fat     1297 b- defN 23-Jun-03 03:51 domain/audit/LOMAnalyzerService.py
+-rw-rw-rw-  2.0 fat     8527 b- defN 23-Jun-03 03:51 domain/audit/LogService.py
+-rw-rw-rw-  2.0 fat     2333 b- defN 23-Jun-03 03:51 domain/audit/SetFixerService.py
+-rw-rw-rw-  2.0 fat     3209 b- defN 23-Jun-03 03:51 domain/audit/SetUpgradeService.py
+-rw-rw-rw-  2.0 fat      382 b- defN 23-Jun-03 03:51 domain/audit/SongStatsService.py
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 15:31 domain/audit/__init__.py
+-rw-rw-rw-  2.0 fat      327 b- defN 23-Jun-03 03:51 domain/audit/utils.py
+-rw-rw-rw-  2.0 fat     1389 b- defN 23-Jun-03 03:51 domain/audit/stats/ClipStats.py
+-rw-rw-rw-  2.0 fat     3296 b- defN 23-Jun-03 03:51 domain/audit/stats/DeviceStats.py
+-rw-rw-rw-  2.0 fat     2245 b- defN 23-Jun-03 03:51 domain/audit/stats/SampleStats.py
+-rw-rw-rw-  2.0 fat      994 b- defN 23-Jun-03 03:51 domain/audit/stats/SceneStats.py
+-rw-rw-rw-  2.0 fat      945 b- defN 23-Jun-03 03:51 domain/audit/stats/SongStats.py
+-rw-rw-rw-  2.0 fat      180 b- defN 23-May-16 17:22 domain/audit/stats/Stats.py
+-rw-rw-rw-  2.0 fat      870 b- defN 23-Jun-03 03:51 domain/audit/stats/TrackStats.py
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 15:31 domain/audit/stats/__init__.py
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 15:31 domain/lom/__init__.py
+-rw-rw-rw-  2.0 fat     2351 b- defN 23-Jun-03 03:51 domain/lom/clip/AudioClip.py
+-rw-rw-rw-  2.0 fat     7726 b- defN 23-Jun-03 03:51 domain/lom/clip/Clip.py
+-rw-rw-rw-  2.0 fat      893 b- defN 23-Jun-03 03:51 domain/lom/clip/ClipAppearance.py
+-rw-rw-rw-  2.0 fat      150 b- defN 23-Jun-03 03:51 domain/lom/clip/ClipColorEnum.py
+-rw-rw-rw-  2.0 fat      183 b- defN 23-Mar-14 16:41 domain/lom/clip/ClipConfig.py
+-rw-rw-rw-  2.0 fat      287 b- defN 22-Oct-29 15:31 domain/lom/clip/ClipCreatedOrDeletedEvent.py
+-rw-rw-rw-  2.0 fat       50 b- defN 22-Oct-29 15:31 domain/lom/clip/ClipEnvelopeShowedEvent.py
+-rw-rw-rw-  2.0 fat     4139 b- defN 23-Jun-03 03:51 domain/lom/clip/ClipInfo.py
+-rw-rw-rw-  2.0 fat     5508 b- defN 23-Jun-03 03:51 domain/lom/clip/ClipLoop.py
+-rw-rw-rw-  2.0 fat     4037 b- defN 23-Jun-03 03:51 domain/lom/clip/ClipName.py
+-rw-rw-rw-  2.0 fat      900 b- defN 23-Jun-03 03:51 domain/lom/clip/ClipPlayingPosition.py
+-rw-rw-rw-  2.0 fat      192 b- defN 22-Oct-29 15:31 domain/lom/clip/ClipSlotSelectedEvent.py
+-rw-rw-rw-  2.0 fat     2060 b- defN 23-Jun-03 03:51 domain/lom/clip/ClipTail.py
+-rw-rw-rw-  2.0 fat     7258 b- defN 23-Jun-03 03:51 domain/lom/clip/MidiClip.py
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 15:31 domain/lom/clip/__init__.py
+-rw-rw-rw-  2.0 fat     3649 b- defN 23-Jun-03 03:51 domain/lom/clip/automation/ClipAutomation.py
+-rw-rw-rw-  2.0 fat     1868 b- defN 23-Jun-03 03:51 domain/lom/clip/automation/ClipAutomationEnvelope.py
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 15:31 domain/lom/clip/automation/__init__.py
+-rw-rw-rw-  2.0 fat     2594 b- defN 23-Jun-03 03:51 domain/lom/clip_slot/AudioClipSlot.py
+-rw-rw-rw-  2.0 fat     5589 b- defN 23-Jun-03 03:51 domain/lom/clip_slot/ClipSlot.py
+-rw-rw-rw-  2.0 fat      736 b- defN 22-Oct-30 13:44 domain/lom/clip_slot/ClipSlotAppearance.py
+-rw-rw-rw-  2.0 fat      171 b- defN 23-Feb-12 00:17 domain/lom/clip_slot/ClipSlotHasClipEvent.py
+-rw-rw-rw-  2.0 fat      381 b- defN 23-Jun-03 03:51 domain/lom/clip_slot/MidiClipSlot.py
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 15:31 domain/lom/clip_slot/__init__.py
+-rw-rw-rw-  2.0 fat     4627 b- defN 23-Jun-03 03:51 domain/lom/device/Device.py
+-rw-rw-rw-  2.0 fat     1405 b- defN 23-Jun-03 03:51 domain/lom/device/DeviceChain.py
+-rw-rw-rw-  2.0 fat     6758 b- defN 23-Jun-03 03:51 domain/lom/device/DeviceDisplayService.py
+-rw-rw-rw-  2.0 fat    12653 b- defN 23-Jun-03 03:51 domain/lom/device/DeviceEnum.py
+-rw-rw-rw-  2.0 fat      575 b- defN 23-Jun-03 03:51 domain/lom/device/DeviceEnumGroup.py
+-rw-rw-rw-  2.0 fat      207 b- defN 23-Jun-03 03:51 domain/lom/device/DeviceLoadedEvent.py
+-rw-rw-rw-  2.0 fat     4488 b- defN 23-Jun-03 03:51 domain/lom/device/DeviceService.py
+-rw-rw-rw-  2.0 fat     2106 b- defN 23-Jun-03 03:51 domain/lom/device/DrumPad.py
+-rw-rw-rw-  2.0 fat     1163 b- defN 23-Jun-03 03:51 domain/lom/device/DrumRackDevice.py
+-rw-rw-rw-  2.0 fat       46 b- defN 22-Oct-29 15:31 domain/lom/device/DrumRackLoadedEvent.py
+-rw-rw-rw-  2.0 fat     1541 b- defN 23-Jun-03 03:51 domain/lom/device/DrumRackSampleService.py
+-rw-rw-rw-  2.0 fat     7134 b- defN 23-Jun-03 03:51 domain/lom/device/DrumRackService.py
+-rw-rw-rw-  2.0 fat     1383 b- defN 23-Jun-03 03:51 domain/lom/device/MixerDevice.py
+-rw-rw-rw-  2.0 fat     1280 b- defN 23-Jun-03 03:51 domain/lom/device/PluginDevice.py
+-rw-rw-rw-  2.0 fat     1782 b- defN 23-Jun-03 03:51 domain/lom/device/RackDevice.py
+-rw-rw-rw-  2.0 fat     5336 b- defN 23-Jun-03 03:51 domain/lom/device/SimpleTrackDevices.py
+-rw-rw-rw-  2.0 fat     1772 b- defN 23-Jun-03 03:51 domain/lom/device/SimplerDevice.py
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 15:31 domain/lom/device/__init__.py
+-rw-rw-rw-  2.0 fat     1409 b- defN 23-Jun-03 03:51 domain/lom/device/Sample/Sample.py
+-rw-rw-rw-  2.0 fat      336 b- defN 23-Jun-03 03:51 domain/lom/device/Sample/SampleNotFoundError.py
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 15:31 domain/lom/device/Sample/__init__.py
+-rw-rw-rw-  2.0 fat     4569 b- defN 23-Jun-03 03:51 domain/lom/device_parameter/DeviceParameter.py
+-rw-rw-rw-  2.0 fat     4094 b- defN 23-Jun-03 03:51 domain/lom/device_parameter/DeviceParameterEnum.py
+-rw-rw-rw-  2.0 fat      895 b- defN 23-Jun-03 03:51 domain/lom/device_parameter/DeviceParameterValue.py
+-rw-rw-rw-  2.0 fat     1391 b- defN 23-Jun-03 03:51 domain/lom/device_parameter/LinkedDeviceParameters.py
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 15:31 domain/lom/device_parameter/__init__.py
+-rw-rw-rw-  2.0 fat      242 b- defN 23-Jun-03 03:51 domain/lom/instrument/InstrumentActivatedEvent.py
+-rw-rw-rw-  2.0 fat      227 b- defN 23-Jun-03 03:51 domain/lom/instrument/InstrumentColorEnum.py
+-rw-rw-rw-  2.0 fat     4335 b- defN 23-Jun-03 03:51 domain/lom/instrument/InstrumentDisplayService.py
+-rw-rw-rw-  2.0 fat     4153 b- defN 23-Jun-03 03:51 domain/lom/instrument/InstrumentFactory.py
+-rw-rw-rw-  2.0 fat     4330 b- defN 23-Jun-03 03:51 domain/lom/instrument/InstrumentInterface.py
+-rw-rw-rw-  2.0 fat       50 b- defN 22-Oct-29 15:31 domain/lom/instrument/InstrumentSelectedEvent.py
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 15:31 domain/lom/instrument/__init__.py
+-rw-rw-rw-  2.0 fat      564 b- defN 23-Jun-03 03:51 domain/lom/instrument/instrument/InstrumentAddictiveKeys.py
+-rw-rw-rw-  2.0 fat      470 b- defN 23-Jun-03 03:51 domain/lom/instrument/instrument/InstrumentDrumRack.py
+-rw-rw-rw-  2.0 fat      364 b- defN 23-Jun-03 03:51 domain/lom/instrument/instrument/InstrumentKontakt.py
+-rw-rw-rw-  2.0 fat      707 b- defN 23-Jun-03 03:51 domain/lom/instrument/instrument/InstrumentMinitaur.py
+-rw-rw-rw-  2.0 fat      352 b- defN 23-Jun-03 03:51 domain/lom/instrument/instrument/InstrumentOpus.py
+-rw-rw-rw-  2.0 fat      352 b- defN 23-Jun-03 03:51 domain/lom/instrument/instrument/InstrumentPlay.py
+-rw-rw-rw-  2.0 fat     2894 b- defN 23-Jun-03 03:51 domain/lom/instrument/instrument/InstrumentRev2.py
+-rw-rw-rw-  2.0 fat      270 b- defN 23-Jun-03 03:51 domain/lom/instrument/instrument/InstrumentSampler.py
+-rw-rw-rw-  2.0 fat      475 b- defN 23-Jun-03 03:51 domain/lom/instrument/instrument/InstrumentSerum.py
+-rw-rw-rw-  2.0 fat      953 b- defN 23-Jun-03 03:51 domain/lom/instrument/instrument/InstrumentSimpler.py
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 15:31 domain/lom/instrument/instrument/__init__.py
+-rw-rw-rw-  2.0 fat      953 b- defN 23-Jun-03 03:51 domain/lom/instrument/preset/InstrumentPreset.py
+-rw-rw-rw-  2.0 fat     3149 b- defN 23-Jun-03 03:51 domain/lom/instrument/preset/InstrumentPresetList.py
+-rw-rw-rw-  2.0 fat     1877 b- defN 23-Jun-03 03:51 domain/lom/instrument/preset/InstrumentPresetScrollerService.py
+-rw-rw-rw-  2.0 fat      161 b- defN 23-Jun-03 03:51 domain/lom/instrument/preset/PresetDisplayOptionEnum.py
+-rw-rw-rw-  2.0 fat      155 b- defN 22-Dec-30 11:40 domain/lom/instrument/preset/PresetProgramSelectedEvent.py
+-rw-rw-rw-  2.0 fat      145 b- defN 22-Oct-29 15:31 domain/lom/instrument/preset/SampleSelectedEvent.py
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 15:31 domain/lom/instrument/preset/__init__.py
+-rw-rw-rw-  2.0 fat      772 b- defN 23-Jun-03 03:51 domain/lom/instrument/preset/preset_changer/InstrumentRackPresetChanger.py
+-rw-rw-rw-  2.0 fat      478 b- defN 23-Jun-03 03:51 domain/lom/instrument/preset/preset_changer/PresetChangerInterface.py
+-rw-rw-rw-  2.0 fat      761 b- defN 23-Jun-03 03:51 domain/lom/instrument/preset/preset_changer/ProgramChangePresetChanger.py
+-rw-rw-rw-  2.0 fat      541 b- defN 23-Jun-03 03:51 domain/lom/instrument/preset/preset_changer/SamplePresetChanger.py
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 15:31 domain/lom/instrument/preset/preset_changer/__init__.py
+-rw-rw-rw-  2.0 fat     1962 b- defN 23-Jun-03 03:51 domain/lom/instrument/preset/preset_importer/DirectoryPresetImporter.py
+-rw-rw-rw-  2.0 fat      593 b- defN 23-Jun-03 03:51 domain/lom/instrument/preset/preset_importer/FilePresetImporter.py
+-rw-rw-rw-  2.0 fat      367 b- defN 23-Jun-03 03:51 domain/lom/instrument/preset/preset_importer/NullPresetImporter.py
+-rw-rw-rw-  2.0 fat      669 b- defN 23-Jun-03 03:51 domain/lom/instrument/preset/preset_importer/PluginDevicePresetImporter.py
+-rw-rw-rw-  2.0 fat      802 b- defN 23-Jun-03 03:51 domain/lom/instrument/preset/preset_importer/PresetImportInterface.py
+-rw-rw-rw-  2.0 fat     1754 b- defN 23-Jun-03 03:51 domain/lom/instrument/preset/preset_importer/PresetImporterFactory.py
+-rw-rw-rw-  2.0 fat      656 b- defN 23-Jun-03 03:51 domain/lom/instrument/preset/preset_importer/RackDevicePresetImporter.py
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 15:31 domain/lom/instrument/preset/preset_importer/__init__.py
+-rw-rw-rw-  2.0 fat      597 b- defN 23-Jun-03 03:51 domain/lom/instrument/preset/preset_initializer/PresetInitializerDevicePresetName.py
+-rw-rw-rw-  2.0 fat      545 b- defN 23-Jun-03 03:51 domain/lom/instrument/preset/preset_initializer/PresetInitializerGroupTrackName.py
+-rw-rw-rw-  2.0 fat      591 b- defN 23-Jun-03 03:51 domain/lom/instrument/preset/preset_initializer/PresetInitializerInterface.py
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 15:31 domain/lom/instrument/preset/preset_initializer/__init__.py
+-rw-rw-rw-  2.0 fat      915 b- defN 22-Oct-29 15:31 domain/lom/loop/LoopableInterface.py
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 15:31 domain/lom/loop/__init__.py
+-rw-rw-rw-  2.0 fat     3558 b- defN 23-Jun-03 03:51 domain/lom/note/Note.py
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 15:31 domain/lom/note/__init__.py
+-rw-rw-rw-  2.0 fat     3412 b- defN 23-Jun-03 03:51 domain/lom/sample/SampleCategory.py
+-rw-rw-rw-  2.0 fat     1205 b- defN 23-Jun-03 03:51 domain/lom/sample/SampleCategoryEnum.py
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 15:31 domain/lom/sample/__init__.py
+-rw-rw-rw-  2.0 fat     1149 b- defN 23-Jun-03 03:51 domain/lom/scene/LoopingSceneToggler.py
+-rw-rw-rw-  2.0 fat      372 b- defN 22-Oct-29 15:31 domain/lom/scene/NextSceneStartedEvent.py
+-rw-rw-rw-  2.0 fat       51 b- defN 22-Oct-29 15:31 domain/lom/scene/PlayingSceneChangedEvent.py
+-rw-rw-rw-  2.0 fat     2833 b- defN 23-Jun-03 03:51 domain/lom/scene/PlayingSceneFacade.py
+-rw-rw-rw-  2.0 fat     8331 b- defN 23-Jun-03 03:51 domain/lom/scene/Scene.py
+-rw-rw-rw-  2.0 fat      867 b- defN 23-Jun-03 03:51 domain/lom/scene/SceneAppearance.py
+-rw-rw-rw-  2.0 fat     3382 b- defN 23-Jun-03 03:51 domain/lom/scene/SceneClips.py
+-rw-rw-rw-  2.0 fat      715 b- defN 23-Jun-03 03:51 domain/lom/scene/SceneCropScroller.py
+-rw-rw-rw-  2.0 fat      202 b- defN 22-Oct-29 15:31 domain/lom/scene/SceneFiredEvent.py
+-rw-rw-rw-  2.0 fat      263 b- defN 22-Oct-29 15:31 domain/lom/scene/SceneLastBarPassedEvent.py
+-rw-rw-rw-  2.0 fat     2307 b- defN 23-Jun-03 03:51 domain/lom/scene/SceneLength.py
+-rw-rw-rw-  2.0 fat     3470 b- defN 23-Jun-03 03:51 domain/lom/scene/SceneName.py
+-rw-rw-rw-  2.0 fat     5613 b- defN 23-Jun-03 03:51 domain/lom/scene/ScenePlaybackService.py
+-rw-rw-rw-  2.0 fat     1947 b- defN 23-Jun-03 03:51 domain/lom/scene/ScenePlayingState.py
+-rw-rw-rw-  2.0 fat       53 b- defN 22-Oct-29 15:31 domain/lom/scene/ScenePositionScrolledEvent.py
+-rw-rw-rw-  2.0 fat     1707 b- defN 23-Jun-03 03:51 domain/lom/scene/ScenePositionScroller.py
+-rw-rw-rw-  2.0 fat     6000 b- defN 23-Jun-03 03:51 domain/lom/scene/SceneService.py
+-rw-rw-rw-  2.0 fat     3315 b- defN 23-Jun-03 03:51 domain/lom/scene/SceneWindow.py
+-rw-rw-rw-  2.0 fat       44 b- defN 22-Oct-29 15:31 domain/lom/scene/ScenesMappedEvent.py
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 15:31 domain/lom/scene/__init__.py
+-rw-rw-rw-  2.0 fat     4479 b- defN 23-Jun-03 03:51 domain/lom/set/AbletonSet.py
+-rw-rw-rw-  2.0 fat      260 b- defN 23-Jun-03 03:51 domain/lom/set/AbletonSetChangedEvent.py
+-rw-rw-rw-  2.0 fat      400 b- defN 23-Jun-03 03:51 domain/lom/set/MixingService.py
+-rw-rw-rw-  2.0 fat     6017 b- defN 23-Jun-03 03:51 domain/lom/set/SessionToArrangementService.py
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 15:31 domain/lom/set/__init__.py
+-rw-rw-rw-  2.0 fat     1972 b- defN 23-Jun-03 03:51 domain/lom/song/SongInitService.py
+-rw-rw-rw-  2.0 fat       47 b- defN 22-Oct-29 15:31 domain/lom/song/SongInitializedEvent.py
+-rw-rw-rw-  2.0 fat       43 b- defN 22-Oct-29 15:31 domain/lom/song/SongStartedEvent.py
+-rw-rw-rw-  2.0 fat       43 b- defN 22-Oct-29 15:31 domain/lom/song/SongStoppedEvent.py
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 15:31 domain/lom/song/__init__.py
+-rw-rw-rw-  2.0 fat     2428 b- defN 23-Jun-03 03:51 domain/lom/song/components/ClipComponent.py
+-rw-rw-rw-  2.0 fat     2410 b- defN 23-Jun-03 03:51 domain/lom/song/components/DeviceComponent.py
+-rw-rw-rw-  2.0 fat     5120 b- defN 23-Jun-03 03:51 domain/lom/song/components/PlaybackComponent.py
+-rw-rw-rw-  2.0 fat     1167 b- defN 23-Jun-03 03:51 domain/lom/song/components/QuantizationComponent.py
+-rw-rw-rw-  2.0 fat     2880 b- defN 23-Jun-03 03:51 domain/lom/song/components/RecordingComponent.py
+-rw-rw-rw-  2.0 fat     2208 b- defN 23-Jun-03 03:51 domain/lom/song/components/SceneComponent.py
+-rw-rw-rw-  2.0 fat     2483 b- defN 23-Jun-03 03:51 domain/lom/song/components/SceneCrudComponent.py
+-rw-rw-rw-  2.0 fat     1159 b- defN 23-Jun-03 03:51 domain/lom/song/components/TempoComponent.py
+-rw-rw-rw-  2.0 fat     4670 b- defN 23-Jun-03 03:51 domain/lom/song/components/TrackComponent.py
+-rw-rw-rw-  2.0 fat     1978 b- defN 23-Jun-03 03:51 domain/lom/song/components/TrackCrudComponent.py
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 15:31 domain/lom/song/components/__init__.py
+-rw-rw-rw-  2.0 fat      125 b- defN 23-Jun-03 03:51 domain/lom/track/CurrentMonitoringStateEnum.py
+-rw-rw-rw-  2.0 fat      205 b- defN 23-May-16 17:22 domain/lom/track/P0TrackInterface.py
+-rw-rw-rw-  2.0 fat       52 b- defN 22-Oct-29 15:31 domain/lom/track/SelectedTrackChangedEvent.py
+-rw-rw-rw-  2.0 fat       42 b- defN 22-Oct-29 15:31 domain/lom/track/TrackAddedEvent.py
+-rw-rw-rw-  2.0 fat     5976 b- defN 23-Jun-03 03:51 domain/lom/track/TrackAutomationService.py
+-rw-rw-rw-  2.0 fat      156 b- defN 23-Jun-03 03:51 domain/lom/track/TrackColorEnum.py
+-rw-rw-rw-  2.0 fat      276 b- defN 23-Jun-03 03:51 domain/lom/track/TrackDisconnectedEvent.py
+-rw-rw-rw-  2.0 fat     4541 b- defN 23-Jun-03 03:51 domain/lom/track/TrackFactory.py
+-rw-rw-rw-  2.0 fat     8569 b- defN 23-Jun-03 03:51 domain/lom/track/TrackMapperService.py
+-rw-rw-rw-  2.0 fat     1014 b- defN 23-Jun-03 03:51 domain/lom/track/TrackService.py
+-rw-rw-rw-  2.0 fat       44 b- defN 22-Oct-29 15:31 domain/lom/track/TracksMappedEvent.py
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 15:31 domain/lom/track/__init__.py
+-rw-rw-rw-  2.0 fat     1469 b- defN 23-Jun-03 03:51 domain/lom/track/abstract_track/AbstrackTrackArmState.py
+-rw-rw-rw-  2.0 fat     5998 b- defN 23-Jun-03 03:51 domain/lom/track/abstract_track/AbstractTrack.py
+-rw-rw-rw-  2.0 fat     2133 b- defN 23-Jun-03 03:51 domain/lom/track/abstract_track/AbstractTrackAppearance.py
+-rw-rw-rw-  2.0 fat       56 b- defN 22-Oct-29 15:31 domain/lom/track/abstract_track/AbstractTrackNameUpdatedEvent.py
+-rw-rw-rw-  2.0 fat      179 b- defN 22-Oct-29 15:31 domain/lom/track/abstract_track/AbstractTrackSelectedEvent.py
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 15:31 domain/lom/track/abstract_track/__init__.py
+-rw-rw-rw-  2.0 fat     3757 b- defN 23-Jun-03 03:51 domain/lom/track/group_track/AbstractGroupTrack.py
+-rw-rw-rw-  2.0 fat      365 b- defN 23-Jun-03 03:51 domain/lom/track/group_track/DrumsTrack.py
+-rw-rw-rw-  2.0 fat      957 b- defN 23-Jun-03 03:51 domain/lom/track/group_track/NormalGroupMatchingTrack.py
+-rw-rw-rw-  2.0 fat     1522 b- defN 23-Jun-03 03:51 domain/lom/track/group_track/NormalGroupMatchingTrackCreator.py
+-rw-rw-rw-  2.0 fat     3653 b- defN 23-Jun-03 03:51 domain/lom/track/group_track/NormalGroupTrack.py
+-rw-rw-rw-  2.0 fat      145 b- defN 23-Jun-03 03:51 domain/lom/track/group_track/VocalsTrack.py
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 15:31 domain/lom/track/group_track/__init__.py
+-rw-rw-rw-  2.0 fat     2214 b- defN 23-Jun-03 03:51 domain/lom/track/group_track/ext_track/ExtArmState.py
+-rw-rw-rw-  2.0 fat      261 b- defN 23-Jun-03 03:51 domain/lom/track/group_track/ext_track/ExtArmedEvent.py
+-rw-rw-rw-  2.0 fat     2519 b- defN 23-Jun-03 03:51 domain/lom/track/group_track/ext_track/ExtMatchingTrack.py
+-rw-rw-rw-  2.0 fat     2900 b- defN 23-Jun-03 03:51 domain/lom/track/group_track/ext_track/ExtMatchingTrackCreator.py
+-rw-rw-rw-  2.0 fat     1912 b- defN 23-Jun-03 03:51 domain/lom/track/group_track/ext_track/ExtMonitoringState.py
+-rw-rw-rw-  2.0 fat     2095 b- defN 23-Jun-03 03:51 domain/lom/track/group_track/ext_track/ExtSoloState.py
+-rw-rw-rw-  2.0 fat     4200 b- defN 23-Jun-03 03:51 domain/lom/track/group_track/ext_track/ExternalSynthTrack.py
+-rw-rw-rw-  2.0 fat      642 b- defN 23-Jun-03 03:51 domain/lom/track/group_track/ext_track/SimpleAudioExtTrack.py
+-rw-rw-rw-  2.0 fat      807 b- defN 23-Jun-03 03:51 domain/lom/track/group_track/ext_track/SimpleBaseExtTrack.py
+-rw-rw-rw-  2.0 fat      729 b- defN 23-Jun-03 03:51 domain/lom/track/group_track/ext_track/SimpleMidiExtTrack.py
+-rw-rw-rw-  2.0 fat        0 b- defN 23-Feb-12 00:17 domain/lom/track/group_track/ext_track/__init__.py
+-rw-rw-rw-  2.0 fat     1962 b- defN 23-Jun-03 03:51 domain/lom/track/group_track/matching_track/MatchingTrackClipColorManager.py
+-rw-rw-rw-  2.0 fat     3554 b- defN 23-Jun-03 03:51 domain/lom/track/group_track/matching_track/MatchingTrackClipManager.py
+-rw-rw-rw-  2.0 fat      615 b- defN 23-Jun-03 03:51 domain/lom/track/group_track/matching_track/MatchingTrackCreatorInterface.py
+-rw-rw-rw-  2.0 fat     1965 b- defN 23-Jun-03 03:51 domain/lom/track/group_track/matching_track/MatchingTrackInterface.py
+-rw-rw-rw-  2.0 fat     2230 b- defN 23-Jun-03 03:51 domain/lom/track/group_track/matching_track/MatchingTrackRouter.py
+-rw-rw-rw-  2.0 fat     6979 b- defN 23-Jun-03 03:51 domain/lom/track/group_track/matching_track/MatchingTrackService.py
+-rw-rw-rw-  2.0 fat      926 b- defN 23-Jun-03 03:51 domain/lom/track/group_track/matching_track/MatchingTrackSoloState.py
+-rw-rw-rw-  2.0 fat        0 b- defN 23-Feb-12 00:17 domain/lom/track/group_track/matching_track/__init__.py
+-rw-rw-rw-  2.0 fat     2049 b- defN 23-Jun-03 03:51 domain/lom/track/group_track/matching_track/utils.py
+-rw-rw-rw-  2.0 fat      227 b- defN 23-Jun-03 03:51 domain/lom/track/routing/InputRoutingChannelEnum.py
+-rw-rw-rw-  2.0 fat      241 b- defN 23-Jun-03 03:51 domain/lom/track/routing/InputRoutingTypeEnum.py
+-rw-rw-rw-  2.0 fat      241 b- defN 23-Jun-03 03:51 domain/lom/track/routing/OutputRoutingTypeEnum.py
+-rw-rw-rw-  2.0 fat     1746 b- defN 23-Jun-03 03:51 domain/lom/track/routing/RoutingDisplayNameDescriptor.py
+-rw-rw-rw-  2.0 fat     3516 b- defN 23-Jun-03 03:51 domain/lom/track/routing/RoutingTrackDescriptor.py
+-rw-rw-rw-  2.0 fat      729 b- defN 23-Jun-03 03:51 domain/lom/track/routing/TrackInputRouting.py
+-rw-rw-rw-  2.0 fat      555 b- defN 23-Jun-03 03:51 domain/lom/track/routing/TrackOutputRouting.py
+-rw-rw-rw-  2.0 fat      441 b- defN 22-Oct-29 15:31 domain/lom/track/routing/TrackRoutingInterface.py
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 15:31 domain/lom/track/routing/__init__.py
+-rw-rw-rw-  2.0 fat     2882 b- defN 23-Jun-03 03:51 domain/lom/track/simple_track/AudioToMidiClipMapping.py
+-rw-rw-rw-  2.0 fat     2562 b- defN 23-Jun-03 03:51 domain/lom/track/simple_track/SimpleMatchingTrack.py
+-rw-rw-rw-  2.0 fat     1498 b- defN 23-Jun-03 03:51 domain/lom/track/simple_track/SimpleMatchingTrackCreator.py
+-rw-rw-rw-  2.0 fat    15916 b- defN 23-Jun-03 03:51 domain/lom/track/simple_track/SimpleTrack.py
+-rw-rw-rw-  2.0 fat     1365 b- defN 23-Jun-03 03:51 domain/lom/track/simple_track/SimpleTrackArmState.py
+-rw-rw-rw-  2.0 fat      174 b- defN 22-Oct-29 15:31 domain/lom/track/simple_track/SimpleTrackArmedEvent.py
+-rw-rw-rw-  2.0 fat     1357 b- defN 23-Jun-03 03:51 domain/lom/track/simple_track/SimpleTrackClipColorManager.py
+-rw-rw-rw-  2.0 fat     4608 b- defN 23-Jun-03 03:51 domain/lom/track/simple_track/SimpleTrackClipSlots.py
+-rw-rw-rw-  2.0 fat      998 b- defN 23-Jun-03 03:51 domain/lom/track/simple_track/SimpleTrackClips.py
+-rw-rw-rw-  2.0 fat      269 b- defN 23-Jun-03 03:51 domain/lom/track/simple_track/SimpleTrackCreatedEvent.py
+-rw-rw-rw-  2.0 fat      269 b- defN 23-Jun-03 03:51 domain/lom/track/simple_track/SimpleTrackDeletedEvent.py
+-rw-rw-rw-  2.0 fat      237 b- defN 23-Jun-03 03:51 domain/lom/track/simple_track/SimpleTrackFlattenedEvent.py
+-rw-rw-rw-  2.0 fat     1179 b- defN 23-Jun-03 03:51 domain/lom/track/simple_track/SimpleTrackMonitoringState.py
+-rw-rw-rw-  2.0 fat       54 b- defN 23-Mar-06 23:47 domain/lom/track/simple_track/SimpleTrackSaveStartedEvent.py
+-rw-rw-rw-  2.0 fat      854 b- defN 23-Jun-03 03:51 domain/lom/track/simple_track/SimpleTrackService.py
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 15:31 domain/lom/track/simple_track/__init__.py
+-rw-rw-rw-  2.0 fat     4827 b- defN 23-Jun-03 03:51 domain/lom/track/simple_track/audio/SimpleAudioTrack.py
+-rw-rw-rw-  2.0 fat      620 b- defN 23-Jun-03 03:51 domain/lom/track/simple_track/audio/SimpleReturnTrack.py
+-rw-rw-rw-  2.0 fat        0 b- defN 23-Feb-12 00:17 domain/lom/track/simple_track/audio/__init__.py
+-rw-rw-rw-  2.0 fat     1901 b- defN 23-Jun-03 03:51 domain/lom/track/simple_track/audio/master/MasterTrack.py
+-rw-rw-rw-  2.0 fat        0 b- defN 23-Feb-12 00:17 domain/lom/track/simple_track/audio/master/__init__.py
+-rw-rw-rw-  2.0 fat     1223 b- defN 23-Jun-03 03:51 domain/lom/track/simple_track/audio/special/ReferenceTrack.py
+-rw-rw-rw-  2.0 fat      387 b- defN 23-Jun-03 03:51 domain/lom/track/simple_track/audio/special/ResamplingTrack.py
+-rw-rw-rw-  2.0 fat        0 b- defN 23-Feb-12 00:17 domain/lom/track/simple_track/audio/special/__init__.py
+-rw-rw-rw-  2.0 fat     1496 b- defN 23-Jun-03 03:51 domain/lom/track/simple_track/midi/SimpleMidiTrack.py
+-rw-rw-rw-  2.0 fat        0 b- defN 23-Feb-12 00:17 domain/lom/track/simple_track/midi/__init__.py
+-rw-rw-rw-  2.0 fat     2627 b- defN 23-Jun-03 03:51 domain/lom/track/simple_track/midi/special/UsamoTrack.py
+-rw-rw-rw-  2.0 fat        0 b- defN 23-Feb-12 00:17 domain/lom/track/simple_track/midi/special/__init__.py
+-rw-rw-rw-  2.0 fat     2043 b- defN 23-Jun-03 03:51 domain/lom/validation/ValidatorFactory.py
+-rw-rw-rw-  2.0 fat      549 b- defN 23-Jun-03 03:51 domain/lom/validation/ValidatorInterface.py
+-rw-rw-rw-  2.0 fat     1827 b- defN 23-Jun-03 03:51 domain/lom/validation/ValidatorService.py
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 15:31 domain/lom/validation/__init__.py
+-rw-rw-rw-  2.0 fat      365 b- defN 23-Jun-03 03:51 domain/lom/validation/object_validators/AbstractGroupTrackValidator.py
+-rw-rw-rw-  2.0 fat      910 b- defN 23-Jun-03 03:51 domain/lom/validation/object_validators/SceneValidator.py
+-rw-rw-rw-  2.0 fat      898 b- defN 23-Jun-03 03:51 domain/lom/validation/object_validators/SimpleAudioTrackValidator.py
+-rw-rw-rw-  2.0 fat      393 b- defN 23-Jun-03 03:51 domain/lom/validation/object_validators/SimpleTrackValidator.py
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 15:31 domain/lom/validation/object_validators/__init__.py
+-rw-rw-rw-  2.0 fat     2017 b- defN 23-Jun-03 03:51 domain/lom/validation/object_validators/external_synth_track/ExternalSynthTrackValidator.py
+-rw-rw-rw-  2.0 fat     1665 b- defN 23-Jun-03 03:51 domain/lom/validation/object_validators/external_synth_track/SimpleAudioExtTrackValidator.py
+-rw-rw-rw-  2.0 fat     2036 b- defN 23-Jun-03 03:51 domain/lom/validation/object_validators/external_synth_track/SimpleMidiExtTrackValidator.py
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 15:31 domain/lom/validation/object_validators/external_synth_track/__init__.py
+-rw-rw-rw-  2.0 fat     1033 b- defN 23-Jun-03 03:51 domain/lom/validation/sub_validators/AggregateValidator.py
+-rw-rw-rw-  2.0 fat     1086 b- defN 23-Jun-03 03:51 domain/lom/validation/sub_validators/CallbackValidator.py
+-rw-rw-rw-  2.0 fat     1530 b- defN 23-Jun-03 03:51 domain/lom/validation/sub_validators/DeviceParameterValidator.py
+-rw-rw-rw-  2.0 fat     1872 b- defN 23-Jun-03 03:51 domain/lom/validation/sub_validators/PropertyValueValidator.py
+-rw-rw-rw-  2.0 fat     1305 b- defN 23-Jun-03 03:51 domain/lom/validation/sub_validators/SimpleTrackHasDeviceValidator.py
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 15:31 domain/lom/validation/sub_validators/__init__.py
+-rw-rw-rw-  2.0 fat     3690 b- defN 23-Jun-03 03:51 domain/shared/ApplicationView.py
+-rw-rw-rw-  2.0 fat      624 b- defN 23-Jun-03 03:51 domain/shared/BrowserServiceInterface.py
+-rw-rw-rw-  2.0 fat      118 b- defN 22-Oct-29 15:31 domain/shared/InterfaceClicksServiceInterface.py
+-rw-rw-rw-  2.0 fat      570 b- defN 23-May-16 17:22 domain/shared/LiveObject.py
+-rw-rw-rw-  2.0 fat     1946 b- defN 23-Jun-03 03:51 domain/shared/LiveObjectMapping.py
+-rw-rw-rw-  2.0 fat      139 b- defN 22-Oct-29 15:31 domain/shared/SessionServiceInterface.py
+-rw-rw-rw-  2.0 fat     2207 b- defN 23-Jun-03 03:51 domain/shared/ValueScroller.py
+-rw-rw-rw-  2.0 fat      993 b- defN 23-Jun-03 03:51 domain/shared/ValueToggler.py
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 15:31 domain/shared/__init__.py
+-rw-rw-rw-  2.0 fat     1287 b- defN 23-Jun-03 03:51 domain/shared/backend/Backend.py
+-rw-rw-rw-  2.0 fat      190 b- defN 23-Mar-06 23:47 domain/shared/backend/BackendEvent.py
+-rw-rw-rw-  2.0 fat      103 b- defN 22-Oct-29 15:31 domain/shared/backend/NotificationColorEnum.py
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 15:31 domain/shared/backend/__init__.py
+-rw-rw-rw-  2.0 fat      178 b- defN 22-Oct-29 15:31 domain/shared/errors/ErrorRaisedEvent.py
+-rw-rw-rw-  2.0 fat       47 b- defN 22-Oct-29 15:31 domain/shared/errors/Protocol0Error.py
+-rw-rw-rw-  2.0 fat      349 b- defN 23-Jun-03 03:51 domain/shared/errors/Protocol0Warning.py
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 15:31 domain/shared/errors/__init__.py
+-rw-rw-rw-  2.0 fat      575 b- defN 23-Jun-03 03:51 domain/shared/errors/error_handler.py
+-rw-rw-rw-  2.0 fat     4585 b- defN 23-Jun-03 03:51 domain/shared/event/DomainEventBus.py
+-rw-rw-rw-  2.0 fat      200 b- defN 23-May-16 17:22 domain/shared/event/HasEmitter.py
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 15:31 domain/shared/event/__init__.py
+-rw-rw-rw-  2.0 fat       42 b- defN 22-Oct-29 15:31 domain/shared/scheduler/BarChangedEvent.py
+-rw-rw-rw-  2.0 fat       41 b- defN 22-Oct-29 15:31 domain/shared/scheduler/BarEndingEvent.py
+-rw-rw-rw-  2.0 fat      309 b- defN 22-Oct-29 15:31 domain/shared/scheduler/BeatSchedulerInterface.py
+-rw-rw-rw-  2.0 fat       46 b- defN 22-Oct-29 15:31 domain/shared/scheduler/Last16thPassedEvent.py
+-rw-rw-rw-  2.0 fat       46 b- defN 22-Oct-29 15:31 domain/shared/scheduler/Last32thPassedEvent.py
+-rw-rw-rw-  2.0 fat       45 b- defN 22-Oct-29 15:31 domain/shared/scheduler/Last8thPassedEvent.py
+-rw-rw-rw-  2.0 fat       46 b- defN 22-Oct-29 15:31 domain/shared/scheduler/LastBeatPassedEvent.py
+-rw-rw-rw-  2.0 fat     2500 b- defN 23-Jun-03 03:51 domain/shared/scheduler/Scheduler.py
+-rw-rw-rw-  2.0 fat       47 b- defN 22-Oct-29 15:31 domain/shared/scheduler/ThirdBeatPassedEvent.py
+-rw-rw-rw-  2.0 fat      130 b- defN 22-Oct-29 15:31 domain/shared/scheduler/TickSchedulerEventInterface.py
+-rw-rw-rw-  2.0 fat      555 b- defN 23-Jun-03 03:51 domain/shared/scheduler/TickSchedulerInterface.py
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 15:31 domain/shared/scheduler/__init__.py
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 15:31 domain/shared/script/__init__.py
+-rw-rw-rw-  2.0 fat      118 b- defN 23-Jun-03 03:51 domain/shared/ui/ColorEnum.py
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 15:31 domain/shared/ui/__init__.py
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 15:31 domain/shared/utils/__init__.py
+-rw-rw-rw-  2.0 fat      954 b- defN 23-Jun-03 03:51 domain/shared/utils/concurrency.py
+-rw-rw-rw-  2.0 fat      914 b- defN 23-Jun-03 03:51 domain/shared/utils/debug.py
+-rw-rw-rw-  2.0 fat     1607 b- defN 22-Oct-29 15:31 domain/shared/utils/forward_to.py
+-rw-rw-rw-  2.0 fat     3193 b- defN 23-Jun-03 03:51 domain/shared/utils/func.py
+-rw-rw-rw-  2.0 fat      260 b- defN 23-Jun-03 03:51 domain/shared/utils/list.py
+-rw-rw-rw-  2.0 fat      545 b- defN 23-May-16 17:22 domain/shared/utils/string.py
+-rw-rw-rw-  2.0 fat     4769 b- defN 23-Jun-03 03:51 domain/shared/utils/timing.py
+-rw-rw-rw-  2.0 fat     3475 b- defN 23-Jun-03 03:51 domain/shared/utils/utils.py
+-rw-rw-rw-  2.0 fat      647 b- defN 23-Jun-03 03:51 domain/track_recorder/AbstractRecorderFactory.py
+-rw-rw-rw-  2.0 fat     3192 b- defN 23-Jun-03 03:51 domain/track_recorder/BaseRecorder.py
+-rw-rw-rw-  2.0 fat      640 b- defN 23-Jun-03 03:51 domain/track_recorder/RecordProcessorInterface.py
+-rw-rw-rw-  2.0 fat     7566 b- defN 23-Jun-03 03:51 domain/track_recorder/RecordService.py
+-rw-rw-rw-  2.0 fat      859 b- defN 23-Jun-03 03:51 domain/track_recorder/RecordTypeEnum.py
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 15:31 domain/track_recorder/__init__.py
+-rw-rw-rw-  2.0 fat     1769 b- defN 23-Jun-03 03:51 domain/track_recorder/config/RecordConfig.py
+-rw-rw-rw-  2.0 fat     1192 b- defN 23-Jun-03 03:51 domain/track_recorder/config/RecordProcessors.py
+-rw-rw-rw-  2.0 fat        0 b- defN 23-Feb-12 00:17 domain/track_recorder/config/__init__.py
+-rw-rw-rw-  2.0 fat      382 b- defN 23-Jun-03 03:51 domain/track_recorder/count_in/CountInInterface.py
+-rw-rw-rw-  2.0 fat     1603 b- defN 23-Jun-03 03:51 domain/track_recorder/count_in/CountInOneBar.py
+-rw-rw-rw-  2.0 fat      605 b- defN 23-Jun-03 03:51 domain/track_recorder/count_in/CountInShort.py
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 15:31 domain/track_recorder/count_in/__init__.py
+-rw-rw-rw-  2.0 fat       47 b- defN 23-Feb-12 00:17 domain/track_recorder/event/RecordCancelledEvent.py
+-rw-rw-rw-  2.0 fat       41 b- defN 23-Feb-12 00:17 domain/track_recorder/event/RecordEndedEvent.py
+-rw-rw-rw-  2.0 fat      265 b- defN 23-Feb-12 00:17 domain/track_recorder/event/RecordStartedEvent.py
+-rw-rw-rw-  2.0 fat        0 b- defN 23-Feb-12 00:17 domain/track_recorder/event/__init__.py
+-rw-rw-rw-  2.0 fat       47 b- defN 23-Feb-12 00:17 domain/track_recorder/external_synth/AudioClipSilentEvent.py
+-rw-rw-rw-  2.0 fat      255 b- defN 23-Jun-03 03:51 domain/track_recorder/external_synth/ExtAudioRecordingEndedEvent.py
+-rw-rw-rw-  2.0 fat      257 b- defN 23-Jun-03 03:51 domain/track_recorder/external_synth/ExtAudioRecordingStartedEvent.py
+-rw-rw-rw-  2.0 fat     2986 b- defN 23-Jun-03 03:51 domain/track_recorder/external_synth/OnRecordEndClipTail.py
+-rw-rw-rw-  2.0 fat     4630 b- defN 23-Jun-03 03:51 domain/track_recorder/external_synth/TrackRecorderExternalSynthFactory.py
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 15:31 domain/track_recorder/external_synth/__init__.py
+-rw-rw-rw-  2.0 fat     1868 b- defN 23-Jun-03 03:51 domain/track_recorder/external_synth/record_audio/PostRecordAudio.py
+-rw-rw-rw-  2.0 fat      944 b- defN 23-Jun-03 03:51 domain/track_recorder/external_synth/record_audio/PostRecordAudioFull.py
+-rw-rw-rw-  2.0 fat      955 b- defN 23-Jun-03 03:51 domain/track_recorder/external_synth/record_audio/PreRecordAudio.py
+-rw-rw-rw-  2.0 fat        0 b- defN 23-Feb-12 00:17 domain/track_recorder/external_synth/record_audio/__init__.py
+-rw-rw-rw-  2.0 fat     2496 b- defN 23-Jun-03 03:51 domain/track_recorder/external_synth/record_audio/record_multi/PreRecordAudioMulti.py
+-rw-rw-rw-  2.0 fat     2131 b- defN 23-Jun-03 03:51 domain/track_recorder/external_synth/record_audio/record_multi/RecordAudioMulti.py
+-rw-rw-rw-  2.0 fat        0 b- defN 23-Feb-12 00:17 domain/track_recorder/external_synth/record_audio/record_multi/__init__.py
+-rw-rw-rw-  2.0 fat     1421 b- defN 23-Jun-03 03:51 domain/track_recorder/external_synth/record_midi/PostRecordMidi.py
+-rw-rw-rw-  2.0 fat      443 b- defN 23-Jun-03 03:51 domain/track_recorder/external_synth/record_midi/PreRecordMidi.py
+-rw-rw-rw-  2.0 fat        0 b- defN 23-Feb-12 00:17 domain/track_recorder/external_synth/record_midi/__init__.py
+-rw-rw-rw-  2.0 fat      555 b- defN 23-Jun-03 03:51 domain/track_recorder/recording_bar_length/RecordingBarLengthEnum.py
+-rw-rw-rw-  2.0 fat      840 b- defN 23-Jun-03 03:51 domain/track_recorder/recording_bar_length/RecordingBarLengthScroller.py
+-rw-rw-rw-  2.0 fat       65 b- defN 22-Oct-29 15:31 domain/track_recorder/recording_bar_length/SelectedRecordingBarLengthUpdatedEvent.py
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 15:31 domain/track_recorder/recording_bar_length/__init__.py
+-rw-rw-rw-  2.0 fat      663 b- defN 23-Jun-03 03:51 domain/track_recorder/simple/PostRecordSimple.py
+-rw-rw-rw-  2.0 fat     2150 b- defN 23-Jun-03 03:51 domain/track_recorder/simple/RecorderSimpleFactory.py
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 15:31 domain/track_recorder/simple/__init__.py
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 15:31 infra/__init__.py
+-rw-rw-rw-  2.0 fat     5533 b- defN 23-Jun-03 03:51 infra/interface/BrowserLoaderService.py
+-rw-rw-rw-  2.0 fat     2712 b- defN 23-Jun-03 03:51 infra/interface/BrowserService.py
+-rw-rw-rw-  2.0 fat      397 b- defN 23-Jun-03 03:51 infra/interface/InterfaceClicksService.py
+-rw-rw-rw-  2.0 fat      252 b- defN 23-Jun-03 03:51 infra/interface/PixelEnum.py
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 15:31 infra/interface/__init__.py
+-rw-rw-rw-  2.0 fat     2678 b- defN 23-Jun-03 03:51 infra/interface/session/SessionService.py
+-rw-rw-rw-  2.0 fat      226 b- defN 22-Oct-29 15:31 infra/interface/session/SessionUpdatedEvent.py
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 15:31 infra/interface/session/__init__.py
+-rw-rw-rw-  2.0 fat     2140 b- defN 23-Jun-03 03:51 infra/logging/LoggerService.py
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 15:31 infra/logging/__init__.py
+-rw-rw-rw-  2.0 fat      177 b- defN 22-Oct-29 15:31 infra/midi/MidiBytesReceivedEvent.py
+-rw-rw-rw-  2.0 fat      173 b- defN 22-Nov-09 00:32 infra/midi/MidiBytesSentEvent.py
+-rw-rw-rw-  2.0 fat     3146 b- defN 23-Jun-03 03:51 infra/midi/MidiService.py
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 15:31 infra/midi/__init__.py
+-rw-rw-rw-  2.0 fat      244 b- defN 23-Jun-03 03:51 infra/persistence/SongDataEnum.py
+-rw-rw-rw-  2.0 fat     3008 b- defN 23-Jun-03 03:51 infra/persistence/SongDataService.py
+-rw-rw-rw-  2.0 fat     1189 b- defN 23-Jun-03 03:51 infra/persistence/TrackData.py
+-rw-rw-rw-  2.0 fat      121 b- defN 23-Jun-03 03:51 infra/persistence/TrackDataEnum.py
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 15:31 infra/persistence/__init__.py
+-rw-rw-rw-  2.0 fat     5010 b- defN 23-Jun-03 03:51 infra/scheduler/BeatScheduler.py
+-rw-rw-rw-  2.0 fat      850 b- defN 23-Jun-03 03:51 infra/scheduler/BeatSchedulerEvent.py
+-rw-rw-rw-  2.0 fat     3796 b- defN 23-Jun-03 03:51 infra/scheduler/BeatTime.py
+-rw-rw-rw-  2.0 fat     2928 b- defN 23-Jun-03 03:51 infra/scheduler/TickScheduler.py
+-rw-rw-rw-  2.0 fat     1011 b- defN 23-Jun-03 03:51 infra/scheduler/TickSchedulerEvent.py
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 15:31 infra/scheduler/__init__.py
+-rw-rw-rw-  2.0 fat      803 b- defN 23-Jun-03 03:51 shared/AbstractEnum.py
+-rw-rw-rw-  2.0 fat      915 b- defN 23-Jun-03 03:51 shared/Config.py
+-rw-rw-rw-  2.0 fat    13682 b- defN 23-Jun-03 03:51 shared/Song.py
+-rw-rw-rw-  2.0 fat      596 b- defN 23-Feb-12 00:17 shared/UndoFacade.py
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 15:31 shared/__init__.py
+-rw-rw-rw-  2.0 fat      127 b- defN 23-Mar-06 23:47 shared/types.py
+-rw-rw-rw-  2.0 fat      144 b- defN 23-Jun-03 03:51 shared/logging/LogLevelEnum.py
+-rw-rw-rw-  2.0 fat     1877 b- defN 23-Jun-03 03:51 shared/logging/Logger.py
+-rw-rw-rw-  2.0 fat      261 b- defN 23-Jun-03 03:51 shared/logging/LoggerServiceInterface.py
+-rw-rw-rw-  2.0 fat      714 b- defN 23-Jun-03 03:51 shared/logging/StatusBar.py
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 15:31 shared/logging/__init__.py
+-rw-rw-rw-  2.0 fat      692 b- defN 23-Jun-03 03:51 shared/observer/Observable.py
+-rw-rw-rw-  2.0 fat      249 b- defN 23-Jun-03 03:51 shared/observer/Observer.py
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 15:31 shared/observer/__init__.py
+-rw-rw-rw-  2.0 fat      688 b- defN 23-Jun-03 03:51 shared/sequence/HasSequenceState.py
+-rw-rw-rw-  2.0 fat     2023 b- defN 23-Jun-03 03:51 shared/sequence/ParallelSequence.py
+-rw-rw-rw-  2.0 fat    11927 b- defN 23-Jun-03 03:51 shared/sequence/Sequence.py
+-rw-rw-rw-  2.0 fat     1646 b- defN 23-Jun-03 03:51 shared/sequence/SequenceState.py
+-rw-rw-rw-  2.0 fat     2789 b- defN 23-Jun-03 03:51 shared/sequence/SequenceStep.py
+-rw-rw-rw-  2.0 fat      851 b- defN 23-Jun-03 03:51 shared/sequence/SequenceTransition.py
+-rw-rw-rw-  2.0 fat     1761 b- defN 23-Jun-03 03:51 shared/sequence/TimeoutLimit.py
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 15:31 shared/sequence/__init__.py
+-rw-rw-rw-  2.0 fat      210 b- defN 23-Jun-03 03:51 tests/__init__.py
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 15:31 tests/application/__init__.py
+-rw-rw-rw-  2.0 fat     2750 b- defN 23-Jun-03 03:51 tests/application/test_multi_encoder.py
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 15:31 tests/domain/__init__.py
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 15:31 tests/domain/clip/__init__.py
+-rw-rw-rw-  2.0 fat      803 b- defN 23-Jun-03 03:51 tests/domain/clip/test_clip_playing_position.py
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 15:31 tests/domain/fixtures/__init__.py
+-rw-rw-rw-  2.0 fat     1007 b- defN 23-Jun-03 03:51 tests/domain/fixtures/clip.py
+-rw-rw-rw-  2.0 fat      437 b- defN 23-Jun-03 03:51 tests/domain/fixtures/clip_slot.py
+-rw-rw-rw-  2.0 fat       72 b- defN 22-Oct-29 15:31 tests/domain/fixtures/clip_view.py
+-rw-rw-rw-  2.0 fat      241 b- defN 23-Jun-03 03:51 tests/domain/fixtures/container.py
+-rw-rw-rw-  2.0 fat      645 b- defN 23-Jun-03 03:51 tests/domain/fixtures/device.py
+-rw-rw-rw-  2.0 fat      319 b- defN 23-Feb-12 00:17 tests/domain/fixtures/device_parameter.py
+-rw-rw-rw-  2.0 fat      842 b- defN 23-Jun-03 03:51 tests/domain/fixtures/group_track.py
+-rw-rw-rw-  2.0 fat     2436 b- defN 23-Jun-03 03:51 tests/domain/fixtures/p0.py
+-rw-rw-rw-  2.0 fat      264 b- defN 22-Oct-29 15:31 tests/domain/fixtures/scene.py
+-rw-rw-rw-  2.0 fat     3007 b- defN 23-Jun-03 03:51 tests/domain/fixtures/simple_track.py
+-rw-rw-rw-  2.0 fat     2701 b- defN 23-Jun-03 03:51 tests/domain/fixtures/song.py
+-rw-rw-rw-  2.0 fat      308 b- defN 22-Oct-29 15:31 tests/domain/fixtures/song_view.py
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 15:31 tests/domain/scene/__init__.py
+-rw-rw-rw-  2.0 fat      547 b- defN 23-Jun-03 03:51 tests/domain/scene/test_scene_clips.py
+-rw-rw-rw-  2.0 fat     1168 b- defN 23-Jun-03 03:51 tests/domain/scene/test_scene_length.py
+-rw-rw-rw-  2.0 fat     1291 b- defN 23-Jun-03 03:51 tests/domain/scene/test_scene_playing_position.py
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 15:31 tests/domain/shared/__init__.py
+-rw-rw-rw-  2.0 fat      223 b- defN 23-Jun-03 03:51 tests/domain/shared/test_decorators.py
+-rw-rw-rw-  2.0 fat      933 b- defN 23-Jun-03 03:51 tests/domain/shared/test_live_object_mapping.py
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 15:31 tests/domain/shared/event/__init__.py
+-rw-rw-rw-  2.0 fat     1187 b- defN 23-Jun-03 03:51 tests/domain/shared/event/test_domain_event_bus.py
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 15:31 tests/domain/shared/utils/__init__.py
+-rw-rw-rw-  2.0 fat      597 b- defN 23-Jun-03 03:51 tests/domain/shared/utils/test_func.py
+-rw-rw-rw-  2.0 fat     1457 b- defN 23-Jun-03 03:51 tests/domain/shared/utils/test_utils.py
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 15:31 tests/domain/track/__init__.py
+-rw-rw-rw-  2.0 fat      787 b- defN 23-Jun-03 03:51 tests/domain/track/test_audio_to_midi_clip_mapping.py
+-rw-rw-rw-  2.0 fat      846 b- defN 23-Jun-03 03:51 tests/domain/track/test_instantiation.py
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 15:31 tests/domain/validation/__init__.py
+-rw-rw-rw-  2.0 fat     1349 b- defN 23-Jun-03 03:51 tests/domain/validation/test_aggregate_validator.py
+-rw-rw-rw-  2.0 fat     1021 b- defN 23-Jun-03 03:51 tests/domain/validation/test_callback_validator.py
+-rw-rw-rw-  2.0 fat     1066 b- defN 23-Jun-03 03:51 tests/domain/validation/test_property_validator.py
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 15:31 tests/infra/__init__.py
+-rw-rw-rw-  2.0 fat     1948 b- defN 23-Jun-03 03:51 tests/infra/test_scheduler.py
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 15:31 tests/infra/listeners/__init__.py
+-rw-rw-rw-  2.0 fat     1301 b- defN 22-Oct-29 15:31 tests/infra/listeners/test_subject_slot.py
+-rw-rw-rw-  2.0 fat      494 b- defN 23-Jun-03 03:51 tests/infra/scheduler/TickSchedulerEventTest.py
+-rw-rw-rw-  2.0 fat      735 b- defN 23-Jun-03 03:51 tests/infra/scheduler/TickSchedulerTest.py
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 15:31 tests/infra/scheduler/__init__.py
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 15:31 tests/shared/__init__.py
+-rw-rw-rw-  2.0 fat      555 b- defN 23-Jun-03 03:51 tests/shared/test_container.py
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-29 15:31 tests/shared/sequence/__init__.py
+-rw-rw-rw-  2.0 fat     1405 b- defN 23-Jun-03 03:51 tests/shared/sequence/test_sanity_sequence.py
+-rw-rw-rw-  2.0 fat     3270 b- defN 23-Jun-03 03:51 tests/shared/sequence/test_sequence.py
+-rw-rw-rw-  2.0 fat     1692 b- defN 23-Jun-03 03:51 tests/shared/sequence/test_sequence_parallel.py
+-rw-rw-rw-  2.0 fat      126 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/easy_install.py
+-rw-rw-rw-  2.0 fat       24 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/__init__.py
+-rw-rw-rw-  2.0 fat      629 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/__main__.py
+-rw-rw-rw-  2.0 fat     8675 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_internal/__init__.py
+-rw-rw-rw-  2.0 fat    14014 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_internal/basecommand.py
+-rw-rw-rw-  2.0 fat     8764 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_internal/baseparser.py
+-rw-rw-rw-  2.0 fat     2773 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_internal/build_env.py
+-rw-rw-rw-  2.0 fat     7023 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_internal/cache.py
+-rw-rw-rw-  2.0 fat    16679 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_internal/cmdoptions.py
+-rw-rw-rw-  2.0 fat     7912 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_internal/compat.py
+-rw-rw-rw-  2.0 fat    13330 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_internal/configuration.py
+-rw-rw-rw-  2.0 fat    34257 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_internal/download.py
+-rw-rw-rw-  2.0 fat     8470 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_internal/exceptions.py
+-rw-rw-rw-  2.0 fat    41718 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_internal/index.py
+-rw-rw-rw-  2.0 fat     6504 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_internal/locations.py
+-rw-rw-rw-  2.0 fat    11115 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_internal/pep425tags.py
+-rw-rw-rw-  2.0 fat    13939 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_internal/resolve.py
+-rw-rw-rw-  2.0 fat      164 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_internal/status_codes.py
+-rw-rw-rw-  2.0 fat    31967 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_internal/wheel.py
+-rw-rw-rw-  2.0 fat     2297 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_internal/commands/__init__.py
+-rw-rw-rw-  2.0 fat     1500 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_internal/commands/check.py
+-rw-rw-rw-  2.0 fat     3018 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_internal/commands/completion.py
+-rw-rw-rw-  2.0 fat     7343 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_internal/commands/configuration.py
+-rw-rw-rw-  2.0 fat     9092 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_internal/commands/download.py
+-rw-rw-rw-  2.0 fat     3320 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_internal/commands/freeze.py
+-rw-rw-rw-  2.0 fat     1729 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_internal/commands/hash.py
+-rw-rw-rw-  2.0 fat     1079 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_internal/commands/help.py
+-rw-rw-rw-  2.0 fat    20270 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_internal/commands/install.py
+-rw-rw-rw-  2.0 fat    11957 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_internal/commands/list.py
+-rw-rw-rw-  2.0 fat     4842 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_internal/commands/search.py
+-rw-rw-rw-  2.0 fat     6378 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_internal/commands/show.py
+-rw-rw-rw-  2.0 fat     2786 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_internal/commands/uninstall.py
+-rw-rw-rw-  2.0 fat     6986 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_internal/commands/wheel.py
+-rw-rw-rw-  2.0 fat       85 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_internal/models/__init__.py
+-rw-rw-rw-  2.0 fat      433 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_internal/models/index.py
+-rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_internal/operations/__init__.py
+-rw-rw-rw-  2.0 fat     3776 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_internal/operations/check.py
+-rw-rw-rw-  2.0 fat    10277 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_internal/operations/freeze.py
+-rw-rw-rw-  2.0 fat    15496 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_internal/operations/prepare.py
+-rw-rw-rw-  2.0 fat     2152 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_internal/req/__init__.py
+-rw-rw-rw-  2.0 fat    12248 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_internal/req/req_file.py
+-rw-rw-rw-  2.0 fat    43930 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_internal/req/req_install.py
+-rw-rw-rw-  2.0 fat     7268 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_internal/req/req_set.py
+-rw-rw-rw-  2.0 fat    17002 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_internal/req/req_uninstall.py
+-rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_internal/utils/__init__.py
+-rw-rw-rw-  2.0 fat     9372 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_internal/utils/appdirs.py
+-rw-rw-rw-  2.0 fat     2374 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_internal/utils/deprecation.py
+-rw-rw-rw-  2.0 fat     1058 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_internal/utils/encoding.py
+-rw-rw-rw-  2.0 fat      937 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_internal/utils/filesystem.py
+-rw-rw-rw-  2.0 fat     3088 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_internal/utils/glibc.py
+-rw-rw-rw-  2.0 fat     2994 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_internal/utils/hashes.py
+-rw-rw-rw-  2.0 fat     3586 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_internal/utils/logging.py
+-rw-rw-rw-  2.0 fat    28053 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_internal/utils/misc.py
+-rw-rw-rw-  2.0 fat     5951 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_internal/utils/outdated.py
+-rw-rw-rw-  2.0 fat     2347 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_internal/utils/packaging.py
+-rw-rw-rw-  2.0 fat      286 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_internal/utils/setuptools_build.py
+-rw-rw-rw-  2.0 fat     2697 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_internal/utils/temp_dir.py
+-rw-rw-rw-  2.0 fat     1144 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_internal/utils/typing.py
+-rw-rw-rw-  2.0 fat    14058 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_internal/utils/ui.py
+-rw-rw-rw-  2.0 fat    15755 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_internal/vcs/__init__.py
+-rw-rw-rw-  2.0 fat     3848 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_internal/vcs/bazaar.py
+-rw-rw-rw-  2.0 fat    11743 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_internal/vcs/git.py
+-rw-rw-rw-  2.0 fat     3708 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_internal/vcs/mercurial.py
+-rw-rw-rw-  2.0 fat     9826 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_internal/vcs/subversion.py
+-rw-rw-rw-  2.0 fat     4841 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/__init__.py
+-rw-rw-rw-  2.0 fat    25151 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/appdirs.py
+-rw-rw-rw-  2.0 fat    40565 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/distro.py
+-rw-rw-rw-  2.0 fat    82271 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/ipaddress.py
+-rw-rw-rw-  2.0 fat   231068 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/pyparsing.py
+-rw-rw-rw-  2.0 fat    10239 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/retrying.py
+-rw-rw-rw-  2.0 fat    31779 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/six.py
+-rw-rw-rw-  2.0 fat      313 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/cachecontrol/__init__.py
+-rw-rw-rw-  2.0 fat     1380 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/cachecontrol/_cmd.py
+-rw-rw-rw-  2.0 fat     5156 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/cachecontrol/adapter.py
+-rw-rw-rw-  2.0 fat      829 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/cachecontrol/cache.py
+-rw-rw-rw-  2.0 fat      724 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/cachecontrol/compat.py
+-rw-rw-rw-  2.0 fat    14232 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/cachecontrol/controller.py
+-rw-rw-rw-  2.0 fat     2609 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/cachecontrol/filewrapper.py
+-rw-rw-rw-  2.0 fat     4282 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/cachecontrol/heuristics.py
+-rw-rw-rw-  2.0 fat     7249 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/cachecontrol/serialize.py
+-rw-rw-rw-  2.0 fat      781 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/cachecontrol/wrapper.py
+-rw-rw-rw-  2.0 fat       88 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/__init__.py
+-rw-rw-rw-  2.0 fat     4202 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py
+-rw-rw-rw-  2.0 fat     1145 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py
+-rw-rw-rw-  2.0 fat       66 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/certifi/__init__.py
+-rw-rw-rw-  2.0 fat       43 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/certifi/__main__.py
+-rw-rw-rw-  2.0 fat      873 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/certifi/core.py
+-rw-rw-rw-  2.0 fat     1598 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/chardet/__init__.py
+-rw-rw-rw-  2.0 fat    31640 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/chardet/big5freq.py
+-rw-rw-rw-  2.0 fat     1804 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/chardet/big5prober.py
+-rw-rw-rw-  2.0 fat     9644 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/chardet/chardistribution.py
+-rw-rw-rw-  2.0 fat     3893 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/chardet/charsetgroupprober.py
+-rw-rw-rw-  2.0 fat     5255 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/chardet/charsetprober.py
+-rw-rw-rw-  2.0 fat     3678 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/chardet/codingstatemachine.py
+-rw-rw-rw-  2.0 fat     1168 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/chardet/compat.py
+-rw-rw-rw-  2.0 fat     1904 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/chardet/cp949prober.py
+-rw-rw-rw-  2.0 fat     1737 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/chardet/enums.py
+-rw-rw-rw-  2.0 fat     4051 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/chardet/escprober.py
+-rw-rw-rw-  2.0 fat    10756 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/chardet/escsm.py
+-rw-rw-rw-  2.0 fat     3841 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/chardet/eucjpprober.py
+-rw-rw-rw-  2.0 fat    13741 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/chardet/euckrfreq.py
+-rw-rw-rw-  2.0 fat     1795 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/chardet/euckrprober.py
+-rw-rw-rw-  2.0 fat    32008 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/chardet/euctwfreq.py
+-rw-rw-rw-  2.0 fat     1793 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/chardet/euctwprober.py
+-rw-rw-rw-  2.0 fat    20998 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/chardet/gb2312freq.py
+-rw-rw-rw-  2.0 fat     1800 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/chardet/gb2312prober.py
+-rw-rw-rw-  2.0 fat    14130 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/chardet/hebrewprober.py
+-rw-rw-rw-  2.0 fat    26102 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/chardet/jisfreq.py
+-rw-rw-rw-  2.0 fat    19876 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/chardet/jpcntx.py
+-rw-rw-rw-  2.0 fat    13067 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/chardet/langbulgarianmodel.py
+-rw-rw-rw-  2.0 fat    18281 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/chardet/langcyrillicmodel.py
+-rw-rw-rw-  2.0 fat    12913 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/chardet/langgreekmodel.py
+-rw-rw-rw-  2.0 fat    11545 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/chardet/langhebrewmodel.py
+-rw-rw-rw-  2.0 fat    12817 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/chardet/langhungarianmodel.py
+-rw-rw-rw-  2.0 fat    11489 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/chardet/langthaimodel.py
+-rw-rw-rw-  2.0 fat    11295 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/chardet/langturkishmodel.py
+-rw-rw-rw-  2.0 fat     5515 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/chardet/latin1prober.py
+-rw-rw-rw-  2.0 fat     3504 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/chardet/mbcharsetprober.py
+-rw-rw-rw-  2.0 fat     2066 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/chardet/mbcsgroupprober.py
+-rw-rw-rw-  2.0 fat    26053 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/chardet/mbcssm.py
+-rw-rw-rw-  2.0 fat     5789 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/chardet/sbcharsetprober.py
+-rw-rw-rw-  2.0 fat     3619 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/chardet/sbcsgroupprober.py
+-rw-rw-rw-  2.0 fat     3866 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/chardet/sjisprober.py
+-rw-rw-rw-  2.0 fat    12771 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/chardet/universaldetector.py
+-rw-rw-rw-  2.0 fat     2848 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/chardet/utf8prober.py
+-rw-rw-rw-  2.0 fat      251 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/chardet/version.py
+-rw-rw-rw-  2.0 fat        2 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/chardet/cli/__init__.py
+-rw-rw-rw-  2.0 fat     2859 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/chardet/cli/chardetect.py
+-rw-rw-rw-  2.0 fat      247 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/colorama/__init__.py
+-rw-rw-rw-  2.0 fat     2626 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/colorama/ansi.py
+-rw-rw-rw-  2.0 fat     9904 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/colorama/ansitowin32.py
+-rw-rw-rw-  2.0 fat     1999 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/colorama/initialise.py
+-rw-rw-rw-  2.0 fat     5582 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/colorama/win32.py
+-rw-rw-rw-  2.0 fat     6452 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/colorama/winterm.py
+-rw-rw-rw-  2.0 fat      604 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/distlib/__init__.py
+-rw-rw-rw-  2.0 fat    42524 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/distlib/compat.py
+-rw-rw-rw-  2.0 fat    52204 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/distlib/database.py
+-rw-rw-rw-  2.0 fat    21589 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/distlib/index.py
+-rw-rw-rw-  2.0 fat    52949 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/distlib/locators.py
+-rw-rw-rw-  2.0 fat    15204 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/distlib/manifest.py
+-rw-rw-rw-  2.0 fat     4518 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/distlib/markers.py
+-rw-rw-rw-  2.0 fat    41077 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/distlib/metadata.py
+-rw-rw-rw-  2.0 fat    11121 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/distlib/resources.py
+-rw-rw-rw-  2.0 fat    17000 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/distlib/scripts.py
+-rw-rw-rw-  2.0 fat    61249 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/distlib/util.py
+-rw-rw-rw-  2.0 fat    24127 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/distlib/version.py
+-rw-rw-rw-  2.0 fat    40490 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/distlib/wheel.py
+-rw-rw-rw-  2.0 fat      280 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/distlib/_backport/__init__.py
+-rw-rw-rw-  2.0 fat     1012 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/distlib/_backport/misc.py
+-rw-rw-rw-  2.0 fat    26408 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/distlib/_backport/shutil.py
+-rw-rw-rw-  2.0 fat    27752 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/distlib/_backport/sysconfig.py
+-rw-rw-rw-  2.0 fat    95235 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/distlib/_backport/tarfile.py
+-rw-rw-rw-  2.0 fat     1197 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/html5lib/__init__.py
+-rw-rw-rw-  2.0 fat    16993 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/html5lib/_ihatexml.py
+-rw-rw-rw-  2.0 fat    33475 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/html5lib/_inputstream.py
+-rw-rw-rw-  2.0 fat    78301 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/html5lib/_tokenizer.py
+-rw-rw-rw-  2.0 fat     4139 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/html5lib/_utils.py
+-rw-rw-rw-  2.0 fat    86465 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/html5lib/constants.py
+-rw-rw-rw-  2.0 fat   121754 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/html5lib/html5parser.py
+-rw-rw-rw-  2.0 fat    16167 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/html5lib/serializer.py
+-rw-rw-rw-  2.0 fat      303 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/html5lib/_trie/__init__.py
+-rw-rw-rw-  2.0 fat      967 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/html5lib/_trie/_base.py
+-rw-rw-rw-  2.0 fat     1222 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/html5lib/_trie/datrie.py
+-rw-rw-rw-  2.0 fat     1842 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/html5lib/_trie/py.py
+-rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/html5lib/filters/__init__.py
+-rw-rw-rw-  2.0 fat      948 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/html5lib/filters/alphabeticalattributes.py
+-rw-rw-rw-  2.0 fat      298 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/html5lib/filters/base.py
+-rw-rw-rw-  2.0 fat     3018 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/html5lib/filters/inject_meta_charset.py
+-rw-rw-rw-  2.0 fat     3736 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/html5lib/filters/lint.py
+-rw-rw-rw-  2.0 fat    10795 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/html5lib/filters/optionaltags.py
+-rw-rw-rw-  2.0 fat    27144 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/html5lib/filters/sanitizer.py
+-rw-rw-rw-  2.0 fat     1252 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/html5lib/filters/whitespace.py
+-rw-rw-rw-  2.0 fat      709 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/html5lib/treeadapters/__init__.py
+-rw-rw-rw-  2.0 fat     1769 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/html5lib/treeadapters/genshi.py
+-rw-rw-rw-  2.0 fat     1826 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/html5lib/treeadapters/sax.py
+-rw-rw-rw-  2.0 fat     3680 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/html5lib/treebuilders/__init__.py
+-rw-rw-rw-  2.0 fat    14996 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/html5lib/treebuilders/base.py
+-rw-rw-rw-  2.0 fat     9071 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/html5lib/treebuilders/dom.py
+-rw-rw-rw-  2.0 fat    13104 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/html5lib/treebuilders/etree.py
+-rw-rw-rw-  2.0 fat    14488 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/html5lib/treebuilders/etree_lxml.py
+-rw-rw-rw-  2.0 fat     5868 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/html5lib/treewalkers/__init__.py
+-rw-rw-rw-  2.0 fat     7728 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/html5lib/treewalkers/base.py
+-rw-rw-rw-  2.0 fat     1456 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/html5lib/treewalkers/dom.py
+-rw-rw-rw-  2.0 fat     4680 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/html5lib/treewalkers/etree.py
+-rw-rw-rw-  2.0 fat     6522 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/html5lib/treewalkers/etree_lxml.py
+-rw-rw-rw-  2.0 fat     2378 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/html5lib/treewalkers/genshi.py
+-rw-rw-rw-  2.0 fat       60 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/idna/__init__.py
+-rw-rw-rw-  2.0 fat     3417 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/idna/codec.py
+-rw-rw-rw-  2.0 fat      244 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/idna/compat.py
+-rw-rw-rw-  2.0 fat    11777 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/idna/core.py
+-rw-rw-rw-  2.0 fat    34584 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/idna/idnadata.py
+-rw-rw-rw-  2.0 fat     1802 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/idna/intranges.py
+-rw-rw-rw-  2.0 fat       23 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/idna/package_data.py
+-rw-rw-rw-  2.0 fat   192578 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/idna/uts46data.py
+-rw-rw-rw-  2.0 fat     9718 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/lockfile/__init__.py
+-rw-rw-rw-  2.0 fat     2725 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/lockfile/linklockfile.py
+-rw-rw-rw-  2.0 fat     3180 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/lockfile/mkdirlockfile.py
+-rw-rw-rw-  2.0 fat     6280 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/lockfile/pidlockfile.py
+-rw-rw-rw-  2.0 fat     5662 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/lockfile/sqlitelockfile.py
+-rw-rw-rw-  2.0 fat     2686 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/lockfile/symlinklockfile.py
+-rw-rw-rw-  2.0 fat     1743 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/msgpack/__init__.py
+-rw-rw-rw-  2.0 fat       21 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/msgpack/_version.py
+-rw-rw-rw-  2.0 fat     1097 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/msgpack/exceptions.py
+-rw-rw-rw-  2.0 fat    37388 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/msgpack/fallback.py
+-rw-rw-rw-  2.0 fat      741 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/packaging/__about__.py
+-rw-rw-rw-  2.0 fat      527 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/packaging/__init__.py
+-rw-rw-rw-  2.0 fat      890 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/packaging/_compat.py
+-rw-rw-rw-  2.0 fat     1488 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/packaging/_structures.py
+-rw-rw-rw-  2.0 fat     8522 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/packaging/markers.py
+-rw-rw-rw-  2.0 fat     4571 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/packaging/requirements.py
+-rw-rw-rw-  2.0 fat    28800 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/packaging/specifiers.py
+-rw-rw-rw-  2.0 fat     1643 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/packaging/utils.py
+-rw-rw-rw-  2.0 fat    12660 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/packaging/version.py
+-rw-rw-rw-  2.0 fat   106604 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/pkg_resources/__init__.py
+-rw-rw-rw-  2.0 fat      622 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/pkg_resources/py31compat.py
+-rw-rw-rw-  2.0 fat     3315 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/progress/__init__.py
+-rw-rw-rw-  2.0 fat     2924 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/progress/bar.py
+-rw-rw-rw-  2.0 fat     1576 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/progress/counter.py
+-rw-rw-rw-  2.0 fat     2945 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/progress/helpers.py
+-rw-rw-rw-  2.0 fat     1483 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/progress/spinner.py
+-rw-rw-rw-  2.0 fat       95 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/pytoml/__init__.py
+-rw-rw-rw-  2.0 fat      522 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/pytoml/core.py
+-rw-rw-rw-  2.0 fat    10916 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/pytoml/parser.py
+-rw-rw-rw-  2.0 fat     3942 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/pytoml/writer.py
+-rw-rw-rw-  2.0 fat     3765 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/requests/__init__.py
+-rw-rw-rw-  2.0 fat      450 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/requests/__version__.py
+-rw-rw-rw-  2.0 fat     1138 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/requests/_internal_utils.py
+-rw-rw-rw-  2.0 fat    21541 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/requests/adapters.py
+-rw-rw-rw-  2.0 fat     6389 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/requests/api.py
+-rw-rw-rw-  2.0 fat    10021 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/requests/auth.py
+-rw-rw-rw-  2.0 fat      483 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/requests/certs.py
+-rw-rw-rw-  2.0 fat     1943 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/requests/compat.py
+-rw-rw-rw-  2.0 fat    18750 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/requests/cookies.py
+-rw-rw-rw-  2.0 fat     3237 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/requests/exceptions.py
+-rw-rw-rw-  2.0 fat     3787 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/requests/help.py
+-rw-rw-rw-  2.0 fat      801 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/requests/hooks.py
+-rw-rw-rw-  2.0 fat    35016 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/requests/models.py
+-rw-rw-rw-  2.0 fat      711 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/requests/packages.py
+-rw-rw-rw-  2.0 fat    28283 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/requests/sessions.py
+-rw-rw-rw-  2.0 fat     3414 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/requests/status_codes.py
+-rw-rw-rw-  2.0 fat     3117 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/requests/structures.py
+-rw-rw-rw-  2.0 fat    28556 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/requests/utils.py
+-rw-rw-rw-  2.0 fat     2950 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/urllib3/__init__.py
+-rw-rw-rw-  2.0 fat    10523 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/urllib3/_collections.py
+-rw-rw-rw-  2.0 fat    13376 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/urllib3/connection.py
+-rw-rw-rw-  2.0 fat    36263 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/urllib3/connectionpool.py
+-rw-rw-rw-  2.0 fat     6849 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/urllib3/exceptions.py
+-rw-rw-rw-  2.0 fat     6121 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/urllib3/fields.py
+-rw-rw-rw-  2.0 fat     2415 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/urllib3/filepost.py
+-rw-rw-rw-  2.0 fat    16785 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/urllib3/poolmanager.py
+-rw-rw-rw-  2.0 fat     6094 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/urllib3/request.py
+-rw-rw-rw-  2.0 fat    23529 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/urllib3/response.py
+-rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/urllib3/contrib/__init__.py
+-rw-rw-rw-  2.0 fat    11185 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/urllib3/contrib/appengine.py
+-rw-rw-rw-  2.0 fat     4590 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py
+-rw-rw-rw-  2.0 fat    15826 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py
+-rw-rw-rw-  2.0 fat    31311 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/urllib3/contrib/securetransport.py
+-rw-rw-rw-  2.0 fat     6383 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/urllib3/contrib/socks.py
+-rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
+-rw-rw-rw-  2.0 fat    18153 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
+-rw-rw-rw-  2.0 fat    12405 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
+-rw-rw-rw-  2.0 fat      114 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/urllib3/packages/__init__.py
+-rw-rw-rw-  2.0 fat     9194 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/urllib3/packages/ordered_dict.py
+-rw-rw-rw-  2.0 fat    30966 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/urllib3/packages/six.py
+-rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/__init__.py
+-rw-rw-rw-  2.0 fat     1514 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py
+-rw-rw-rw-  2.0 fat      707 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/urllib3/packages/ssl_match_hostname/__init__.py
+-rw-rw-rw-  2.0 fat     5876 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/urllib3/packages/ssl_match_hostname/_implementation.py
+-rw-rw-rw-  2.0 fat     1098 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/urllib3/util/__init__.py
+-rw-rw-rw-  2.0 fat     4367 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/urllib3/util/connection.py
+-rw-rw-rw-  2.0 fat     3823 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/urllib3/util/request.py
+-rw-rw-rw-  2.0 fat     2424 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/urllib3/util/response.py
+-rw-rw-rw-  2.0 fat    15002 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/urllib3/util/retry.py
+-rw-rw-rw-  2.0 fat    21728 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/urllib3/util/selectors.py
+-rw-rw-rw-  2.0 fat    12561 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/urllib3/util/ssl_.py
+-rw-rw-rw-  2.0 fat     9999 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/urllib3/util/timeout.py
+-rw-rw-rw-  2.0 fat     6717 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/urllib3/util/url.py
+-rw-rw-rw-  2.0 fat     1491 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/urllib3/util/wait.py
+-rw-rw-rw-  2.0 fat    10921 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/webencodings/__init__.py
+-rw-rw-rw-  2.0 fat     9210 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/webencodings/labels.py
+-rw-rw-rw-  2.0 fat     1364 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/webencodings/mklabels.py
+-rw-rw-rw-  2.0 fat     6716 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/webencodings/tests.py
+-rw-rw-rw-  2.0 fat     4632 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pip/_vendor/webencodings/x_user_defined.py
+-rw-rw-rw-  2.0 fat   103551 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pkg_resources/__init__.py
+-rw-rw-rw-  2.0 fat      600 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pkg_resources/py31compat.py
+-rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pkg_resources/_vendor/__init__.py
+-rw-rw-rw-  2.0 fat    22374 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pkg_resources/_vendor/appdirs.py
+-rw-rw-rw-  2.0 fat   229867 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pkg_resources/_vendor/pyparsing.py
+-rw-rw-rw-  2.0 fat    30098 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pkg_resources/_vendor/six.py
+-rw-rw-rw-  2.0 fat      720 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pkg_resources/_vendor/packaging/__about__.py
+-rw-rw-rw-  2.0 fat      513 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pkg_resources/_vendor/packaging/__init__.py
+-rw-rw-rw-  2.0 fat      860 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pkg_resources/_vendor/packaging/_compat.py
+-rw-rw-rw-  2.0 fat     1416 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pkg_resources/_vendor/packaging/_structures.py
+-rw-rw-rw-  2.0 fat     8248 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pkg_resources/_vendor/packaging/markers.py
+-rw-rw-rw-  2.0 fat     4355 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pkg_resources/_vendor/packaging/requirements.py
+-rw-rw-rw-  2.0 fat    28025 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pkg_resources/_vendor/packaging/specifiers.py
+-rw-rw-rw-  2.0 fat      421 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pkg_resources/_vendor/packaging/utils.py
+-rw-rw-rw-  2.0 fat    11556 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pkg_resources/_vendor/packaging/version.py
+-rw-rw-rw-  2.0 fat     2487 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/pkg_resources/extern/__init__.py
+-rw-rw-rw-  2.0 fat     5700 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/setuptools/__init__.py
+-rw-rw-rw-  2.0 fat     6592 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/setuptools/archive_util.py
+-rw-rw-rw-  2.0 fat     5671 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/setuptools/build_meta.py
+-rw-rw-rw-  2.0 fat    16381 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/setuptools/config.py
+-rw-rw-rw-  2.0 fat      935 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/setuptools/dep_util.py
+-rw-rw-rw-  2.0 fat     5837 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/setuptools/depends.py
+-rw-rw-rw-  2.0 fat    42514 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/setuptools/dist.py
+-rw-rw-rw-  2.0 fat     1729 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/setuptools/extension.py
+-rw-rw-rw-  2.0 fat     3146 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/setuptools/glibc.py
+-rw-rw-rw-  2.0 fat     5207 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/setuptools/glob.py
+-rw-rw-rw-  2.0 fat      787 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/setuptools/launch.py
+-rw-rw-rw-  2.0 fat     2013 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/setuptools/lib2to3_ex.py
+-rw-rw-rw-  2.0 fat     5789 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/setuptools/monkey.py
+-rw-rw-rw-  2.0 fat    40877 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/setuptools/msvc.py
+-rw-rw-rw-  2.0 fat     3199 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/setuptools/namespaces.py
+-rw-rw-rw-  2.0 fat    40142 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/setuptools/package_index.py
+-rw-rw-rw-  2.0 fat    10882 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/setuptools/pep425tags.py
+-rw-rw-rw-  2.0 fat      536 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/setuptools/py27compat.py
+-rw-rw-rw-  2.0 fat     1192 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/setuptools/py31compat.py
+-rw-rw-rw-  2.0 fat     1182 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/setuptools/py33compat.py
+-rw-rw-rw-  2.0 fat     2891 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/setuptools/py36compat.py
+-rw-rw-rw-  2.0 fat    14276 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/setuptools/sandbox.py
+-rw-rw-rw-  2.0 fat     2307 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/setuptools/site-patch.py
+-rw-rw-rw-  2.0 fat     8492 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/setuptools/ssl_support.py
+-rw-rw-rw-  2.0 fat      996 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/setuptools/unicode_utils.py
+-rw-rw-rw-  2.0 fat      144 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/setuptools/version.py
+-rw-rw-rw-  2.0 fat     7230 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/setuptools/wheel.py
+-rw-rw-rw-  2.0 fat      714 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/setuptools/windows_support.py
+-rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/setuptools/_vendor/__init__.py
+-rw-rw-rw-  2.0 fat   229867 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/setuptools/_vendor/pyparsing.py
+-rw-rw-rw-  2.0 fat    30098 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/setuptools/_vendor/six.py
+-rw-rw-rw-  2.0 fat      720 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/setuptools/_vendor/packaging/__about__.py
+-rw-rw-rw-  2.0 fat      513 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/setuptools/_vendor/packaging/__init__.py
+-rw-rw-rw-  2.0 fat      860 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/setuptools/_vendor/packaging/_compat.py
+-rw-rw-rw-  2.0 fat     1416 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/setuptools/_vendor/packaging/_structures.py
+-rw-rw-rw-  2.0 fat     8239 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/setuptools/_vendor/packaging/markers.py
+-rw-rw-rw-  2.0 fat     4343 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/setuptools/_vendor/packaging/requirements.py
+-rw-rw-rw-  2.0 fat    28025 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/setuptools/_vendor/packaging/specifiers.py
+-rw-rw-rw-  2.0 fat      421 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/setuptools/_vendor/packaging/utils.py
+-rw-rw-rw-  2.0 fat    11556 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/setuptools/_vendor/packaging/version.py
+-rw-rw-rw-  2.0 fat      594 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/setuptools/command/__init__.py
+-rw-rw-rw-  2.0 fat     2426 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/setuptools/command/alias.py
+-rw-rw-rw-  2.0 fat    18185 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/setuptools/command/bdist_egg.py
+-rw-rw-rw-  2.0 fat     1508 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/setuptools/command/bdist_rpm.py
+-rw-rw-rw-  2.0 fat      637 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/setuptools/command/bdist_wininst.py
+-rw-rw-rw-  2.0 fat     4484 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/setuptools/command/build_clib.py
+-rw-rw-rw-  2.0 fat    13173 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/setuptools/command/build_ext.py
+-rw-rw-rw-  2.0 fat     9596 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/setuptools/command/build_py.py
+-rw-rw-rw-  2.0 fat     8046 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/setuptools/command/develop.py
+-rw-rw-rw-  2.0 fat      960 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/setuptools/command/dist_info.py
+-rw-rw-rw-  2.0 fat    87054 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/setuptools/command/easy_install.py
+-rw-rw-rw-  2.0 fat    24800 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/setuptools/command/egg_info.py
+-rw-rw-rw-  2.0 fat     4683 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/setuptools/command/install.py
+-rw-rw-rw-  2.0 fat     2203 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/setuptools/command/install_egg_info.py
+-rw-rw-rw-  2.0 fat     3840 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/setuptools/command/install_lib.py
+-rw-rw-rw-  2.0 fat     2439 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/setuptools/command/install_scripts.py
+-rw-rw-rw-  2.0 fat     4986 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/setuptools/command/py36compat.py
+-rw-rw-rw-  2.0 fat      270 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/setuptools/command/register.py
+-rw-rw-rw-  2.0 fat     2164 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/setuptools/command/rotate.py
+-rw-rw-rw-  2.0 fat      658 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/setuptools/command/saveopts.py
+-rw-rw-rw-  2.0 fat     6711 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/setuptools/command/sdist.py
+-rw-rw-rw-  2.0 fat     5085 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/setuptools/command/setopt.py
+-rw-rw-rw-  2.0 fat     9214 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/setuptools/command/test.py
+-rw-rw-rw-  2.0 fat     1172 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/setuptools/command/upload.py
+-rw-rw-rw-  2.0 fat     7311 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/setuptools/command/upload_docs.py
+-rw-rw-rw-  2.0 fat     2499 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/setuptools/extern/__init__.py
+-rw-rw-rw-  2.0 fat     1091 b- defN 23-Jun-03 04:11 p0_script-1.1.0.dist-info/LICENSE.rst
+-rw-rw-rw-  2.0 fat     8190 b- defN 23-Jun-03 04:11 p0_script-1.1.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-03 04:11 p0_script-1.1.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       43 b- defN 23-Jun-03 04:11 p0_script-1.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat    96277 b- defN 23-Jun-03 04:11 p0_script-1.1.0.dist-info/RECORD
+916 files, 5568108 bytes uncompressed, 1501196 bytes compressed:  73.0%
```

## zipnote {}

```diff
@@ -1,3202 +1,2749 @@
-Filename: p0-script-1.0.2/
+Filename: application/CommandBus.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/
+Filename: application/CommandBusHistory.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/
+Filename: application/Container.py
 Comment: 
 
-Filename: p0-script-1.0.2/infra/
+Filename: application/ContainerInterface.py
 Comment: 
 
-Filename: p0-script-1.0.2/p0_script.egg-info/
+Filename: application/Protocol0.py
 Comment: 
 
-Filename: p0-script-1.0.2/shared/
+Filename: application/Protocol0Midi.py
 Comment: 
 
-Filename: p0-script-1.0.2/tests/
+Filename: application/ScriptDisconnectedEvent.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/
+Filename: application/ScriptResetActivatedEvent.py
 Comment: 
 
-Filename: p0-script-1.0.2/LICENSE.rst
+Filename: application/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/PKG-INFO
+Filename: application/main.py
 Comment: 
 
-Filename: p0-script-1.0.2/pyproject.toml
+Filename: application/command/BounceTrackToAudioCommand.py
 Comment: 
 
-Filename: p0-script-1.0.2/README.md
+Filename: application/command/CheckAudioExportValidCommand.py
 Comment: 
 
-Filename: p0-script-1.0.2/setup.cfg
+Filename: application/command/DrumRackToSimplerCommand.py
 Comment: 
 
-Filename: p0-script-1.0.2/setup.py
+Filename: application/command/EmitBackendEventCommand.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/command/
+Filename: application/command/FireSceneToPositionCommand.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/command_handler/
+Filename: application/command/FireSelectedSceneCommand.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/control_surface/
+Filename: application/command/GetSetStateCommand.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/error/
+Filename: application/command/GoToGroupTrackCommand.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/push2/
+Filename: application/command/LoadDeviceCommand.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/CommandBus.py
+Filename: application/command/LoadDrumRackCommand.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/CommandBusHistory.py
+Filename: application/command/LoadMatchingTrackCommand.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/Container.py
+Filename: application/command/LoadMinitaurCommand.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/ContainerInterface.py
+Filename: application/command/LoadRev2Command.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/main.py
+Filename: application/command/MidiNoteCommand.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/Protocol0.py
+Filename: application/command/PlayPauseSongCommand.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/Protocol0Midi.py
+Filename: application/command/RecordUnlimitedCommand.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/ScriptDisconnectedEvent.py
+Filename: application/command/ReloadScriptCommand.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/ScriptResetActivatedEvent.py
+Filename: application/command/ResetPlaybackCommand.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/__init__.py
+Filename: application/command/ScrollScenePositionCommand.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/command/BounceTrackToAudioCommand.py
+Filename: application/command/ScrollSceneTracksCommand.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/command/CheckAudioExportValidCommand.py
+Filename: application/command/ScrollScenesCommand.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/command/DrumRackToSimplerCommand.py
+Filename: application/command/ScrollTrackVolumeCommand.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/command/EmitBackendEventCommand.py
+Filename: application/command/SelectOrLoadDeviceCommand.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/command/FireSceneToPositionCommand.py
+Filename: application/command/SelectTrackCommand.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/command/FireSelectedSceneCommand.py
+Filename: application/command/SerializableCommand.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/command/GetSetStateCommand.py
+Filename: application/command/ShowAutomationCommand.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/command/GoToGroupTrackCommand.py
+Filename: application/command/ShowInstrumentCommand.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/command/LoadDeviceCommand.py
+Filename: application/command/ShowMessageCommand.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/command/LoadDrumRackCommand.py
+Filename: application/command/ToggleArmCommand.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/command/LoadMatchingTrackCommand.py
+Filename: application/command/ToggleNotesCommand.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/command/LoadMinitaurCommand.py
+Filename: application/command/ToggleReferenceTrackCommand.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/command/LoadRev2Command.py
+Filename: application/command/ToggleSceneLoopCommand.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/command/MidiNoteCommand.py
+Filename: application/command/UnfoldSelectedSceneCommand.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/command/PlayPauseSongCommand.py
+Filename: application/command/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/command/RecordUnlimitedCommand.py
+Filename: application/command_handler/BounceTrackToAudioCommandHandler.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/command/ReloadScriptCommand.py
+Filename: application/command_handler/CheckAudioExportValidCommandHandler.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/command/ResetPlaybackCommand.py
+Filename: application/command_handler/CommandHandlerInterface.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/command/ScrollScenePositionCommand.py
+Filename: application/command_handler/DrumRackToSimplerCommandHandler.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/command/ScrollScenesCommand.py
+Filename: application/command_handler/EmitBackendEventCommandHandler.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/command/ScrollSceneTracksCommand.py
+Filename: application/command_handler/FireSceneToPositionCommandHandler.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/command/ScrollTrackVolumeCommand.py
+Filename: application/command_handler/FireSelectedSceneCommandHandler.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/command/SelectOrLoadDeviceCommand.py
+Filename: application/command_handler/GetSetStateCommandHandler.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/command/SelectTrackCommand.py
+Filename: application/command_handler/GoToGroupTrackCommandHandler.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/command/SerializableCommand.py
+Filename: application/command_handler/LoadDeviceCommandHandler.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/command/ShowAutomationCommand.py
+Filename: application/command_handler/LoadDrumRackCommandHandler.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/command/ShowInstrumentCommand.py
+Filename: application/command_handler/LoadMatchingTrackCommandHandler.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/command/ShowMessageCommand.py
+Filename: application/command_handler/LoadMinitaurCommandHandler.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/command/ToggleArmCommand.py
+Filename: application/command_handler/LoadRev2CommandHandler.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/command/ToggleNotesCommand.py
+Filename: application/command_handler/MidiNoteCommandHandler.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/command/ToggleReferenceTrackCommand.py
+Filename: application/command_handler/PlayPauseSongCommandHandler.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/command/ToggleSceneLoopCommand.py
+Filename: application/command_handler/RecordUnlimitedCommandHandler.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/command/UnfoldSelectedSceneCommand.py
+Filename: application/command_handler/ReloadScriptCommandHandler.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/command/__init__.py
+Filename: application/command_handler/ResetPlaybackCommandHandler.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/command_handler/BounceTrackToAudioCommandHandler.py
+Filename: application/command_handler/ScrollScenePositionCommandHandler.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/command_handler/CheckAudioExportValidCommandHandler.py
+Filename: application/command_handler/ScrollSceneTracksCommandHandler.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/command_handler/CommandHandlerInterface.py
+Filename: application/command_handler/ScrollScenesCommandHandler.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/command_handler/DrumRackToSimplerCommandHandler.py
+Filename: application/command_handler/ScrollTrackVolumeCommandHandler.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/command_handler/EmitBackendEventCommandHandler.py
+Filename: application/command_handler/SelectOrLoadDeviceCommandHandler.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/command_handler/FireSceneToPositionCommandHandler.py
+Filename: application/command_handler/SelectTrackCommandHandler.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/command_handler/FireSelectedSceneCommandHandler.py
+Filename: application/command_handler/ShowAutomationCommandHandler.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/command_handler/GetSetStateCommandHandler.py
+Filename: application/command_handler/ShowInstrumentCommandHandler.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/command_handler/GoToGroupTrackCommandHandler.py
+Filename: application/command_handler/ShowMessageCommandHandler.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/command_handler/LoadDeviceCommandHandler.py
+Filename: application/command_handler/ToggleArmCommandJHandler.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/command_handler/LoadDrumRackCommandHandler.py
+Filename: application/command_handler/ToggleNotesCommandHandler.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/command_handler/LoadMatchingTrackCommandHandler.py
+Filename: application/command_handler/ToggleReferenceTrackCommandHandler.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/command_handler/LoadMinitaurCommandHandler.py
+Filename: application/command_handler/ToggleSceneLoopCommandHandler.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/command_handler/LoadRev2CommandHandler.py
+Filename: application/command_handler/UnfoldSelectedSceneCommandHandler.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/command_handler/MidiNoteCommandHandler.py
+Filename: application/command_handler/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/command_handler/PlayPauseSongCommandHandler.py
+Filename: application/control_surface/ActionGroupFactory.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/command_handler/RecordUnlimitedCommandHandler.py
+Filename: application/control_surface/ActionGroupInterface.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/command_handler/ReloadScriptCommandHandler.py
+Filename: application/control_surface/EncoderAction.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/command_handler/ResetPlaybackCommandHandler.py
+Filename: application/control_surface/EncoderMoveEnum.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/command_handler/ScrollScenePositionCommandHandler.py
+Filename: application/control_surface/MultiEncoder.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/command_handler/ScrollScenesCommandHandler.py
+Filename: application/control_surface/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/command_handler/ScrollSceneTracksCommandHandler.py
+Filename: application/control_surface/group/ActionGroupClip.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/command_handler/ScrollTrackVolumeCommandHandler.py
+Filename: application/control_surface/group/ActionGroupCut.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/command_handler/SelectOrLoadDeviceCommandHandler.py
+Filename: application/control_surface/group/ActionGroupFix.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/command_handler/SelectTrackCommandHandler.py
+Filename: application/control_surface/group/ActionGroupLog.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/command_handler/ShowAutomationCommandHandler.py
+Filename: application/control_surface/group/ActionGroupMain.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/command_handler/ShowInstrumentCommandHandler.py
+Filename: application/control_surface/group/ActionGroupSample.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/command_handler/ShowMessageCommandHandler.py
+Filename: application/control_surface/group/ActionGroupSet.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/command_handler/ToggleArmCommandJHandler.py
+Filename: application/control_surface/group/ActionGroupTest.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/command_handler/ToggleNotesCommandHandler.py
+Filename: application/control_surface/group/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/command_handler/ToggleReferenceTrackCommandHandler.py
+Filename: application/control_surface/group/legacy/ActionGroupPreset.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/command_handler/ToggleSceneLoopCommandHandler.py
+Filename: application/control_surface/group/legacy/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/command_handler/UnfoldSelectedSceneCommandHandler.py
+Filename: application/error/ErrorService.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/command_handler/__init__.py
+Filename: application/error/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/control_surface/group/
+Filename: application/push2/P0Push2.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/control_surface/ActionGroupFactory.py
+Filename: application/push2/P0SessionRingTrackProvider.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/control_surface/ActionGroupInterface.py
+Filename: application/push2/P0ShowInstrumentMode.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/control_surface/EncoderAction.py
+Filename: application/push2/P0TrackListComponent.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/control_surface/EncoderMoveEnum.py
+Filename: application/push2/P0TransportComponent.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/control_surface/MultiEncoder.py
+Filename: application/push2/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/control_surface/__init__.py
+Filename: domain/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/control_surface/group/legacy/
+Filename: domain/audit/AudioLatencyAnalyzerService.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/control_surface/group/ActionGroupClip.py
+Filename: domain/audit/LOMAnalyzerService.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/control_surface/group/ActionGroupCut.py
+Filename: domain/audit/LogService.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/control_surface/group/ActionGroupFix.py
+Filename: domain/audit/SetFixerService.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/control_surface/group/ActionGroupLog.py
+Filename: domain/audit/SetUpgradeService.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/control_surface/group/ActionGroupMain.py
+Filename: domain/audit/SongStatsService.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/control_surface/group/ActionGroupSample.py
+Filename: domain/audit/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/control_surface/group/ActionGroupSet.py
+Filename: domain/audit/utils.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/control_surface/group/ActionGroupTest.py
+Filename: domain/audit/stats/ClipStats.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/control_surface/group/__init__.py
+Filename: domain/audit/stats/DeviceStats.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/control_surface/group/legacy/ActionGroupPreset.py
+Filename: domain/audit/stats/SampleStats.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/control_surface/group/legacy/__init__.py
+Filename: domain/audit/stats/SceneStats.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/error/ErrorService.py
+Filename: domain/audit/stats/SongStats.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/error/__init__.py
+Filename: domain/audit/stats/Stats.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/push2/P0Push2.py
+Filename: domain/audit/stats/TrackStats.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/push2/P0SessionRingTrackProvider.py
+Filename: domain/audit/stats/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/push2/P0ShowInstrumentMode.py
+Filename: domain/lom/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/push2/P0TrackListComponent.py
+Filename: domain/lom/clip/AudioClip.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/push2/P0TransportComponent.py
+Filename: domain/lom/clip/Clip.py
 Comment: 
 
-Filename: p0-script-1.0.2/application/push2/__init__.py
+Filename: domain/lom/clip/ClipAppearance.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/audit/
+Filename: domain/lom/clip/ClipColorEnum.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/
+Filename: domain/lom/clip/ClipConfig.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/shared/
+Filename: domain/lom/clip/ClipCreatedOrDeletedEvent.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/track_recorder/
+Filename: domain/lom/clip/ClipEnvelopeShowedEvent.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/__init__.py
+Filename: domain/lom/clip/ClipInfo.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/audit/stats/
+Filename: domain/lom/clip/ClipLoop.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/audit/AudioLatencyAnalyzerService.py
+Filename: domain/lom/clip/ClipName.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/audit/LogService.py
+Filename: domain/lom/clip/ClipPlayingPosition.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/audit/LOMAnalyzerService.py
+Filename: domain/lom/clip/ClipSlotSelectedEvent.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/audit/SetFixerService.py
+Filename: domain/lom/clip/ClipTail.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/audit/SetUpgradeService.py
+Filename: domain/lom/clip/MidiClip.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/audit/SongStatsService.py
+Filename: domain/lom/clip/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/audit/utils.py
+Filename: domain/lom/clip/automation/ClipAutomation.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/audit/__init__.py
+Filename: domain/lom/clip/automation/ClipAutomationEnvelope.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/audit/stats/ClipStats.py
+Filename: domain/lom/clip/automation/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/audit/stats/DeviceStats.py
+Filename: domain/lom/clip_slot/AudioClipSlot.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/audit/stats/SampleStats.py
+Filename: domain/lom/clip_slot/ClipSlot.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/audit/stats/SceneStats.py
+Filename: domain/lom/clip_slot/ClipSlotAppearance.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/audit/stats/SongStats.py
+Filename: domain/lom/clip_slot/ClipSlotHasClipEvent.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/audit/stats/Stats.py
+Filename: domain/lom/clip_slot/MidiClipSlot.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/audit/stats/TrackStats.py
+Filename: domain/lom/clip_slot/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/audit/stats/__init__.py
+Filename: domain/lom/device/Device.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/clip/
+Filename: domain/lom/device/DeviceChain.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/clip_slot/
+Filename: domain/lom/device/DeviceDisplayService.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/device/
+Filename: domain/lom/device/DeviceEnum.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/device_parameter/
+Filename: domain/lom/device/DeviceEnumGroup.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/instrument/
+Filename: domain/lom/device/DeviceLoadedEvent.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/loop/
+Filename: domain/lom/device/DeviceService.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/note/
+Filename: domain/lom/device/DrumPad.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/sample/
+Filename: domain/lom/device/DrumRackDevice.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/scene/
+Filename: domain/lom/device/DrumRackLoadedEvent.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/set/
+Filename: domain/lom/device/DrumRackSampleService.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/song/
+Filename: domain/lom/device/DrumRackService.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/
+Filename: domain/lom/device/MixerDevice.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/validation/
+Filename: domain/lom/device/PluginDevice.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/__init__.py
+Filename: domain/lom/device/RackDevice.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/clip/automation/
+Filename: domain/lom/device/SimpleTrackDevices.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/clip/AudioClip.py
+Filename: domain/lom/device/SimplerDevice.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/clip/Clip.py
+Filename: domain/lom/device/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/clip/ClipAppearance.py
+Filename: domain/lom/device/Sample/Sample.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/clip/ClipColorEnum.py
+Filename: domain/lom/device/Sample/SampleNotFoundError.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/clip/ClipConfig.py
+Filename: domain/lom/device/Sample/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/clip/ClipCreatedOrDeletedEvent.py
+Filename: domain/lom/device_parameter/DeviceParameter.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/clip/ClipEnvelopeShowedEvent.py
+Filename: domain/lom/device_parameter/DeviceParameterEnum.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/clip/ClipInfo.py
+Filename: domain/lom/device_parameter/DeviceParameterValue.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/clip/ClipLoop.py
+Filename: domain/lom/device_parameter/LinkedDeviceParameters.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/clip/ClipName.py
+Filename: domain/lom/device_parameter/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/clip/ClipPlayingPosition.py
+Filename: domain/lom/instrument/InstrumentActivatedEvent.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/clip/ClipSlotSelectedEvent.py
+Filename: domain/lom/instrument/InstrumentColorEnum.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/clip/ClipTail.py
+Filename: domain/lom/instrument/InstrumentDisplayService.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/clip/MidiClip.py
+Filename: domain/lom/instrument/InstrumentFactory.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/clip/__init__.py
+Filename: domain/lom/instrument/InstrumentInterface.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/clip/automation/ClipAutomation.py
+Filename: domain/lom/instrument/InstrumentSelectedEvent.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/clip/automation/ClipAutomationEnvelope.py
+Filename: domain/lom/instrument/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/clip/automation/__init__.py
+Filename: domain/lom/instrument/instrument/InstrumentAddictiveKeys.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/clip_slot/AudioClipSlot.py
+Filename: domain/lom/instrument/instrument/InstrumentDrumRack.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/clip_slot/ClipSlot.py
+Filename: domain/lom/instrument/instrument/InstrumentKontakt.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/clip_slot/ClipSlotAppearance.py
+Filename: domain/lom/instrument/instrument/InstrumentMinitaur.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/clip_slot/ClipSlotHasClipEvent.py
+Filename: domain/lom/instrument/instrument/InstrumentOpus.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/clip_slot/MidiClipSlot.py
+Filename: domain/lom/instrument/instrument/InstrumentPlay.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/clip_slot/__init__.py
+Filename: domain/lom/instrument/instrument/InstrumentRev2.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/device/Sample/
+Filename: domain/lom/instrument/instrument/InstrumentSampler.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/device/Device.py
+Filename: domain/lom/instrument/instrument/InstrumentSerum.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/device/DeviceChain.py
+Filename: domain/lom/instrument/instrument/InstrumentSimpler.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/device/DeviceDisplayService.py
+Filename: domain/lom/instrument/instrument/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/device/DeviceEnum.py
+Filename: domain/lom/instrument/preset/InstrumentPreset.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/device/DeviceEnumGroup.py
+Filename: domain/lom/instrument/preset/InstrumentPresetList.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/device/DeviceLoadedEvent.py
+Filename: domain/lom/instrument/preset/InstrumentPresetScrollerService.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/device/DeviceService.py
+Filename: domain/lom/instrument/preset/PresetDisplayOptionEnum.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/device/DrumPad.py
+Filename: domain/lom/instrument/preset/PresetProgramSelectedEvent.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/device/DrumRackDevice.py
+Filename: domain/lom/instrument/preset/SampleSelectedEvent.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/device/DrumRackLoadedEvent.py
+Filename: domain/lom/instrument/preset/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/device/DrumRackSampleService.py
+Filename: domain/lom/instrument/preset/preset_changer/InstrumentRackPresetChanger.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/device/DrumRackService.py
+Filename: domain/lom/instrument/preset/preset_changer/PresetChangerInterface.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/device/MixerDevice.py
+Filename: domain/lom/instrument/preset/preset_changer/ProgramChangePresetChanger.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/device/PluginDevice.py
+Filename: domain/lom/instrument/preset/preset_changer/SamplePresetChanger.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/device/RackDevice.py
+Filename: domain/lom/instrument/preset/preset_changer/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/device/SimplerDevice.py
+Filename: domain/lom/instrument/preset/preset_importer/DirectoryPresetImporter.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/device/SimpleTrackDevices.py
+Filename: domain/lom/instrument/preset/preset_importer/FilePresetImporter.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/device/__init__.py
+Filename: domain/lom/instrument/preset/preset_importer/NullPresetImporter.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/device/Sample/Sample.py
+Filename: domain/lom/instrument/preset/preset_importer/PluginDevicePresetImporter.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/device/Sample/SampleNotFoundError.py
+Filename: domain/lom/instrument/preset/preset_importer/PresetImportInterface.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/device/Sample/__init__.py
+Filename: domain/lom/instrument/preset/preset_importer/PresetImporterFactory.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/device_parameter/DeviceParameter.py
+Filename: domain/lom/instrument/preset/preset_importer/RackDevicePresetImporter.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/device_parameter/DeviceParameterEnum.py
+Filename: domain/lom/instrument/preset/preset_importer/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/device_parameter/DeviceParameterValue.py
+Filename: domain/lom/instrument/preset/preset_initializer/PresetInitializerDevicePresetName.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/device_parameter/LinkedDeviceParameters.py
+Filename: domain/lom/instrument/preset/preset_initializer/PresetInitializerGroupTrackName.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/device_parameter/__init__.py
+Filename: domain/lom/instrument/preset/preset_initializer/PresetInitializerInterface.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/instrument/instrument/
+Filename: domain/lom/instrument/preset/preset_initializer/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/instrument/preset/
+Filename: domain/lom/loop/LoopableInterface.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/instrument/InstrumentActivatedEvent.py
+Filename: domain/lom/loop/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/instrument/InstrumentColorEnum.py
+Filename: domain/lom/note/Note.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/instrument/InstrumentDisplayService.py
+Filename: domain/lom/note/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/instrument/InstrumentFactory.py
+Filename: domain/lom/sample/SampleCategory.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/instrument/InstrumentInterface.py
+Filename: domain/lom/sample/SampleCategoryEnum.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/instrument/InstrumentSelectedEvent.py
+Filename: domain/lom/sample/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/instrument/__init__.py
+Filename: domain/lom/scene/LoopingSceneToggler.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/instrument/instrument/InstrumentAddictiveKeys.py
+Filename: domain/lom/scene/NextSceneStartedEvent.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/instrument/instrument/InstrumentDrumRack.py
+Filename: domain/lom/scene/PlayingSceneChangedEvent.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/instrument/instrument/InstrumentKontakt.py
+Filename: domain/lom/scene/PlayingSceneFacade.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/instrument/instrument/InstrumentMinitaur.py
+Filename: domain/lom/scene/Scene.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/instrument/instrument/InstrumentOpus.py
+Filename: domain/lom/scene/SceneAppearance.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/instrument/instrument/InstrumentPlay.py
+Filename: domain/lom/scene/SceneClips.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/instrument/instrument/InstrumentRev2.py
+Filename: domain/lom/scene/SceneCropScroller.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/instrument/instrument/InstrumentSampler.py
+Filename: domain/lom/scene/SceneFiredEvent.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/instrument/instrument/InstrumentSerum.py
+Filename: domain/lom/scene/SceneLastBarPassedEvent.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/instrument/instrument/InstrumentSimpler.py
+Filename: domain/lom/scene/SceneLength.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/instrument/instrument/__init__.py
+Filename: domain/lom/scene/SceneName.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/instrument/preset/preset_changer/
+Filename: domain/lom/scene/ScenePlaybackService.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/instrument/preset/preset_importer/
+Filename: domain/lom/scene/ScenePlayingState.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/instrument/preset/preset_initializer/
+Filename: domain/lom/scene/ScenePositionScrolledEvent.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/instrument/preset/InstrumentPreset.py
+Filename: domain/lom/scene/ScenePositionScroller.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/instrument/preset/InstrumentPresetList.py
+Filename: domain/lom/scene/SceneService.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/instrument/preset/InstrumentPresetScrollerService.py
+Filename: domain/lom/scene/SceneWindow.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/instrument/preset/PresetDisplayOptionEnum.py
+Filename: domain/lom/scene/ScenesMappedEvent.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/instrument/preset/PresetProgramSelectedEvent.py
+Filename: domain/lom/scene/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/instrument/preset/SampleSelectedEvent.py
+Filename: domain/lom/set/AbletonSet.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/instrument/preset/__init__.py
+Filename: domain/lom/set/AbletonSetChangedEvent.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/instrument/preset/preset_changer/InstrumentRackPresetChanger.py
+Filename: domain/lom/set/MixingService.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/instrument/preset/preset_changer/PresetChangerInterface.py
+Filename: domain/lom/set/SessionToArrangementService.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/instrument/preset/preset_changer/ProgramChangePresetChanger.py
+Filename: domain/lom/set/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/instrument/preset/preset_changer/SamplePresetChanger.py
+Filename: domain/lom/song/SongInitService.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/instrument/preset/preset_changer/__init__.py
+Filename: domain/lom/song/SongInitializedEvent.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/instrument/preset/preset_importer/DirectoryPresetImporter.py
+Filename: domain/lom/song/SongStartedEvent.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/instrument/preset/preset_importer/FilePresetImporter.py
+Filename: domain/lom/song/SongStoppedEvent.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/instrument/preset/preset_importer/NullPresetImporter.py
+Filename: domain/lom/song/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/instrument/preset/preset_importer/PluginDevicePresetImporter.py
+Filename: domain/lom/song/components/ClipComponent.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/instrument/preset/preset_importer/PresetImporterFactory.py
+Filename: domain/lom/song/components/DeviceComponent.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/instrument/preset/preset_importer/PresetImportInterface.py
+Filename: domain/lom/song/components/PlaybackComponent.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/instrument/preset/preset_importer/RackDevicePresetImporter.py
+Filename: domain/lom/song/components/QuantizationComponent.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/instrument/preset/preset_importer/__init__.py
+Filename: domain/lom/song/components/RecordingComponent.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/instrument/preset/preset_initializer/PresetInitializerDevicePresetName.py
+Filename: domain/lom/song/components/SceneComponent.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/instrument/preset/preset_initializer/PresetInitializerGroupTrackName.py
+Filename: domain/lom/song/components/SceneCrudComponent.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/instrument/preset/preset_initializer/PresetInitializerInterface.py
+Filename: domain/lom/song/components/TempoComponent.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/instrument/preset/preset_initializer/__init__.py
+Filename: domain/lom/song/components/TrackComponent.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/loop/LoopableInterface.py
+Filename: domain/lom/song/components/TrackCrudComponent.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/loop/__init__.py
+Filename: domain/lom/song/components/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/note/Note.py
+Filename: domain/lom/track/CurrentMonitoringStateEnum.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/note/__init__.py
+Filename: domain/lom/track/P0TrackInterface.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/sample/SampleCategory.py
+Filename: domain/lom/track/SelectedTrackChangedEvent.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/sample/SampleCategoryEnum.py
+Filename: domain/lom/track/TrackAddedEvent.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/sample/__init__.py
+Filename: domain/lom/track/TrackAutomationService.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/scene/LoopingSceneToggler.py
+Filename: domain/lom/track/TrackColorEnum.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/scene/NextSceneStartedEvent.py
+Filename: domain/lom/track/TrackDisconnectedEvent.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/scene/PlayingSceneChangedEvent.py
+Filename: domain/lom/track/TrackFactory.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/scene/PlayingSceneFacade.py
+Filename: domain/lom/track/TrackMapperService.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/scene/Scene.py
+Filename: domain/lom/track/TrackService.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/scene/SceneAppearance.py
+Filename: domain/lom/track/TracksMappedEvent.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/scene/SceneClips.py
+Filename: domain/lom/track/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/scene/SceneCropScroller.py
+Filename: domain/lom/track/abstract_track/AbstrackTrackArmState.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/scene/SceneFiredEvent.py
+Filename: domain/lom/track/abstract_track/AbstractTrack.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/scene/SceneLastBarPassedEvent.py
+Filename: domain/lom/track/abstract_track/AbstractTrackAppearance.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/scene/SceneLength.py
+Filename: domain/lom/track/abstract_track/AbstractTrackNameUpdatedEvent.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/scene/SceneName.py
+Filename: domain/lom/track/abstract_track/AbstractTrackSelectedEvent.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/scene/ScenePlaybackService.py
+Filename: domain/lom/track/abstract_track/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/scene/ScenePlayingState.py
+Filename: domain/lom/track/group_track/AbstractGroupTrack.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/scene/ScenePositionScrolledEvent.py
+Filename: domain/lom/track/group_track/DrumsTrack.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/scene/ScenePositionScroller.py
+Filename: domain/lom/track/group_track/NormalGroupMatchingTrack.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/scene/SceneService.py
+Filename: domain/lom/track/group_track/NormalGroupMatchingTrackCreator.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/scene/ScenesMappedEvent.py
+Filename: domain/lom/track/group_track/NormalGroupTrack.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/scene/SceneWindow.py
+Filename: domain/lom/track/group_track/VocalsTrack.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/scene/__init__.py
+Filename: domain/lom/track/group_track/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/set/AbletonSet.py
+Filename: domain/lom/track/group_track/ext_track/ExtArmState.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/set/AbletonSetChangedEvent.py
+Filename: domain/lom/track/group_track/ext_track/ExtArmedEvent.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/set/MixingService.py
+Filename: domain/lom/track/group_track/ext_track/ExtMatchingTrack.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/set/SessionToArrangementService.py
+Filename: domain/lom/track/group_track/ext_track/ExtMatchingTrackCreator.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/set/__init__.py
+Filename: domain/lom/track/group_track/ext_track/ExtMonitoringState.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/song/components/
+Filename: domain/lom/track/group_track/ext_track/ExtSoloState.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/song/SongInitializedEvent.py
+Filename: domain/lom/track/group_track/ext_track/ExternalSynthTrack.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/song/SongInitService.py
+Filename: domain/lom/track/group_track/ext_track/SimpleAudioExtTrack.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/song/SongStartedEvent.py
+Filename: domain/lom/track/group_track/ext_track/SimpleBaseExtTrack.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/song/SongStoppedEvent.py
+Filename: domain/lom/track/group_track/ext_track/SimpleMidiExtTrack.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/song/__init__.py
+Filename: domain/lom/track/group_track/ext_track/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/song/components/ClipComponent.py
+Filename: domain/lom/track/group_track/matching_track/MatchingTrackClipColorManager.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/song/components/DeviceComponent.py
+Filename: domain/lom/track/group_track/matching_track/MatchingTrackClipManager.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/song/components/PlaybackComponent.py
+Filename: domain/lom/track/group_track/matching_track/MatchingTrackCreatorInterface.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/song/components/QuantizationComponent.py
+Filename: domain/lom/track/group_track/matching_track/MatchingTrackInterface.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/song/components/RecordingComponent.py
+Filename: domain/lom/track/group_track/matching_track/MatchingTrackRouter.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/song/components/SceneComponent.py
+Filename: domain/lom/track/group_track/matching_track/MatchingTrackService.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/song/components/SceneCrudComponent.py
+Filename: domain/lom/track/group_track/matching_track/MatchingTrackSoloState.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/song/components/TempoComponent.py
+Filename: domain/lom/track/group_track/matching_track/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/song/components/TrackComponent.py
+Filename: domain/lom/track/group_track/matching_track/utils.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/song/components/TrackCrudComponent.py
+Filename: domain/lom/track/routing/InputRoutingChannelEnum.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/song/components/__init__.py
+Filename: domain/lom/track/routing/InputRoutingTypeEnum.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/abstract_track/
+Filename: domain/lom/track/routing/OutputRoutingTypeEnum.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/group_track/
+Filename: domain/lom/track/routing/RoutingDisplayNameDescriptor.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/routing/
+Filename: domain/lom/track/routing/RoutingTrackDescriptor.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/simple_track/
+Filename: domain/lom/track/routing/TrackInputRouting.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/CurrentMonitoringStateEnum.py
+Filename: domain/lom/track/routing/TrackOutputRouting.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/P0TrackInterface.py
+Filename: domain/lom/track/routing/TrackRoutingInterface.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/SelectedTrackChangedEvent.py
+Filename: domain/lom/track/routing/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/TrackAddedEvent.py
+Filename: domain/lom/track/simple_track/AudioToMidiClipMapping.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/TrackAutomationService.py
+Filename: domain/lom/track/simple_track/SimpleMatchingTrack.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/TrackColorEnum.py
+Filename: domain/lom/track/simple_track/SimpleMatchingTrackCreator.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/TrackDisconnectedEvent.py
+Filename: domain/lom/track/simple_track/SimpleTrack.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/TrackFactory.py
+Filename: domain/lom/track/simple_track/SimpleTrackArmState.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/TrackMapperService.py
+Filename: domain/lom/track/simple_track/SimpleTrackArmedEvent.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/TrackService.py
+Filename: domain/lom/track/simple_track/SimpleTrackClipColorManager.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/TracksMappedEvent.py
+Filename: domain/lom/track/simple_track/SimpleTrackClipSlots.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/__init__.py
+Filename: domain/lom/track/simple_track/SimpleTrackClips.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/abstract_track/AbstrackTrackArmState.py
+Filename: domain/lom/track/simple_track/SimpleTrackCreatedEvent.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/abstract_track/AbstractTrack.py
+Filename: domain/lom/track/simple_track/SimpleTrackDeletedEvent.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/abstract_track/AbstractTrackAppearance.py
+Filename: domain/lom/track/simple_track/SimpleTrackFlattenedEvent.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/abstract_track/AbstractTrackNameUpdatedEvent.py
+Filename: domain/lom/track/simple_track/SimpleTrackMonitoringState.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/abstract_track/AbstractTrackSelectedEvent.py
+Filename: domain/lom/track/simple_track/SimpleTrackSaveStartedEvent.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/abstract_track/__init__.py
+Filename: domain/lom/track/simple_track/SimpleTrackService.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/group_track/ext_track/
+Filename: domain/lom/track/simple_track/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/group_track/matching_track/
+Filename: domain/lom/track/simple_track/audio/SimpleAudioTrack.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/group_track/AbstractGroupTrack.py
+Filename: domain/lom/track/simple_track/audio/SimpleReturnTrack.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/group_track/DrumsTrack.py
+Filename: domain/lom/track/simple_track/audio/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/group_track/NormalGroupMatchingTrack.py
+Filename: domain/lom/track/simple_track/audio/master/MasterTrack.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/group_track/NormalGroupMatchingTrackCreator.py
+Filename: domain/lom/track/simple_track/audio/master/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/group_track/NormalGroupTrack.py
+Filename: domain/lom/track/simple_track/audio/special/ReferenceTrack.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/group_track/VocalsTrack.py
+Filename: domain/lom/track/simple_track/audio/special/ResamplingTrack.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/group_track/__init__.py
+Filename: domain/lom/track/simple_track/audio/special/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/group_track/ext_track/ExtArmedEvent.py
+Filename: domain/lom/track/simple_track/midi/SimpleMidiTrack.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/group_track/ext_track/ExtArmState.py
+Filename: domain/lom/track/simple_track/midi/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/group_track/ext_track/ExternalSynthTrack.py
+Filename: domain/lom/track/simple_track/midi/special/UsamoTrack.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/group_track/ext_track/ExtMatchingTrack.py
+Filename: domain/lom/track/simple_track/midi/special/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/group_track/ext_track/ExtMatchingTrackCreator.py
+Filename: domain/lom/validation/ValidatorFactory.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/group_track/ext_track/ExtMonitoringState.py
+Filename: domain/lom/validation/ValidatorInterface.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/group_track/ext_track/ExtSoloState.py
+Filename: domain/lom/validation/ValidatorService.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/group_track/ext_track/SimpleAudioExtTrack.py
+Filename: domain/lom/validation/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/group_track/ext_track/SimpleBaseExtTrack.py
+Filename: domain/lom/validation/object_validators/AbstractGroupTrackValidator.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/group_track/ext_track/SimpleMidiExtTrack.py
+Filename: domain/lom/validation/object_validators/SceneValidator.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/group_track/ext_track/__init__.py
+Filename: domain/lom/validation/object_validators/SimpleAudioTrackValidator.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/group_track/matching_track/MatchingTrackClipColorManager.py
+Filename: domain/lom/validation/object_validators/SimpleTrackValidator.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/group_track/matching_track/MatchingTrackClipManager.py
+Filename: domain/lom/validation/object_validators/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/group_track/matching_track/MatchingTrackCreatorInterface.py
+Filename: domain/lom/validation/object_validators/external_synth_track/ExternalSynthTrackValidator.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/group_track/matching_track/MatchingTrackInterface.py
+Filename: domain/lom/validation/object_validators/external_synth_track/SimpleAudioExtTrackValidator.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/group_track/matching_track/MatchingTrackRouter.py
+Filename: domain/lom/validation/object_validators/external_synth_track/SimpleMidiExtTrackValidator.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/group_track/matching_track/MatchingTrackService.py
+Filename: domain/lom/validation/object_validators/external_synth_track/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/group_track/matching_track/MatchingTrackSoloState.py
+Filename: domain/lom/validation/sub_validators/AggregateValidator.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/group_track/matching_track/utils.py
+Filename: domain/lom/validation/sub_validators/CallbackValidator.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/group_track/matching_track/__init__.py
+Filename: domain/lom/validation/sub_validators/DeviceParameterValidator.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/routing/InputRoutingChannelEnum.py
+Filename: domain/lom/validation/sub_validators/PropertyValueValidator.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/routing/InputRoutingTypeEnum.py
+Filename: domain/lom/validation/sub_validators/SimpleTrackHasDeviceValidator.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/routing/OutputRoutingTypeEnum.py
+Filename: domain/lom/validation/sub_validators/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/routing/RoutingDisplayNameDescriptor.py
+Filename: domain/shared/ApplicationView.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/routing/RoutingTrackDescriptor.py
+Filename: domain/shared/BrowserServiceInterface.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/routing/TrackInputRouting.py
+Filename: domain/shared/InterfaceClicksServiceInterface.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/routing/TrackOutputRouting.py
+Filename: domain/shared/LiveObject.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/routing/TrackRoutingInterface.py
+Filename: domain/shared/LiveObjectMapping.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/routing/__init__.py
+Filename: domain/shared/SessionServiceInterface.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/simple_track/audio/
+Filename: domain/shared/ValueScroller.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/simple_track/midi/
+Filename: domain/shared/ValueToggler.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/simple_track/AudioToMidiClipMapping.py
+Filename: domain/shared/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/simple_track/SimpleMatchingTrack.py
+Filename: domain/shared/backend/Backend.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/simple_track/SimpleMatchingTrackCreator.py
+Filename: domain/shared/backend/BackendEvent.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/simple_track/SimpleTrack.py
+Filename: domain/shared/backend/NotificationColorEnum.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/simple_track/SimpleTrackArmedEvent.py
+Filename: domain/shared/backend/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/simple_track/SimpleTrackArmState.py
+Filename: domain/shared/errors/ErrorRaisedEvent.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/simple_track/SimpleTrackClipColorManager.py
+Filename: domain/shared/errors/Protocol0Error.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/simple_track/SimpleTrackClips.py
+Filename: domain/shared/errors/Protocol0Warning.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/simple_track/SimpleTrackClipSlots.py
+Filename: domain/shared/errors/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/simple_track/SimpleTrackCreatedEvent.py
+Filename: domain/shared/errors/error_handler.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/simple_track/SimpleTrackDeletedEvent.py
+Filename: domain/shared/event/DomainEventBus.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/simple_track/SimpleTrackFlattenedEvent.py
+Filename: domain/shared/event/HasEmitter.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/simple_track/SimpleTrackMonitoringState.py
+Filename: domain/shared/event/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/simple_track/SimpleTrackSaveStartedEvent.py
+Filename: domain/shared/scheduler/BarChangedEvent.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/simple_track/SimpleTrackService.py
+Filename: domain/shared/scheduler/BarEndingEvent.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/simple_track/__init__.py
+Filename: domain/shared/scheduler/BeatSchedulerInterface.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/simple_track/audio/master/
+Filename: domain/shared/scheduler/Last16thPassedEvent.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/simple_track/audio/special/
+Filename: domain/shared/scheduler/Last32thPassedEvent.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/simple_track/audio/SimpleAudioTrack.py
+Filename: domain/shared/scheduler/Last8thPassedEvent.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/simple_track/audio/SimpleReturnTrack.py
+Filename: domain/shared/scheduler/LastBeatPassedEvent.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/simple_track/audio/__init__.py
+Filename: domain/shared/scheduler/Scheduler.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/simple_track/audio/master/MasterTrack.py
+Filename: domain/shared/scheduler/ThirdBeatPassedEvent.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/simple_track/audio/master/__init__.py
+Filename: domain/shared/scheduler/TickSchedulerEventInterface.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/simple_track/audio/special/ReferenceTrack.py
+Filename: domain/shared/scheduler/TickSchedulerInterface.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/simple_track/audio/special/ResamplingTrack.py
+Filename: domain/shared/scheduler/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/simple_track/audio/special/__init__.py
+Filename: domain/shared/script/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/simple_track/midi/special/
+Filename: domain/shared/ui/ColorEnum.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/simple_track/midi/SimpleMidiTrack.py
+Filename: domain/shared/ui/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/simple_track/midi/__init__.py
+Filename: domain/shared/utils/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/simple_track/midi/special/UsamoTrack.py
+Filename: domain/shared/utils/concurrency.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/track/simple_track/midi/special/__init__.py
+Filename: domain/shared/utils/debug.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/validation/object_validators/
+Filename: domain/shared/utils/forward_to.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/validation/sub_validators/
+Filename: domain/shared/utils/func.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/validation/ValidatorFactory.py
+Filename: domain/shared/utils/list.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/validation/ValidatorInterface.py
+Filename: domain/shared/utils/string.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/validation/ValidatorService.py
+Filename: domain/shared/utils/timing.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/validation/__init__.py
+Filename: domain/shared/utils/utils.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/validation/object_validators/external_synth_track/
+Filename: domain/track_recorder/AbstractRecorderFactory.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/validation/object_validators/AbstractGroupTrackValidator.py
+Filename: domain/track_recorder/BaseRecorder.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/validation/object_validators/SceneValidator.py
+Filename: domain/track_recorder/RecordProcessorInterface.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/validation/object_validators/SimpleAudioTrackValidator.py
+Filename: domain/track_recorder/RecordService.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/validation/object_validators/SimpleTrackValidator.py
+Filename: domain/track_recorder/RecordTypeEnum.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/validation/object_validators/__init__.py
+Filename: domain/track_recorder/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/validation/object_validators/external_synth_track/ExternalSynthTrackValidator.py
+Filename: domain/track_recorder/config/RecordConfig.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/validation/object_validators/external_synth_track/SimpleAudioExtTrackValidator.py
+Filename: domain/track_recorder/config/RecordProcessors.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/validation/object_validators/external_synth_track/SimpleMidiExtTrackValidator.py
+Filename: domain/track_recorder/config/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/validation/object_validators/external_synth_track/__init__.py
+Filename: domain/track_recorder/count_in/CountInInterface.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/validation/sub_validators/AggregateValidator.py
+Filename: domain/track_recorder/count_in/CountInOneBar.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/validation/sub_validators/CallbackValidator.py
+Filename: domain/track_recorder/count_in/CountInShort.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/validation/sub_validators/DeviceParameterValidator.py
+Filename: domain/track_recorder/count_in/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/validation/sub_validators/PropertyValueValidator.py
+Filename: domain/track_recorder/event/RecordCancelledEvent.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/validation/sub_validators/SimpleTrackHasDeviceValidator.py
+Filename: domain/track_recorder/event/RecordEndedEvent.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/lom/validation/sub_validators/__init__.py
+Filename: domain/track_recorder/event/RecordStartedEvent.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/shared/backend/
+Filename: domain/track_recorder/event/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/shared/errors/
+Filename: domain/track_recorder/external_synth/AudioClipSilentEvent.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/shared/event/
+Filename: domain/track_recorder/external_synth/ExtAudioRecordingEndedEvent.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/shared/scheduler/
+Filename: domain/track_recorder/external_synth/ExtAudioRecordingStartedEvent.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/shared/script/
+Filename: domain/track_recorder/external_synth/OnRecordEndClipTail.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/shared/ui/
+Filename: domain/track_recorder/external_synth/TrackRecorderExternalSynthFactory.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/shared/utils/
+Filename: domain/track_recorder/external_synth/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/shared/ApplicationView.py
+Filename: domain/track_recorder/external_synth/record_audio/PostRecordAudio.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/shared/BrowserServiceInterface.py
+Filename: domain/track_recorder/external_synth/record_audio/PostRecordAudioFull.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/shared/InterfaceClicksServiceInterface.py
+Filename: domain/track_recorder/external_synth/record_audio/PreRecordAudio.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/shared/LiveObject.py
+Filename: domain/track_recorder/external_synth/record_audio/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/shared/LiveObjectMapping.py
+Filename: domain/track_recorder/external_synth/record_audio/record_multi/PreRecordAudioMulti.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/shared/SessionServiceInterface.py
+Filename: domain/track_recorder/external_synth/record_audio/record_multi/RecordAudioMulti.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/shared/ValueScroller.py
+Filename: domain/track_recorder/external_synth/record_audio/record_multi/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/shared/ValueToggler.py
+Filename: domain/track_recorder/external_synth/record_midi/PostRecordMidi.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/shared/__init__.py
+Filename: domain/track_recorder/external_synth/record_midi/PreRecordMidi.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/shared/backend/Backend.py
+Filename: domain/track_recorder/external_synth/record_midi/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/shared/backend/BackendEvent.py
+Filename: domain/track_recorder/recording_bar_length/RecordingBarLengthEnum.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/shared/backend/NotificationColorEnum.py
+Filename: domain/track_recorder/recording_bar_length/RecordingBarLengthScroller.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/shared/backend/__init__.py
+Filename: domain/track_recorder/recording_bar_length/SelectedRecordingBarLengthUpdatedEvent.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/shared/errors/ErrorRaisedEvent.py
+Filename: domain/track_recorder/recording_bar_length/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/shared/errors/error_handler.py
+Filename: domain/track_recorder/simple/PostRecordSimple.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/shared/errors/Protocol0Error.py
+Filename: domain/track_recorder/simple/RecorderSimpleFactory.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/shared/errors/Protocol0Warning.py
+Filename: domain/track_recorder/simple/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/shared/errors/__init__.py
+Filename: infra/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/shared/event/DomainEventBus.py
+Filename: infra/interface/BrowserLoaderService.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/shared/event/HasEmitter.py
+Filename: infra/interface/BrowserService.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/shared/event/__init__.py
+Filename: infra/interface/InterfaceClicksService.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/shared/scheduler/BarChangedEvent.py
+Filename: infra/interface/PixelEnum.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/shared/scheduler/BarEndingEvent.py
+Filename: infra/interface/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/shared/scheduler/BeatSchedulerInterface.py
+Filename: infra/interface/session/SessionService.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/shared/scheduler/Last16thPassedEvent.py
+Filename: infra/interface/session/SessionUpdatedEvent.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/shared/scheduler/Last32thPassedEvent.py
+Filename: infra/interface/session/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/shared/scheduler/Last8thPassedEvent.py
+Filename: infra/logging/LoggerService.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/shared/scheduler/LastBeatPassedEvent.py
+Filename: infra/logging/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/shared/scheduler/Scheduler.py
+Filename: infra/midi/MidiBytesReceivedEvent.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/shared/scheduler/ThirdBeatPassedEvent.py
+Filename: infra/midi/MidiBytesSentEvent.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/shared/scheduler/TickSchedulerEventInterface.py
+Filename: infra/midi/MidiService.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/shared/scheduler/TickSchedulerInterface.py
+Filename: infra/midi/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/shared/scheduler/__init__.py
+Filename: infra/persistence/SongDataEnum.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/shared/script/__init__.py
+Filename: infra/persistence/SongDataService.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/shared/ui/ColorEnum.py
+Filename: infra/persistence/TrackData.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/shared/ui/__init__.py
+Filename: infra/persistence/TrackDataEnum.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/shared/utils/concurrency.py
+Filename: infra/persistence/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/shared/utils/debug.py
+Filename: infra/scheduler/BeatScheduler.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/shared/utils/forward_to.py
+Filename: infra/scheduler/BeatSchedulerEvent.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/shared/utils/func.py
+Filename: infra/scheduler/BeatTime.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/shared/utils/list.py
+Filename: infra/scheduler/TickScheduler.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/shared/utils/string.py
+Filename: infra/scheduler/TickSchedulerEvent.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/shared/utils/timing.py
+Filename: infra/scheduler/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/shared/utils/utils.py
+Filename: shared/AbstractEnum.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/shared/utils/__init__.py
+Filename: shared/Config.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/track_recorder/config/
+Filename: shared/Song.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/track_recorder/count_in/
+Filename: shared/UndoFacade.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/track_recorder/event/
+Filename: shared/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/track_recorder/external_synth/
+Filename: shared/types.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/track_recorder/recording_bar_length/
+Filename: shared/logging/LogLevelEnum.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/track_recorder/simple/
+Filename: shared/logging/Logger.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/track_recorder/AbstractRecorderFactory.py
+Filename: shared/logging/LoggerServiceInterface.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/track_recorder/BaseRecorder.py
+Filename: shared/logging/StatusBar.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/track_recorder/RecordProcessorInterface.py
+Filename: shared/logging/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/track_recorder/RecordService.py
+Filename: shared/observer/Observable.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/track_recorder/RecordTypeEnum.py
+Filename: shared/observer/Observer.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/track_recorder/__init__.py
+Filename: shared/observer/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/track_recorder/config/RecordConfig.py
+Filename: shared/sequence/HasSequenceState.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/track_recorder/config/RecordProcessors.py
+Filename: shared/sequence/ParallelSequence.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/track_recorder/config/__init__.py
+Filename: shared/sequence/Sequence.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/track_recorder/count_in/CountInInterface.py
+Filename: shared/sequence/SequenceState.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/track_recorder/count_in/CountInOneBar.py
+Filename: shared/sequence/SequenceStep.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/track_recorder/count_in/CountInShort.py
+Filename: shared/sequence/SequenceTransition.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/track_recorder/count_in/__init__.py
+Filename: shared/sequence/TimeoutLimit.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/track_recorder/event/RecordCancelledEvent.py
+Filename: shared/sequence/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/track_recorder/event/RecordEndedEvent.py
+Filename: tests/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/track_recorder/event/RecordStartedEvent.py
+Filename: tests/application/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/track_recorder/event/__init__.py
+Filename: tests/application/test_multi_encoder.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/track_recorder/external_synth/record_audio/
+Filename: tests/domain/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/track_recorder/external_synth/record_midi/
+Filename: tests/domain/clip/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/track_recorder/external_synth/AudioClipSilentEvent.py
+Filename: tests/domain/clip/test_clip_playing_position.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/track_recorder/external_synth/ExtAudioRecordingEndedEvent.py
+Filename: tests/domain/fixtures/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/track_recorder/external_synth/ExtAudioRecordingStartedEvent.py
+Filename: tests/domain/fixtures/clip.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/track_recorder/external_synth/OnRecordEndClipTail.py
+Filename: tests/domain/fixtures/clip_slot.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/track_recorder/external_synth/TrackRecorderExternalSynthFactory.py
+Filename: tests/domain/fixtures/clip_view.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/track_recorder/external_synth/__init__.py
+Filename: tests/domain/fixtures/container.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/track_recorder/external_synth/record_audio/record_multi/
+Filename: tests/domain/fixtures/device.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/track_recorder/external_synth/record_audio/PostRecordAudio.py
+Filename: tests/domain/fixtures/device_parameter.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/track_recorder/external_synth/record_audio/PostRecordAudioFull.py
+Filename: tests/domain/fixtures/group_track.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/track_recorder/external_synth/record_audio/PreRecordAudio.py
+Filename: tests/domain/fixtures/p0.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/track_recorder/external_synth/record_audio/__init__.py
+Filename: tests/domain/fixtures/scene.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/track_recorder/external_synth/record_audio/record_multi/PreRecordAudioMulti.py
+Filename: tests/domain/fixtures/simple_track.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/track_recorder/external_synth/record_audio/record_multi/RecordAudioMulti.py
+Filename: tests/domain/fixtures/song.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/track_recorder/external_synth/record_audio/record_multi/__init__.py
+Filename: tests/domain/fixtures/song_view.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/track_recorder/external_synth/record_midi/PostRecordMidi.py
+Filename: tests/domain/scene/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/track_recorder/external_synth/record_midi/PreRecordMidi.py
+Filename: tests/domain/scene/test_scene_clips.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/track_recorder/external_synth/record_midi/__init__.py
+Filename: tests/domain/scene/test_scene_length.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/track_recorder/recording_bar_length/RecordingBarLengthEnum.py
+Filename: tests/domain/scene/test_scene_playing_position.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/track_recorder/recording_bar_length/RecordingBarLengthScroller.py
+Filename: tests/domain/shared/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/track_recorder/recording_bar_length/SelectedRecordingBarLengthUpdatedEvent.py
+Filename: tests/domain/shared/test_decorators.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/track_recorder/recording_bar_length/__init__.py
+Filename: tests/domain/shared/test_live_object_mapping.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/track_recorder/simple/PostRecordSimple.py
+Filename: tests/domain/shared/event/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/track_recorder/simple/RecorderSimpleFactory.py
+Filename: tests/domain/shared/event/test_domain_event_bus.py
 Comment: 
 
-Filename: p0-script-1.0.2/domain/track_recorder/simple/__init__.py
+Filename: tests/domain/shared/utils/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/infra/interface/
+Filename: tests/domain/shared/utils/test_func.py
 Comment: 
 
-Filename: p0-script-1.0.2/infra/logging/
+Filename: tests/domain/shared/utils/test_utils.py
 Comment: 
 
-Filename: p0-script-1.0.2/infra/midi/
+Filename: tests/domain/track/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/infra/persistence/
+Filename: tests/domain/track/test_audio_to_midi_clip_mapping.py
 Comment: 
 
-Filename: p0-script-1.0.2/infra/scheduler/
+Filename: tests/domain/track/test_instantiation.py
 Comment: 
 
-Filename: p0-script-1.0.2/infra/__init__.py
+Filename: tests/domain/validation/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/infra/interface/session/
+Filename: tests/domain/validation/test_aggregate_validator.py
 Comment: 
 
-Filename: p0-script-1.0.2/infra/interface/BrowserLoaderService.py
+Filename: tests/domain/validation/test_callback_validator.py
 Comment: 
 
-Filename: p0-script-1.0.2/infra/interface/BrowserService.py
+Filename: tests/domain/validation/test_property_validator.py
 Comment: 
 
-Filename: p0-script-1.0.2/infra/interface/InterfaceClicksService.py
+Filename: tests/infra/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/infra/interface/PixelEnum.py
+Filename: tests/infra/test_scheduler.py
 Comment: 
 
-Filename: p0-script-1.0.2/infra/interface/__init__.py
+Filename: tests/infra/listeners/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/infra/interface/session/SessionService.py
+Filename: tests/infra/listeners/test_subject_slot.py
 Comment: 
 
-Filename: p0-script-1.0.2/infra/interface/session/SessionUpdatedEvent.py
+Filename: tests/infra/scheduler/TickSchedulerEventTest.py
 Comment: 
 
-Filename: p0-script-1.0.2/infra/interface/session/__init__.py
+Filename: tests/infra/scheduler/TickSchedulerTest.py
 Comment: 
 
-Filename: p0-script-1.0.2/infra/logging/LoggerService.py
+Filename: tests/infra/scheduler/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/infra/logging/__init__.py
+Filename: tests/shared/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/infra/midi/MidiBytesReceivedEvent.py
+Filename: tests/shared/test_container.py
 Comment: 
 
-Filename: p0-script-1.0.2/infra/midi/MidiBytesSentEvent.py
+Filename: tests/shared/sequence/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/infra/midi/MidiService.py
+Filename: tests/shared/sequence/test_sanity_sequence.py
 Comment: 
 
-Filename: p0-script-1.0.2/infra/midi/__init__.py
+Filename: tests/shared/sequence/test_sequence.py
 Comment: 
 
-Filename: p0-script-1.0.2/infra/persistence/SongDataEnum.py
+Filename: tests/shared/sequence/test_sequence_parallel.py
 Comment: 
 
-Filename: p0-script-1.0.2/infra/persistence/SongDataService.py
+Filename: venv/Lib/site-packages/easy_install.py
 Comment: 
 
-Filename: p0-script-1.0.2/infra/persistence/TrackData.py
+Filename: venv/Lib/site-packages/pip/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/infra/persistence/TrackDataEnum.py
+Filename: venv/Lib/site-packages/pip/__main__.py
 Comment: 
 
-Filename: p0-script-1.0.2/infra/persistence/__init__.py
+Filename: venv/Lib/site-packages/pip/_internal/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/infra/scheduler/BeatScheduler.py
+Filename: venv/Lib/site-packages/pip/_internal/basecommand.py
 Comment: 
 
-Filename: p0-script-1.0.2/infra/scheduler/BeatSchedulerEvent.py
+Filename: venv/Lib/site-packages/pip/_internal/baseparser.py
 Comment: 
 
-Filename: p0-script-1.0.2/infra/scheduler/BeatTime.py
+Filename: venv/Lib/site-packages/pip/_internal/build_env.py
 Comment: 
 
-Filename: p0-script-1.0.2/infra/scheduler/TickScheduler.py
+Filename: venv/Lib/site-packages/pip/_internal/cache.py
 Comment: 
 
-Filename: p0-script-1.0.2/infra/scheduler/TickSchedulerEvent.py
+Filename: venv/Lib/site-packages/pip/_internal/cmdoptions.py
 Comment: 
 
-Filename: p0-script-1.0.2/infra/scheduler/__init__.py
+Filename: venv/Lib/site-packages/pip/_internal/compat.py
 Comment: 
 
-Filename: p0-script-1.0.2/p0_script.egg-info/dependency_links.txt
+Filename: venv/Lib/site-packages/pip/_internal/configuration.py
 Comment: 
 
-Filename: p0-script-1.0.2/p0_script.egg-info/PKG-INFO
+Filename: venv/Lib/site-packages/pip/_internal/download.py
 Comment: 
 
-Filename: p0-script-1.0.2/p0_script.egg-info/requires.txt
+Filename: venv/Lib/site-packages/pip/_internal/exceptions.py
 Comment: 
 
-Filename: p0-script-1.0.2/p0_script.egg-info/SOURCES.txt
+Filename: venv/Lib/site-packages/pip/_internal/index.py
 Comment: 
 
-Filename: p0-script-1.0.2/p0_script.egg-info/top_level.txt
+Filename: venv/Lib/site-packages/pip/_internal/locations.py
 Comment: 
 
-Filename: p0-script-1.0.2/shared/logging/
+Filename: venv/Lib/site-packages/pip/_internal/pep425tags.py
 Comment: 
 
-Filename: p0-script-1.0.2/shared/observer/
+Filename: venv/Lib/site-packages/pip/_internal/resolve.py
 Comment: 
 
-Filename: p0-script-1.0.2/shared/sequence/
+Filename: venv/Lib/site-packages/pip/_internal/status_codes.py
 Comment: 
 
-Filename: p0-script-1.0.2/shared/AbstractEnum.py
+Filename: venv/Lib/site-packages/pip/_internal/wheel.py
 Comment: 
 
-Filename: p0-script-1.0.2/shared/Config.py
+Filename: venv/Lib/site-packages/pip/_internal/commands/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/shared/Song.py
+Filename: venv/Lib/site-packages/pip/_internal/commands/check.py
 Comment: 
 
-Filename: p0-script-1.0.2/shared/types.py
+Filename: venv/Lib/site-packages/pip/_internal/commands/completion.py
 Comment: 
 
-Filename: p0-script-1.0.2/shared/UndoFacade.py
+Filename: venv/Lib/site-packages/pip/_internal/commands/configuration.py
 Comment: 
 
-Filename: p0-script-1.0.2/shared/__init__.py
+Filename: venv/Lib/site-packages/pip/_internal/commands/download.py
 Comment: 
 
-Filename: p0-script-1.0.2/shared/logging/Logger.py
+Filename: venv/Lib/site-packages/pip/_internal/commands/freeze.py
 Comment: 
 
-Filename: p0-script-1.0.2/shared/logging/LoggerServiceInterface.py
+Filename: venv/Lib/site-packages/pip/_internal/commands/hash.py
 Comment: 
 
-Filename: p0-script-1.0.2/shared/logging/LogLevelEnum.py
+Filename: venv/Lib/site-packages/pip/_internal/commands/help.py
 Comment: 
 
-Filename: p0-script-1.0.2/shared/logging/StatusBar.py
+Filename: venv/Lib/site-packages/pip/_internal/commands/install.py
 Comment: 
 
-Filename: p0-script-1.0.2/shared/logging/__init__.py
+Filename: venv/Lib/site-packages/pip/_internal/commands/list.py
 Comment: 
 
-Filename: p0-script-1.0.2/shared/observer/Observable.py
+Filename: venv/Lib/site-packages/pip/_internal/commands/search.py
 Comment: 
 
-Filename: p0-script-1.0.2/shared/observer/Observer.py
+Filename: venv/Lib/site-packages/pip/_internal/commands/show.py
 Comment: 
 
-Filename: p0-script-1.0.2/shared/observer/__init__.py
+Filename: venv/Lib/site-packages/pip/_internal/commands/uninstall.py
 Comment: 
 
-Filename: p0-script-1.0.2/shared/sequence/HasSequenceState.py
+Filename: venv/Lib/site-packages/pip/_internal/commands/wheel.py
 Comment: 
 
-Filename: p0-script-1.0.2/shared/sequence/ParallelSequence.py
+Filename: venv/Lib/site-packages/pip/_internal/models/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/shared/sequence/Sequence.py
+Filename: venv/Lib/site-packages/pip/_internal/models/index.py
 Comment: 
 
-Filename: p0-script-1.0.2/shared/sequence/SequenceState.py
+Filename: venv/Lib/site-packages/pip/_internal/operations/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/shared/sequence/SequenceStep.py
+Filename: venv/Lib/site-packages/pip/_internal/operations/check.py
 Comment: 
 
-Filename: p0-script-1.0.2/shared/sequence/SequenceTransition.py
+Filename: venv/Lib/site-packages/pip/_internal/operations/freeze.py
 Comment: 
 
-Filename: p0-script-1.0.2/shared/sequence/TimeoutLimit.py
+Filename: venv/Lib/site-packages/pip/_internal/operations/prepare.py
 Comment: 
 
-Filename: p0-script-1.0.2/shared/sequence/__init__.py
+Filename: venv/Lib/site-packages/pip/_internal/req/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/tests/application/
+Filename: venv/Lib/site-packages/pip/_internal/req/req_file.py
 Comment: 
 
-Filename: p0-script-1.0.2/tests/domain/
+Filename: venv/Lib/site-packages/pip/_internal/req/req_install.py
 Comment: 
 
-Filename: p0-script-1.0.2/tests/infra/
+Filename: venv/Lib/site-packages/pip/_internal/req/req_set.py
 Comment: 
 
-Filename: p0-script-1.0.2/tests/shared/
+Filename: venv/Lib/site-packages/pip/_internal/req/req_uninstall.py
 Comment: 
 
-Filename: p0-script-1.0.2/tests/__init__.py
+Filename: venv/Lib/site-packages/pip/_internal/utils/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/tests/application/test_multi_encoder.py
+Filename: venv/Lib/site-packages/pip/_internal/utils/appdirs.py
 Comment: 
 
-Filename: p0-script-1.0.2/tests/application/__init__.py
+Filename: venv/Lib/site-packages/pip/_internal/utils/deprecation.py
 Comment: 
 
-Filename: p0-script-1.0.2/tests/domain/clip/
+Filename: venv/Lib/site-packages/pip/_internal/utils/encoding.py
 Comment: 
 
-Filename: p0-script-1.0.2/tests/domain/fixtures/
+Filename: venv/Lib/site-packages/pip/_internal/utils/filesystem.py
 Comment: 
 
-Filename: p0-script-1.0.2/tests/domain/scene/
+Filename: venv/Lib/site-packages/pip/_internal/utils/glibc.py
 Comment: 
 
-Filename: p0-script-1.0.2/tests/domain/shared/
+Filename: venv/Lib/site-packages/pip/_internal/utils/hashes.py
 Comment: 
 
-Filename: p0-script-1.0.2/tests/domain/track/
+Filename: venv/Lib/site-packages/pip/_internal/utils/logging.py
 Comment: 
 
-Filename: p0-script-1.0.2/tests/domain/validation/
+Filename: venv/Lib/site-packages/pip/_internal/utils/misc.py
 Comment: 
 
-Filename: p0-script-1.0.2/tests/domain/__init__.py
+Filename: venv/Lib/site-packages/pip/_internal/utils/outdated.py
 Comment: 
 
-Filename: p0-script-1.0.2/tests/domain/clip/test_clip_playing_position.py
+Filename: venv/Lib/site-packages/pip/_internal/utils/packaging.py
 Comment: 
 
-Filename: p0-script-1.0.2/tests/domain/clip/__init__.py
+Filename: venv/Lib/site-packages/pip/_internal/utils/setuptools_build.py
 Comment: 
 
-Filename: p0-script-1.0.2/tests/domain/fixtures/clip.py
+Filename: venv/Lib/site-packages/pip/_internal/utils/temp_dir.py
 Comment: 
 
-Filename: p0-script-1.0.2/tests/domain/fixtures/clip_slot.py
+Filename: venv/Lib/site-packages/pip/_internal/utils/typing.py
 Comment: 
 
-Filename: p0-script-1.0.2/tests/domain/fixtures/clip_view.py
+Filename: venv/Lib/site-packages/pip/_internal/utils/ui.py
 Comment: 
 
-Filename: p0-script-1.0.2/tests/domain/fixtures/container.py
+Filename: venv/Lib/site-packages/pip/_internal/vcs/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/tests/domain/fixtures/device.py
+Filename: venv/Lib/site-packages/pip/_internal/vcs/bazaar.py
 Comment: 
 
-Filename: p0-script-1.0.2/tests/domain/fixtures/device_parameter.py
+Filename: venv/Lib/site-packages/pip/_internal/vcs/git.py
 Comment: 
 
-Filename: p0-script-1.0.2/tests/domain/fixtures/group_track.py
+Filename: venv/Lib/site-packages/pip/_internal/vcs/mercurial.py
 Comment: 
 
-Filename: p0-script-1.0.2/tests/domain/fixtures/p0.py
+Filename: venv/Lib/site-packages/pip/_internal/vcs/subversion.py
 Comment: 
 
-Filename: p0-script-1.0.2/tests/domain/fixtures/scene.py
+Filename: venv/Lib/site-packages/pip/_vendor/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/tests/domain/fixtures/simple_track.py
+Filename: venv/Lib/site-packages/pip/_vendor/appdirs.py
 Comment: 
 
-Filename: p0-script-1.0.2/tests/domain/fixtures/song.py
+Filename: venv/Lib/site-packages/pip/_vendor/distro.py
 Comment: 
 
-Filename: p0-script-1.0.2/tests/domain/fixtures/song_view.py
+Filename: venv/Lib/site-packages/pip/_vendor/ipaddress.py
 Comment: 
 
-Filename: p0-script-1.0.2/tests/domain/fixtures/__init__.py
+Filename: venv/Lib/site-packages/pip/_vendor/pyparsing.py
 Comment: 
 
-Filename: p0-script-1.0.2/tests/domain/scene/test_scene_clips.py
+Filename: venv/Lib/site-packages/pip/_vendor/retrying.py
 Comment: 
 
-Filename: p0-script-1.0.2/tests/domain/scene/test_scene_length.py
+Filename: venv/Lib/site-packages/pip/_vendor/six.py
 Comment: 
 
-Filename: p0-script-1.0.2/tests/domain/scene/test_scene_playing_position.py
+Filename: venv/Lib/site-packages/pip/_vendor/cachecontrol/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/tests/domain/scene/__init__.py
+Filename: venv/Lib/site-packages/pip/_vendor/cachecontrol/_cmd.py
 Comment: 
 
-Filename: p0-script-1.0.2/tests/domain/shared/event/
+Filename: venv/Lib/site-packages/pip/_vendor/cachecontrol/adapter.py
 Comment: 
 
-Filename: p0-script-1.0.2/tests/domain/shared/utils/
+Filename: venv/Lib/site-packages/pip/_vendor/cachecontrol/cache.py
 Comment: 
 
-Filename: p0-script-1.0.2/tests/domain/shared/test_decorators.py
+Filename: venv/Lib/site-packages/pip/_vendor/cachecontrol/compat.py
 Comment: 
 
-Filename: p0-script-1.0.2/tests/domain/shared/test_live_object_mapping.py
+Filename: venv/Lib/site-packages/pip/_vendor/cachecontrol/controller.py
 Comment: 
 
-Filename: p0-script-1.0.2/tests/domain/shared/__init__.py
+Filename: venv/Lib/site-packages/pip/_vendor/cachecontrol/filewrapper.py
 Comment: 
 
-Filename: p0-script-1.0.2/tests/domain/shared/event/test_domain_event_bus.py
+Filename: venv/Lib/site-packages/pip/_vendor/cachecontrol/heuristics.py
 Comment: 
 
-Filename: p0-script-1.0.2/tests/domain/shared/event/__init__.py
+Filename: venv/Lib/site-packages/pip/_vendor/cachecontrol/serialize.py
 Comment: 
 
-Filename: p0-script-1.0.2/tests/domain/shared/utils/test_func.py
+Filename: venv/Lib/site-packages/pip/_vendor/cachecontrol/wrapper.py
 Comment: 
 
-Filename: p0-script-1.0.2/tests/domain/shared/utils/test_utils.py
+Filename: venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/tests/domain/shared/utils/__init__.py
+Filename: venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py
 Comment: 
 
-Filename: p0-script-1.0.2/tests/domain/track/test_audio_to_midi_clip_mapping.py
+Filename: venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py
 Comment: 
 
-Filename: p0-script-1.0.2/tests/domain/track/test_instantiation.py
+Filename: venv/Lib/site-packages/pip/_vendor/certifi/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/tests/domain/track/__init__.py
+Filename: venv/Lib/site-packages/pip/_vendor/certifi/__main__.py
 Comment: 
 
-Filename: p0-script-1.0.2/tests/domain/validation/test_aggregate_validator.py
+Filename: venv/Lib/site-packages/pip/_vendor/certifi/core.py
 Comment: 
 
-Filename: p0-script-1.0.2/tests/domain/validation/test_callback_validator.py
+Filename: venv/Lib/site-packages/pip/_vendor/chardet/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/tests/domain/validation/test_property_validator.py
+Filename: venv/Lib/site-packages/pip/_vendor/chardet/big5freq.py
 Comment: 
 
-Filename: p0-script-1.0.2/tests/domain/validation/__init__.py
+Filename: venv/Lib/site-packages/pip/_vendor/chardet/big5prober.py
 Comment: 
 
-Filename: p0-script-1.0.2/tests/infra/listeners/
+Filename: venv/Lib/site-packages/pip/_vendor/chardet/chardistribution.py
 Comment: 
 
-Filename: p0-script-1.0.2/tests/infra/scheduler/
+Filename: venv/Lib/site-packages/pip/_vendor/chardet/charsetgroupprober.py
 Comment: 
 
-Filename: p0-script-1.0.2/tests/infra/test_scheduler.py
+Filename: venv/Lib/site-packages/pip/_vendor/chardet/charsetprober.py
 Comment: 
 
-Filename: p0-script-1.0.2/tests/infra/__init__.py
+Filename: venv/Lib/site-packages/pip/_vendor/chardet/codingstatemachine.py
 Comment: 
 
-Filename: p0-script-1.0.2/tests/infra/listeners/test_subject_slot.py
+Filename: venv/Lib/site-packages/pip/_vendor/chardet/compat.py
 Comment: 
 
-Filename: p0-script-1.0.2/tests/infra/listeners/__init__.py
+Filename: venv/Lib/site-packages/pip/_vendor/chardet/cp949prober.py
 Comment: 
 
-Filename: p0-script-1.0.2/tests/infra/scheduler/TickSchedulerEventTest.py
+Filename: venv/Lib/site-packages/pip/_vendor/chardet/enums.py
 Comment: 
 
-Filename: p0-script-1.0.2/tests/infra/scheduler/TickSchedulerTest.py
+Filename: venv/Lib/site-packages/pip/_vendor/chardet/escprober.py
 Comment: 
 
-Filename: p0-script-1.0.2/tests/infra/scheduler/__init__.py
+Filename: venv/Lib/site-packages/pip/_vendor/chardet/escsm.py
 Comment: 
 
-Filename: p0-script-1.0.2/tests/shared/sequence/
+Filename: venv/Lib/site-packages/pip/_vendor/chardet/eucjpprober.py
 Comment: 
 
-Filename: p0-script-1.0.2/tests/shared/test_container.py
+Filename: venv/Lib/site-packages/pip/_vendor/chardet/euckrfreq.py
 Comment: 
 
-Filename: p0-script-1.0.2/tests/shared/__init__.py
+Filename: venv/Lib/site-packages/pip/_vendor/chardet/euckrprober.py
 Comment: 
 
-Filename: p0-script-1.0.2/tests/shared/sequence/test_sanity_sequence.py
+Filename: venv/Lib/site-packages/pip/_vendor/chardet/euctwfreq.py
 Comment: 
 
-Filename: p0-script-1.0.2/tests/shared/sequence/test_sequence.py
+Filename: venv/Lib/site-packages/pip/_vendor/chardet/euctwprober.py
 Comment: 
 
-Filename: p0-script-1.0.2/tests/shared/sequence/test_sequence_parallel.py
+Filename: venv/Lib/site-packages/pip/_vendor/chardet/gb2312freq.py
 Comment: 
 
-Filename: p0-script-1.0.2/tests/shared/sequence/__init__.py
+Filename: venv/Lib/site-packages/pip/_vendor/chardet/gb2312prober.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/
+Filename: venv/Lib/site-packages/pip/_vendor/chardet/hebrewprober.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/
+Filename: venv/Lib/site-packages/pip/_vendor/chardet/jisfreq.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/
+Filename: venv/Lib/site-packages/pip/_vendor/chardet/jpcntx.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pkg_resources/
+Filename: venv/Lib/site-packages/pip/_vendor/chardet/langbulgarianmodel.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/setuptools/
+Filename: venv/Lib/site-packages/pip/_vendor/chardet/langcyrillicmodel.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/easy_install.py
+Filename: venv/Lib/site-packages/pip/_vendor/chardet/langgreekmodel.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/
+Filename: venv/Lib/site-packages/pip/_vendor/chardet/langhebrewmodel.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/
+Filename: venv/Lib/site-packages/pip/_vendor/chardet/langhungarianmodel.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/__init__.py
+Filename: venv/Lib/site-packages/pip/_vendor/chardet/langthaimodel.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/__main__.py
+Filename: venv/Lib/site-packages/pip/_vendor/chardet/langturkishmodel.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/commands/
+Filename: venv/Lib/site-packages/pip/_vendor/chardet/latin1prober.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/models/
+Filename: venv/Lib/site-packages/pip/_vendor/chardet/mbcharsetprober.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/operations/
+Filename: venv/Lib/site-packages/pip/_vendor/chardet/mbcsgroupprober.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/req/
+Filename: venv/Lib/site-packages/pip/_vendor/chardet/mbcssm.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/utils/
+Filename: venv/Lib/site-packages/pip/_vendor/chardet/sbcharsetprober.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/vcs/
+Filename: venv/Lib/site-packages/pip/_vendor/chardet/sbcsgroupprober.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/basecommand.py
+Filename: venv/Lib/site-packages/pip/_vendor/chardet/sjisprober.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/baseparser.py
+Filename: venv/Lib/site-packages/pip/_vendor/chardet/universaldetector.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/build_env.py
+Filename: venv/Lib/site-packages/pip/_vendor/chardet/utf8prober.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/cache.py
+Filename: venv/Lib/site-packages/pip/_vendor/chardet/version.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/cmdoptions.py
+Filename: venv/Lib/site-packages/pip/_vendor/chardet/cli/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/compat.py
+Filename: venv/Lib/site-packages/pip/_vendor/chardet/cli/chardetect.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/configuration.py
+Filename: venv/Lib/site-packages/pip/_vendor/colorama/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/download.py
+Filename: venv/Lib/site-packages/pip/_vendor/colorama/ansi.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/exceptions.py
+Filename: venv/Lib/site-packages/pip/_vendor/colorama/ansitowin32.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/index.py
+Filename: venv/Lib/site-packages/pip/_vendor/colorama/initialise.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/locations.py
+Filename: venv/Lib/site-packages/pip/_vendor/colorama/win32.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/pep425tags.py
+Filename: venv/Lib/site-packages/pip/_vendor/colorama/winterm.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/resolve.py
+Filename: venv/Lib/site-packages/pip/_vendor/distlib/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/status_codes.py
+Filename: venv/Lib/site-packages/pip/_vendor/distlib/compat.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/wheel.py
+Filename: venv/Lib/site-packages/pip/_vendor/distlib/database.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/__init__.py
+Filename: venv/Lib/site-packages/pip/_vendor/distlib/index.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/commands/check.py
+Filename: venv/Lib/site-packages/pip/_vendor/distlib/locators.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/commands/completion.py
+Filename: venv/Lib/site-packages/pip/_vendor/distlib/manifest.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/commands/configuration.py
+Filename: venv/Lib/site-packages/pip/_vendor/distlib/markers.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/commands/download.py
+Filename: venv/Lib/site-packages/pip/_vendor/distlib/metadata.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/commands/freeze.py
+Filename: venv/Lib/site-packages/pip/_vendor/distlib/resources.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/commands/hash.py
+Filename: venv/Lib/site-packages/pip/_vendor/distlib/scripts.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/commands/help.py
+Filename: venv/Lib/site-packages/pip/_vendor/distlib/util.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/commands/install.py
+Filename: venv/Lib/site-packages/pip/_vendor/distlib/version.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/commands/list.py
+Filename: venv/Lib/site-packages/pip/_vendor/distlib/wheel.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/commands/search.py
+Filename: venv/Lib/site-packages/pip/_vendor/distlib/_backport/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/commands/show.py
+Filename: venv/Lib/site-packages/pip/_vendor/distlib/_backport/misc.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/commands/uninstall.py
+Filename: venv/Lib/site-packages/pip/_vendor/distlib/_backport/shutil.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/commands/wheel.py
+Filename: venv/Lib/site-packages/pip/_vendor/distlib/_backport/sysconfig.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/commands/__init__.py
+Filename: venv/Lib/site-packages/pip/_vendor/distlib/_backport/tarfile.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/models/index.py
+Filename: venv/Lib/site-packages/pip/_vendor/html5lib/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/models/__init__.py
+Filename: venv/Lib/site-packages/pip/_vendor/html5lib/_ihatexml.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/operations/check.py
+Filename: venv/Lib/site-packages/pip/_vendor/html5lib/_inputstream.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/operations/freeze.py
+Filename: venv/Lib/site-packages/pip/_vendor/html5lib/_tokenizer.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/operations/prepare.py
+Filename: venv/Lib/site-packages/pip/_vendor/html5lib/_utils.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/operations/__init__.py
+Filename: venv/Lib/site-packages/pip/_vendor/html5lib/constants.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/req/req_file.py
+Filename: venv/Lib/site-packages/pip/_vendor/html5lib/html5parser.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/req/req_install.py
+Filename: venv/Lib/site-packages/pip/_vendor/html5lib/serializer.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/req/req_set.py
+Filename: venv/Lib/site-packages/pip/_vendor/html5lib/_trie/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/req/req_uninstall.py
+Filename: venv/Lib/site-packages/pip/_vendor/html5lib/_trie/_base.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/req/__init__.py
+Filename: venv/Lib/site-packages/pip/_vendor/html5lib/_trie/datrie.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/utils/appdirs.py
+Filename: venv/Lib/site-packages/pip/_vendor/html5lib/_trie/py.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/utils/deprecation.py
+Filename: venv/Lib/site-packages/pip/_vendor/html5lib/filters/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/utils/encoding.py
+Filename: venv/Lib/site-packages/pip/_vendor/html5lib/filters/alphabeticalattributes.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/utils/filesystem.py
+Filename: venv/Lib/site-packages/pip/_vendor/html5lib/filters/base.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/utils/glibc.py
+Filename: venv/Lib/site-packages/pip/_vendor/html5lib/filters/inject_meta_charset.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/utils/hashes.py
+Filename: venv/Lib/site-packages/pip/_vendor/html5lib/filters/lint.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/utils/logging.py
+Filename: venv/Lib/site-packages/pip/_vendor/html5lib/filters/optionaltags.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/utils/misc.py
+Filename: venv/Lib/site-packages/pip/_vendor/html5lib/filters/sanitizer.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/utils/outdated.py
+Filename: venv/Lib/site-packages/pip/_vendor/html5lib/filters/whitespace.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/utils/packaging.py
+Filename: venv/Lib/site-packages/pip/_vendor/html5lib/treeadapters/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/utils/setuptools_build.py
+Filename: venv/Lib/site-packages/pip/_vendor/html5lib/treeadapters/genshi.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/utils/temp_dir.py
+Filename: venv/Lib/site-packages/pip/_vendor/html5lib/treeadapters/sax.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/utils/typing.py
+Filename: venv/Lib/site-packages/pip/_vendor/html5lib/treebuilders/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/utils/ui.py
+Filename: venv/Lib/site-packages/pip/_vendor/html5lib/treebuilders/base.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/utils/__init__.py
+Filename: venv/Lib/site-packages/pip/_vendor/html5lib/treebuilders/dom.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/vcs/bazaar.py
+Filename: venv/Lib/site-packages/pip/_vendor/html5lib/treebuilders/etree.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/vcs/git.py
+Filename: venv/Lib/site-packages/pip/_vendor/html5lib/treebuilders/etree_lxml.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/vcs/mercurial.py
+Filename: venv/Lib/site-packages/pip/_vendor/html5lib/treewalkers/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/vcs/subversion.py
+Filename: venv/Lib/site-packages/pip/_vendor/html5lib/treewalkers/base.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/vcs/__init__.py
+Filename: venv/Lib/site-packages/pip/_vendor/html5lib/treewalkers/dom.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/
+Filename: venv/Lib/site-packages/pip/_vendor/html5lib/treewalkers/etree.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/certifi/
+Filename: venv/Lib/site-packages/pip/_vendor/html5lib/treewalkers/etree_lxml.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/
+Filename: venv/Lib/site-packages/pip/_vendor/html5lib/treewalkers/genshi.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/colorama/
+Filename: venv/Lib/site-packages/pip/_vendor/idna/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/distlib/
+Filename: venv/Lib/site-packages/pip/_vendor/idna/codec.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/
+Filename: venv/Lib/site-packages/pip/_vendor/idna/compat.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/idna/
+Filename: venv/Lib/site-packages/pip/_vendor/idna/core.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/lockfile/
+Filename: venv/Lib/site-packages/pip/_vendor/idna/idnadata.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/msgpack/
+Filename: venv/Lib/site-packages/pip/_vendor/idna/intranges.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/packaging/
+Filename: venv/Lib/site-packages/pip/_vendor/idna/package_data.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/pkg_resources/
+Filename: venv/Lib/site-packages/pip/_vendor/idna/uts46data.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/progress/
+Filename: venv/Lib/site-packages/pip/_vendor/lockfile/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/pytoml/
+Filename: venv/Lib/site-packages/pip/_vendor/lockfile/linklockfile.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/requests/
+Filename: venv/Lib/site-packages/pip/_vendor/lockfile/mkdirlockfile.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/
+Filename: venv/Lib/site-packages/pip/_vendor/lockfile/pidlockfile.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/webencodings/
+Filename: venv/Lib/site-packages/pip/_vendor/lockfile/sqlitelockfile.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/appdirs.py
+Filename: venv/Lib/site-packages/pip/_vendor/lockfile/symlinklockfile.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/distro.py
+Filename: venv/Lib/site-packages/pip/_vendor/msgpack/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/ipaddress.py
+Filename: venv/Lib/site-packages/pip/_vendor/msgpack/_version.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/pyparsing.py
+Filename: venv/Lib/site-packages/pip/_vendor/msgpack/exceptions.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/retrying.py
+Filename: venv/Lib/site-packages/pip/_vendor/msgpack/fallback.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/six.py
+Filename: venv/Lib/site-packages/pip/_vendor/packaging/__about__.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/__init__.py
+Filename: venv/Lib/site-packages/pip/_vendor/packaging/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/
+Filename: venv/Lib/site-packages/pip/_vendor/packaging/_compat.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/adapter.py
+Filename: venv/Lib/site-packages/pip/_vendor/packaging/_structures.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/cache.py
+Filename: venv/Lib/site-packages/pip/_vendor/packaging/markers.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/compat.py
+Filename: venv/Lib/site-packages/pip/_vendor/packaging/requirements.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/controller.py
+Filename: venv/Lib/site-packages/pip/_vendor/packaging/specifiers.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/filewrapper.py
+Filename: venv/Lib/site-packages/pip/_vendor/packaging/utils.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/heuristics.py
+Filename: venv/Lib/site-packages/pip/_vendor/packaging/version.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/serialize.py
+Filename: venv/Lib/site-packages/pip/_vendor/pkg_resources/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/wrapper.py
+Filename: venv/Lib/site-packages/pip/_vendor/pkg_resources/py31compat.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/_cmd.py
+Filename: venv/Lib/site-packages/pip/_vendor/progress/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/__init__.py
+Filename: venv/Lib/site-packages/pip/_vendor/progress/bar.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py
+Filename: venv/Lib/site-packages/pip/_vendor/progress/counter.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py
+Filename: venv/Lib/site-packages/pip/_vendor/progress/helpers.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/__init__.py
+Filename: venv/Lib/site-packages/pip/_vendor/progress/spinner.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/certifi/core.py
+Filename: venv/Lib/site-packages/pip/_vendor/pytoml/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/certifi/__init__.py
+Filename: venv/Lib/site-packages/pip/_vendor/pytoml/core.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/certifi/__main__.py
+Filename: venv/Lib/site-packages/pip/_vendor/pytoml/parser.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/cli/
+Filename: venv/Lib/site-packages/pip/_vendor/pytoml/writer.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/big5freq.py
+Filename: venv/Lib/site-packages/pip/_vendor/requests/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/big5prober.py
+Filename: venv/Lib/site-packages/pip/_vendor/requests/__version__.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/chardistribution.py
+Filename: venv/Lib/site-packages/pip/_vendor/requests/_internal_utils.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/charsetgroupprober.py
+Filename: venv/Lib/site-packages/pip/_vendor/requests/adapters.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/charsetprober.py
+Filename: venv/Lib/site-packages/pip/_vendor/requests/api.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/codingstatemachine.py
+Filename: venv/Lib/site-packages/pip/_vendor/requests/auth.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/compat.py
+Filename: venv/Lib/site-packages/pip/_vendor/requests/certs.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/cp949prober.py
+Filename: venv/Lib/site-packages/pip/_vendor/requests/compat.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/enums.py
+Filename: venv/Lib/site-packages/pip/_vendor/requests/cookies.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/escprober.py
+Filename: venv/Lib/site-packages/pip/_vendor/requests/exceptions.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/escsm.py
+Filename: venv/Lib/site-packages/pip/_vendor/requests/help.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/eucjpprober.py
+Filename: venv/Lib/site-packages/pip/_vendor/requests/hooks.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/euckrfreq.py
+Filename: venv/Lib/site-packages/pip/_vendor/requests/models.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/euckrprober.py
+Filename: venv/Lib/site-packages/pip/_vendor/requests/packages.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/euctwfreq.py
+Filename: venv/Lib/site-packages/pip/_vendor/requests/sessions.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/euctwprober.py
+Filename: venv/Lib/site-packages/pip/_vendor/requests/status_codes.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/gb2312freq.py
+Filename: venv/Lib/site-packages/pip/_vendor/requests/structures.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/gb2312prober.py
+Filename: venv/Lib/site-packages/pip/_vendor/requests/utils.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/hebrewprober.py
+Filename: venv/Lib/site-packages/pip/_vendor/urllib3/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/jisfreq.py
+Filename: venv/Lib/site-packages/pip/_vendor/urllib3/_collections.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/jpcntx.py
+Filename: venv/Lib/site-packages/pip/_vendor/urllib3/connection.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/langbulgarianmodel.py
+Filename: venv/Lib/site-packages/pip/_vendor/urllib3/connectionpool.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/langcyrillicmodel.py
+Filename: venv/Lib/site-packages/pip/_vendor/urllib3/exceptions.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/langgreekmodel.py
+Filename: venv/Lib/site-packages/pip/_vendor/urllib3/fields.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/langhebrewmodel.py
+Filename: venv/Lib/site-packages/pip/_vendor/urllib3/filepost.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/langhungarianmodel.py
+Filename: venv/Lib/site-packages/pip/_vendor/urllib3/poolmanager.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/langthaimodel.py
+Filename: venv/Lib/site-packages/pip/_vendor/urllib3/request.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/langturkishmodel.py
+Filename: venv/Lib/site-packages/pip/_vendor/urllib3/response.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/latin1prober.py
+Filename: venv/Lib/site-packages/pip/_vendor/urllib3/contrib/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/mbcharsetprober.py
+Filename: venv/Lib/site-packages/pip/_vendor/urllib3/contrib/appengine.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/mbcsgroupprober.py
+Filename: venv/Lib/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/mbcssm.py
+Filename: venv/Lib/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/sbcharsetprober.py
+Filename: venv/Lib/site-packages/pip/_vendor/urllib3/contrib/securetransport.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/sbcsgroupprober.py
+Filename: venv/Lib/site-packages/pip/_vendor/urllib3/contrib/socks.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/sjisprober.py
+Filename: venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/universaldetector.py
+Filename: venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/utf8prober.py
+Filename: venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/version.py
+Filename: venv/Lib/site-packages/pip/_vendor/urllib3/packages/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/__init__.py
+Filename: venv/Lib/site-packages/pip/_vendor/urllib3/packages/ordered_dict.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/cli/chardetect.py
+Filename: venv/Lib/site-packages/pip/_vendor/urllib3/packages/six.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/cli/__init__.py
+Filename: venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/colorama/ansi.py
+Filename: venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/colorama/ansitowin32.py
+Filename: venv/Lib/site-packages/pip/_vendor/urllib3/packages/ssl_match_hostname/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/colorama/initialise.py
+Filename: venv/Lib/site-packages/pip/_vendor/urllib3/packages/ssl_match_hostname/_implementation.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/colorama/win32.py
+Filename: venv/Lib/site-packages/pip/_vendor/urllib3/util/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/colorama/winterm.py
+Filename: venv/Lib/site-packages/pip/_vendor/urllib3/util/connection.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/colorama/__init__.py
+Filename: venv/Lib/site-packages/pip/_vendor/urllib3/util/request.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/distlib/_backport/
+Filename: venv/Lib/site-packages/pip/_vendor/urllib3/util/response.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/distlib/compat.py
+Filename: venv/Lib/site-packages/pip/_vendor/urllib3/util/retry.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/distlib/database.py
+Filename: venv/Lib/site-packages/pip/_vendor/urllib3/util/selectors.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/distlib/index.py
+Filename: venv/Lib/site-packages/pip/_vendor/urllib3/util/ssl_.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/distlib/locators.py
+Filename: venv/Lib/site-packages/pip/_vendor/urllib3/util/timeout.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/distlib/manifest.py
+Filename: venv/Lib/site-packages/pip/_vendor/urllib3/util/url.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/distlib/markers.py
+Filename: venv/Lib/site-packages/pip/_vendor/urllib3/util/wait.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/distlib/metadata.py
+Filename: venv/Lib/site-packages/pip/_vendor/webencodings/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/distlib/resources.py
+Filename: venv/Lib/site-packages/pip/_vendor/webencodings/labels.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/distlib/scripts.py
+Filename: venv/Lib/site-packages/pip/_vendor/webencodings/mklabels.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/distlib/util.py
+Filename: venv/Lib/site-packages/pip/_vendor/webencodings/tests.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/distlib/version.py
+Filename: venv/Lib/site-packages/pip/_vendor/webencodings/x_user_defined.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/distlib/wheel.py
+Filename: venv/Lib/site-packages/pkg_resources/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/distlib/__init__.py
+Filename: venv/Lib/site-packages/pkg_resources/py31compat.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/distlib/_backport/misc.py
+Filename: venv/Lib/site-packages/pkg_resources/_vendor/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/distlib/_backport/shutil.py
+Filename: venv/Lib/site-packages/pkg_resources/_vendor/appdirs.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/distlib/_backport/sysconfig.py
+Filename: venv/Lib/site-packages/pkg_resources/_vendor/pyparsing.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/distlib/_backport/tarfile.py
+Filename: venv/Lib/site-packages/pkg_resources/_vendor/six.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/distlib/_backport/__init__.py
+Filename: venv/Lib/site-packages/pkg_resources/_vendor/packaging/__about__.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/filters/
+Filename: venv/Lib/site-packages/pkg_resources/_vendor/packaging/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/treeadapters/
+Filename: venv/Lib/site-packages/pkg_resources/_vendor/packaging/_compat.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/treebuilders/
+Filename: venv/Lib/site-packages/pkg_resources/_vendor/packaging/_structures.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/treewalkers/
+Filename: venv/Lib/site-packages/pkg_resources/_vendor/packaging/markers.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/_trie/
+Filename: venv/Lib/site-packages/pkg_resources/_vendor/packaging/requirements.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/constants.py
+Filename: venv/Lib/site-packages/pkg_resources/_vendor/packaging/specifiers.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/html5parser.py
+Filename: venv/Lib/site-packages/pkg_resources/_vendor/packaging/utils.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/serializer.py
+Filename: venv/Lib/site-packages/pkg_resources/_vendor/packaging/version.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/_ihatexml.py
+Filename: venv/Lib/site-packages/pkg_resources/extern/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/_inputstream.py
+Filename: venv/Lib/site-packages/setuptools/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/_tokenizer.py
+Filename: venv/Lib/site-packages/setuptools/archive_util.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/_utils.py
+Filename: venv/Lib/site-packages/setuptools/build_meta.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/__init__.py
+Filename: venv/Lib/site-packages/setuptools/config.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/filters/alphabeticalattributes.py
+Filename: venv/Lib/site-packages/setuptools/dep_util.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/filters/base.py
+Filename: venv/Lib/site-packages/setuptools/depends.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/filters/inject_meta_charset.py
+Filename: venv/Lib/site-packages/setuptools/dist.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/filters/lint.py
+Filename: venv/Lib/site-packages/setuptools/extension.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/filters/optionaltags.py
+Filename: venv/Lib/site-packages/setuptools/glibc.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/filters/sanitizer.py
+Filename: venv/Lib/site-packages/setuptools/glob.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/filters/whitespace.py
+Filename: venv/Lib/site-packages/setuptools/launch.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/filters/__init__.py
+Filename: venv/Lib/site-packages/setuptools/lib2to3_ex.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/treeadapters/genshi.py
+Filename: venv/Lib/site-packages/setuptools/monkey.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/treeadapters/sax.py
+Filename: venv/Lib/site-packages/setuptools/msvc.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/treeadapters/__init__.py
+Filename: venv/Lib/site-packages/setuptools/namespaces.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/treebuilders/base.py
+Filename: venv/Lib/site-packages/setuptools/package_index.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/treebuilders/dom.py
+Filename: venv/Lib/site-packages/setuptools/pep425tags.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/treebuilders/etree.py
+Filename: venv/Lib/site-packages/setuptools/py27compat.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/treebuilders/etree_lxml.py
+Filename: venv/Lib/site-packages/setuptools/py31compat.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/treebuilders/__init__.py
+Filename: venv/Lib/site-packages/setuptools/py33compat.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/treewalkers/base.py
+Filename: venv/Lib/site-packages/setuptools/py36compat.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/treewalkers/dom.py
+Filename: venv/Lib/site-packages/setuptools/sandbox.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/treewalkers/etree.py
+Filename: venv/Lib/site-packages/setuptools/site-patch.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/treewalkers/etree_lxml.py
+Filename: venv/Lib/site-packages/setuptools/ssl_support.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/treewalkers/genshi.py
+Filename: venv/Lib/site-packages/setuptools/unicode_utils.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/treewalkers/__init__.py
+Filename: venv/Lib/site-packages/setuptools/version.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/_trie/datrie.py
+Filename: venv/Lib/site-packages/setuptools/wheel.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/_trie/py.py
+Filename: venv/Lib/site-packages/setuptools/windows_support.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/_trie/_base.py
+Filename: venv/Lib/site-packages/setuptools/_vendor/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/_trie/__init__.py
+Filename: venv/Lib/site-packages/setuptools/_vendor/pyparsing.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/idna/codec.py
+Filename: venv/Lib/site-packages/setuptools/_vendor/six.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/idna/compat.py
+Filename: venv/Lib/site-packages/setuptools/_vendor/packaging/__about__.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/idna/core.py
+Filename: venv/Lib/site-packages/setuptools/_vendor/packaging/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/idna/idnadata.py
+Filename: venv/Lib/site-packages/setuptools/_vendor/packaging/_compat.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/idna/intranges.py
+Filename: venv/Lib/site-packages/setuptools/_vendor/packaging/_structures.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/idna/package_data.py
+Filename: venv/Lib/site-packages/setuptools/_vendor/packaging/markers.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/idna/uts46data.py
+Filename: venv/Lib/site-packages/setuptools/_vendor/packaging/requirements.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/idna/__init__.py
+Filename: venv/Lib/site-packages/setuptools/_vendor/packaging/specifiers.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/lockfile/linklockfile.py
+Filename: venv/Lib/site-packages/setuptools/_vendor/packaging/utils.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/lockfile/mkdirlockfile.py
+Filename: venv/Lib/site-packages/setuptools/_vendor/packaging/version.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/lockfile/pidlockfile.py
+Filename: venv/Lib/site-packages/setuptools/command/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/lockfile/sqlitelockfile.py
+Filename: venv/Lib/site-packages/setuptools/command/alias.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/lockfile/symlinklockfile.py
+Filename: venv/Lib/site-packages/setuptools/command/bdist_egg.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/lockfile/__init__.py
+Filename: venv/Lib/site-packages/setuptools/command/bdist_rpm.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/msgpack/exceptions.py
+Filename: venv/Lib/site-packages/setuptools/command/bdist_wininst.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/msgpack/fallback.py
+Filename: venv/Lib/site-packages/setuptools/command/build_clib.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/msgpack/_version.py
+Filename: venv/Lib/site-packages/setuptools/command/build_ext.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/msgpack/__init__.py
+Filename: venv/Lib/site-packages/setuptools/command/build_py.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/packaging/markers.py
+Filename: venv/Lib/site-packages/setuptools/command/develop.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/packaging/requirements.py
+Filename: venv/Lib/site-packages/setuptools/command/dist_info.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/packaging/specifiers.py
+Filename: venv/Lib/site-packages/setuptools/command/easy_install.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/packaging/utils.py
+Filename: venv/Lib/site-packages/setuptools/command/egg_info.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/packaging/version.py
+Filename: venv/Lib/site-packages/setuptools/command/install.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/packaging/_compat.py
+Filename: venv/Lib/site-packages/setuptools/command/install_egg_info.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/packaging/_structures.py
+Filename: venv/Lib/site-packages/setuptools/command/install_lib.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/packaging/__about__.py
+Filename: venv/Lib/site-packages/setuptools/command/install_scripts.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/packaging/__init__.py
+Filename: venv/Lib/site-packages/setuptools/command/py36compat.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/pkg_resources/py31compat.py
+Filename: venv/Lib/site-packages/setuptools/command/register.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/pkg_resources/__init__.py
+Filename: venv/Lib/site-packages/setuptools/command/rotate.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/progress/bar.py
+Filename: venv/Lib/site-packages/setuptools/command/saveopts.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/progress/counter.py
+Filename: venv/Lib/site-packages/setuptools/command/sdist.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/progress/helpers.py
+Filename: venv/Lib/site-packages/setuptools/command/setopt.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/progress/spinner.py
+Filename: venv/Lib/site-packages/setuptools/command/test.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/progress/__init__.py
+Filename: venv/Lib/site-packages/setuptools/command/upload.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/pytoml/core.py
+Filename: venv/Lib/site-packages/setuptools/command/upload_docs.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/pytoml/parser.py
+Filename: venv/Lib/site-packages/setuptools/extern/__init__.py
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/pytoml/writer.py
+Filename: p0_script-1.1.0.dist-info/LICENSE.rst
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/pytoml/__init__.py
+Filename: p0_script-1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/requests/adapters.py
+Filename: p0_script-1.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/requests/api.py
+Filename: p0_script-1.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/requests/auth.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/requests/certs.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/requests/compat.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/requests/cookies.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/requests/exceptions.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/requests/help.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/requests/hooks.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/requests/models.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/requests/packages.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/requests/sessions.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/requests/status_codes.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/requests/structures.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/requests/utils.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/requests/_internal_utils.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/requests/__init__.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/requests/__version__.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/packages/
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/connection.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/connectionpool.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/exceptions.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/fields.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/filepost.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/poolmanager.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/request.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/response.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/_collections.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/__init__.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/appengine.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/securetransport.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/socks.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/__init__.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/packages/ssl_match_hostname/
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/packages/ordered_dict.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/packages/six.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/packages/__init__.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/__init__.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/packages/ssl_match_hostname/_implementation.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/packages/ssl_match_hostname/__init__.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/connection.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/request.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/response.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/retry.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/selectors.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/ssl_.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/timeout.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/url.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/wait.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/__init__.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/webencodings/labels.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/webencodings/mklabels.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/webencodings/tests.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/webencodings/x_user_defined.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/webencodings/__init__.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pkg_resources/extern/
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pkg_resources/_vendor/
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pkg_resources/py31compat.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pkg_resources/__init__.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pkg_resources/extern/__init__.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pkg_resources/_vendor/packaging/
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pkg_resources/_vendor/appdirs.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pkg_resources/_vendor/six.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pkg_resources/_vendor/__init__.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pkg_resources/_vendor/packaging/markers.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pkg_resources/_vendor/packaging/requirements.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pkg_resources/_vendor/packaging/specifiers.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pkg_resources/_vendor/packaging/utils.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pkg_resources/_vendor/packaging/version.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_compat.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_structures.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pkg_resources/_vendor/packaging/__about__.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/pkg_resources/_vendor/packaging/__init__.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/setuptools/command/
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/setuptools/extern/
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/setuptools/_vendor/
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/setuptools/archive_util.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/setuptools/build_meta.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/setuptools/config.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/setuptools/depends.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/setuptools/dep_util.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/setuptools/dist.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/setuptools/extension.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/setuptools/glibc.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/setuptools/glob.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/setuptools/launch.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/setuptools/lib2to3_ex.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/setuptools/monkey.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/setuptools/msvc.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/setuptools/namespaces.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/setuptools/package_index.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/setuptools/pep425tags.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/setuptools/py27compat.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/setuptools/py31compat.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/setuptools/py33compat.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/setuptools/py36compat.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/setuptools/sandbox.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/setuptools/site-patch.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/setuptools/ssl_support.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/setuptools/unicode_utils.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/setuptools/version.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/setuptools/wheel.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/setuptools/windows_support.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/setuptools/__init__.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/setuptools/command/alias.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/setuptools/command/bdist_egg.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/setuptools/command/bdist_rpm.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/setuptools/command/bdist_wininst.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/setuptools/command/build_clib.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/setuptools/command/build_ext.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/setuptools/command/build_py.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/setuptools/command/develop.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/setuptools/command/dist_info.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/setuptools/command/easy_install.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/setuptools/command/egg_info.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/setuptools/command/install.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/setuptools/command/install_egg_info.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/setuptools/command/install_lib.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/setuptools/command/install_scripts.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/setuptools/command/py36compat.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/setuptools/command/register.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/setuptools/command/rotate.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/setuptools/command/saveopts.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/setuptools/command/sdist.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/setuptools/command/setopt.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/setuptools/command/test.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/setuptools/command/upload.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/setuptools/command/upload_docs.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/setuptools/command/__init__.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/setuptools/extern/__init__.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/setuptools/_vendor/packaging/
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/setuptools/_vendor/pyparsing.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/setuptools/_vendor/six.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/setuptools/_vendor/__init__.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/setuptools/_vendor/packaging/markers.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/setuptools/_vendor/packaging/requirements.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/setuptools/_vendor/packaging/specifiers.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/setuptools/_vendor/packaging/utils.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/setuptools/_vendor/packaging/version.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/setuptools/_vendor/packaging/_compat.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/setuptools/_vendor/packaging/_structures.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/setuptools/_vendor/packaging/__about__.py
-Comment: 
-
-Filename: p0-script-1.0.2/venv/Lib/site-packages/setuptools/_vendor/packaging/__init__.py
+Filename: p0_script-1.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=store
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## Comparing `p0-script-1.0.2/LICENSE.rst` & `p0_script-1.1.0.dist-info/LICENSE.rst`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/PKG-INFO` & `p0_script-1.1.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: p0-script
-Version: 1.0.2
+Version: 1.1.0
 Summary: Protocol0 ableton remote script
 Author-email: Thibault Lebrun <thibaultlebrun@live.fr>
 License: MIT License
         
         Copyright (c) 2023 Thibault Lebrun
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -29,16 +29,20 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 License-File: LICENSE.rst
+Provides-Extra: dev
+Requires-Dist: flake8 (==6.0.0) ; extra == 'dev'
+Requires-Dist: pytest (==7.3.1) ; extra == 'dev'
+Requires-Dist: qualname (==0.1.0) ; extra == 'dev'
+Requires-Dist: vulture (==2.7) ; extra == 'dev'
 
 # Protocol0 Control Surface Script for Ableton
 
 Protocol0 is a control surface script for Ableton Live (tested on 11 and 10)
 
 It is a "selected track control" like
 script focused on working in session view.
```

## Comparing `p0-script-1.0.2/application/CommandBus.py` & `application/CommandBus.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/application/CommandBusHistory.py` & `application/CommandBusHistory.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/application/Container.py` & `application/Container.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/application/main.py` & `application/main.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/application/Protocol0.py` & `application/Protocol0.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/application/Protocol0Midi.py` & `application/Protocol0Midi.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/application/command/ScrollScenePositionCommand.py` & `application/command/ScrollScenePositionCommand.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/application/command/SerializableCommand.py` & `application/command/SerializableCommand.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/application/command_handler/CheckAudioExportValidCommandHandler.py` & `application/command_handler/CheckAudioExportValidCommandHandler.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/application/command_handler/EmitBackendEventCommandHandler.py` & `application/command_handler/EmitBackendEventCommandHandler.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/application/command_handler/FireSceneToPositionCommandHandler.py` & `application/command_handler/FireSceneToPositionCommandHandler.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/application/command_handler/LoadDrumRackCommandHandler.py` & `application/command_handler/LoadDrumRackCommandHandler.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/application/command_handler/LoadMinitaurCommandHandler.py` & `application/command_handler/LoadMinitaurCommandHandler.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/application/command_handler/MidiNoteCommandHandler.py` & `application/command_handler/MidiNoteCommandHandler.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/application/command_handler/RecordUnlimitedCommandHandler.py` & `application/command_handler/RecordUnlimitedCommandHandler.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/application/command_handler/ReloadScriptCommandHandler.py` & `application/command_handler/ReloadScriptCommandHandler.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/application/command_handler/ScrollScenePositionCommandHandler.py` & `application/command_handler/ScrollScenePositionCommandHandler.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/application/command_handler/SelectOrLoadDeviceCommandHandler.py` & `application/command_handler/SelectOrLoadDeviceCommandHandler.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/application/command_handler/SelectTrackCommandHandler.py` & `application/command_handler/SelectTrackCommandHandler.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/application/command_handler/ShowInstrumentCommandHandler.py` & `application/command_handler/ShowInstrumentCommandHandler.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/application/control_surface/ActionGroupFactory.py` & `application/control_surface/ActionGroupFactory.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/application/control_surface/ActionGroupInterface.py` & `application/control_surface/ActionGroupInterface.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/application/control_surface/EncoderAction.py` & `application/control_surface/EncoderAction.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/application/control_surface/MultiEncoder.py` & `application/control_surface/MultiEncoder.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/application/control_surface/group/ActionGroupClip.py` & `application/control_surface/group/ActionGroupClip.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/application/control_surface/group/ActionGroupCut.py` & `application/control_surface/group/ActionGroupCut.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/application/control_surface/group/ActionGroupFix.py` & `application/control_surface/group/ActionGroupFix.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/application/control_surface/group/ActionGroupLog.py` & `application/control_surface/group/ActionGroupLog.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/application/control_surface/group/ActionGroupMain.py` & `application/control_surface/group/ActionGroupMain.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/application/control_surface/group/ActionGroupSample.py` & `application/control_surface/group/ActionGroupSample.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/application/control_surface/group/ActionGroupSet.py` & `application/control_surface/group/ActionGroupSet.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/application/control_surface/group/ActionGroupTest.py` & `application/control_surface/group/ActionGroupTest.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/application/control_surface/group/legacy/ActionGroupPreset.py` & `application/control_surface/group/legacy/ActionGroupPreset.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/application/error/ErrorService.py` & `application/error/ErrorService.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/application/push2/P0Push2.py` & `application/push2/P0Push2.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/application/push2/P0SessionRingTrackProvider.py` & `application/push2/P0SessionRingTrackProvider.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/application/push2/P0ShowInstrumentMode.py` & `application/push2/P0ShowInstrumentMode.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/application/push2/P0TrackListComponent.py` & `application/push2/P0TrackListComponent.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/audit/AudioLatencyAnalyzerService.py` & `domain/audit/AudioLatencyAnalyzerService.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/audit/LogService.py` & `domain/audit/LogService.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/audit/LOMAnalyzerService.py` & `domain/audit/LOMAnalyzerService.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/audit/SetFixerService.py` & `domain/audit/SetFixerService.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/audit/SetUpgradeService.py` & `domain/audit/SetUpgradeService.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/audit/stats/ClipStats.py` & `domain/audit/stats/ClipStats.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/audit/stats/DeviceStats.py` & `domain/audit/stats/DeviceStats.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/audit/stats/SampleStats.py` & `domain/audit/stats/SampleStats.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/audit/stats/SceneStats.py` & `domain/audit/stats/SceneStats.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/audit/stats/SongStats.py` & `domain/audit/stats/SongStats.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/audit/stats/TrackStats.py` & `domain/audit/stats/TrackStats.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/clip/AudioClip.py` & `domain/lom/clip/AudioClip.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/clip/Clip.py` & `domain/lom/clip/Clip.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/clip/ClipAppearance.py` & `domain/lom/clip/ClipAppearance.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/clip/ClipInfo.py` & `domain/lom/clip/ClipInfo.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/clip/ClipLoop.py` & `domain/lom/clip/ClipLoop.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/clip/ClipName.py` & `domain/lom/clip/ClipName.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/clip/ClipPlayingPosition.py` & `domain/lom/clip/ClipPlayingPosition.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/clip/ClipTail.py` & `domain/lom/clip/ClipTail.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/clip/MidiClip.py` & `domain/lom/clip/MidiClip.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/clip/automation/ClipAutomation.py` & `domain/lom/clip/automation/ClipAutomation.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/clip/automation/ClipAutomationEnvelope.py` & `domain/lom/clip/automation/ClipAutomationEnvelope.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/clip_slot/AudioClipSlot.py` & `domain/lom/clip_slot/AudioClipSlot.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/clip_slot/ClipSlot.py` & `domain/lom/clip_slot/ClipSlot.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/clip_slot/ClipSlotAppearance.py` & `domain/lom/clip_slot/ClipSlotAppearance.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/device/Device.py` & `domain/lom/device/Device.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/device/DeviceChain.py` & `domain/lom/device/DeviceChain.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/device/DeviceDisplayService.py` & `domain/lom/device/DeviceDisplayService.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/device/DeviceEnum.py` & `domain/lom/device/DeviceEnum.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/device/DeviceEnumGroup.py` & `domain/lom/device/DeviceEnumGroup.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/device/DeviceService.py` & `domain/lom/device/DeviceService.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/device/DrumPad.py` & `domain/lom/device/DrumPad.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/device/DrumRackDevice.py` & `domain/lom/device/DrumRackDevice.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/device/DrumRackSampleService.py` & `domain/lom/device/DrumRackSampleService.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/device/DrumRackService.py` & `domain/lom/device/DrumRackService.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/device/MixerDevice.py` & `domain/lom/device/MixerDevice.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/device/PluginDevice.py` & `domain/lom/device/PluginDevice.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/device/RackDevice.py` & `domain/lom/device/RackDevice.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/device/SimplerDevice.py` & `domain/lom/device/SimplerDevice.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/device/SimpleTrackDevices.py` & `domain/lom/device/SimpleTrackDevices.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/device/Sample/Sample.py` & `domain/lom/device/Sample/Sample.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/device_parameter/DeviceParameter.py` & `domain/lom/device_parameter/DeviceParameter.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/device_parameter/DeviceParameterEnum.py` & `domain/lom/device_parameter/DeviceParameterEnum.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/device_parameter/DeviceParameterValue.py` & `domain/lom/device_parameter/DeviceParameterValue.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/device_parameter/LinkedDeviceParameters.py` & `domain/lom/device_parameter/LinkedDeviceParameters.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/instrument/InstrumentDisplayService.py` & `domain/lom/instrument/InstrumentDisplayService.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/instrument/InstrumentFactory.py` & `domain/lom/instrument/InstrumentFactory.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/instrument/InstrumentInterface.py` & `domain/lom/instrument/InstrumentInterface.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/instrument/instrument/InstrumentAddictiveKeys.py` & `domain/lom/instrument/instrument/InstrumentAddictiveKeys.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/instrument/instrument/InstrumentMinitaur.py` & `domain/lom/instrument/instrument/InstrumentMinitaur.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/instrument/instrument/InstrumentRev2.py` & `domain/lom/instrument/instrument/InstrumentRev2.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/instrument/instrument/InstrumentSimpler.py` & `domain/lom/instrument/instrument/InstrumentSimpler.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/instrument/preset/InstrumentPreset.py` & `domain/lom/instrument/preset/InstrumentPreset.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/instrument/preset/InstrumentPresetList.py` & `domain/lom/instrument/preset/InstrumentPresetList.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/instrument/preset/InstrumentPresetScrollerService.py` & `domain/lom/instrument/preset/InstrumentPresetScrollerService.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/instrument/preset/preset_changer/InstrumentRackPresetChanger.py` & `domain/lom/instrument/preset/preset_changer/InstrumentRackPresetChanger.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/instrument/preset/preset_changer/ProgramChangePresetChanger.py` & `domain/lom/instrument/preset/preset_changer/ProgramChangePresetChanger.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/instrument/preset/preset_changer/SamplePresetChanger.py` & `domain/lom/instrument/preset/preset_changer/SamplePresetChanger.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/instrument/preset/preset_importer/DirectoryPresetImporter.py` & `domain/lom/instrument/preset/preset_importer/DirectoryPresetImporter.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/instrument/preset/preset_importer/FilePresetImporter.py` & `domain/lom/instrument/preset/preset_importer/FilePresetImporter.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/instrument/preset/preset_importer/PluginDevicePresetImporter.py` & `domain/lom/instrument/preset/preset_importer/PluginDevicePresetImporter.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/instrument/preset/preset_importer/PresetImporterFactory.py` & `domain/lom/instrument/preset/preset_importer/PresetImporterFactory.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/instrument/preset/preset_importer/PresetImportInterface.py` & `domain/lom/instrument/preset/preset_importer/PresetImportInterface.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/instrument/preset/preset_importer/RackDevicePresetImporter.py` & `domain/lom/instrument/preset/preset_importer/RackDevicePresetImporter.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/instrument/preset/preset_initializer/PresetInitializerDevicePresetName.py` & `domain/lom/instrument/preset/preset_initializer/PresetInitializerDevicePresetName.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/instrument/preset/preset_initializer/PresetInitializerGroupTrackName.py` & `domain/lom/instrument/preset/preset_initializer/PresetInitializerGroupTrackName.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/instrument/preset/preset_initializer/PresetInitializerInterface.py` & `domain/lom/instrument/preset/preset_initializer/PresetInitializerInterface.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/loop/LoopableInterface.py` & `domain/lom/loop/LoopableInterface.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/note/Note.py` & `domain/lom/note/Note.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/sample/SampleCategory.py` & `domain/lom/sample/SampleCategory.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/sample/SampleCategoryEnum.py` & `domain/lom/sample/SampleCategoryEnum.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/scene/LoopingSceneToggler.py` & `domain/lom/scene/LoopingSceneToggler.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/scene/PlayingSceneFacade.py` & `domain/lom/scene/PlayingSceneFacade.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/scene/Scene.py` & `domain/lom/scene/Scene.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/scene/SceneAppearance.py` & `domain/lom/scene/SceneAppearance.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/scene/SceneClips.py` & `domain/lom/scene/SceneClips.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/scene/SceneCropScroller.py` & `domain/lom/scene/SceneCropScroller.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/scene/SceneLength.py` & `domain/lom/scene/SceneLength.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/scene/SceneName.py` & `domain/lom/scene/SceneName.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/scene/ScenePlaybackService.py` & `domain/lom/scene/ScenePlaybackService.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/scene/ScenePlayingState.py` & `domain/lom/scene/ScenePlayingState.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/scene/ScenePositionScroller.py` & `domain/lom/scene/ScenePositionScroller.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/scene/SceneService.py` & `domain/lom/scene/SceneService.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/scene/SceneWindow.py` & `domain/lom/scene/SceneWindow.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/set/AbletonSet.py` & `domain/lom/set/AbletonSet.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/set/SessionToArrangementService.py` & `domain/lom/set/SessionToArrangementService.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/song/SongInitService.py` & `domain/lom/song/SongInitService.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/song/components/ClipComponent.py` & `domain/lom/song/components/ClipComponent.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/song/components/DeviceComponent.py` & `domain/lom/song/components/DeviceComponent.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/song/components/PlaybackComponent.py` & `domain/lom/song/components/PlaybackComponent.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/song/components/QuantizationComponent.py` & `domain/lom/song/components/QuantizationComponent.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/song/components/RecordingComponent.py` & `domain/lom/song/components/RecordingComponent.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/song/components/SceneComponent.py` & `domain/lom/song/components/SceneComponent.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/song/components/SceneCrudComponent.py` & `domain/lom/song/components/SceneCrudComponent.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/song/components/TempoComponent.py` & `domain/lom/song/components/TempoComponent.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/song/components/TrackComponent.py` & `domain/lom/song/components/TrackComponent.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/song/components/TrackCrudComponent.py` & `domain/lom/song/components/TrackCrudComponent.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/track/TrackAutomationService.py` & `domain/lom/track/TrackAutomationService.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/track/TrackFactory.py` & `domain/lom/track/TrackFactory.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/track/TrackMapperService.py` & `domain/lom/track/TrackMapperService.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/track/TrackService.py` & `domain/lom/track/TrackService.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/track/abstract_track/AbstrackTrackArmState.py` & `domain/lom/track/abstract_track/AbstrackTrackArmState.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/track/abstract_track/AbstractTrack.py` & `domain/lom/track/abstract_track/AbstractTrack.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/track/abstract_track/AbstractTrackAppearance.py` & `domain/lom/track/abstract_track/AbstractTrackAppearance.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/track/group_track/AbstractGroupTrack.py` & `domain/lom/track/group_track/AbstractGroupTrack.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/track/group_track/NormalGroupMatchingTrack.py` & `domain/lom/track/group_track/NormalGroupMatchingTrack.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/track/group_track/NormalGroupMatchingTrackCreator.py` & `domain/lom/track/group_track/NormalGroupMatchingTrackCreator.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/track/group_track/NormalGroupTrack.py` & `domain/lom/track/group_track/NormalGroupTrack.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/track/group_track/ext_track/ExtArmState.py` & `domain/lom/track/group_track/ext_track/ExtArmState.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/track/group_track/ext_track/ExternalSynthTrack.py` & `domain/lom/track/group_track/ext_track/ExternalSynthTrack.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/track/group_track/ext_track/ExtMatchingTrack.py` & `domain/lom/track/group_track/ext_track/ExtMatchingTrack.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/track/group_track/ext_track/ExtMatchingTrackCreator.py` & `domain/lom/track/group_track/ext_track/ExtMatchingTrackCreator.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/track/group_track/ext_track/ExtMonitoringState.py` & `domain/lom/track/group_track/ext_track/ExtMonitoringState.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/track/group_track/ext_track/ExtSoloState.py` & `domain/lom/track/group_track/ext_track/ExtSoloState.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/track/group_track/ext_track/SimpleAudioExtTrack.py` & `domain/lom/track/group_track/ext_track/SimpleAudioExtTrack.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/track/group_track/ext_track/SimpleBaseExtTrack.py` & `domain/lom/track/group_track/ext_track/SimpleBaseExtTrack.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/track/group_track/ext_track/SimpleMidiExtTrack.py` & `domain/lom/track/group_track/ext_track/SimpleMidiExtTrack.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/track/group_track/matching_track/MatchingTrackClipColorManager.py` & `domain/lom/track/group_track/matching_track/MatchingTrackClipColorManager.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/track/group_track/matching_track/MatchingTrackClipManager.py` & `domain/lom/track/group_track/matching_track/MatchingTrackClipManager.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/track/group_track/matching_track/MatchingTrackCreatorInterface.py` & `domain/lom/track/group_track/matching_track/MatchingTrackCreatorInterface.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/track/group_track/matching_track/MatchingTrackInterface.py` & `domain/lom/track/group_track/matching_track/MatchingTrackInterface.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/track/group_track/matching_track/MatchingTrackRouter.py` & `domain/lom/track/group_track/matching_track/MatchingTrackRouter.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/track/group_track/matching_track/MatchingTrackService.py` & `domain/lom/track/group_track/matching_track/MatchingTrackService.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/track/group_track/matching_track/MatchingTrackSoloState.py` & `domain/lom/track/group_track/matching_track/MatchingTrackSoloState.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/track/group_track/matching_track/utils.py` & `domain/lom/track/group_track/matching_track/utils.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/track/routing/RoutingDisplayNameDescriptor.py` & `domain/lom/track/routing/RoutingDisplayNameDescriptor.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/track/routing/RoutingTrackDescriptor.py` & `domain/lom/track/routing/RoutingTrackDescriptor.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/track/routing/TrackInputRouting.py` & `domain/lom/track/routing/TrackInputRouting.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/track/routing/TrackOutputRouting.py` & `domain/lom/track/routing/TrackOutputRouting.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/track/simple_track/AudioToMidiClipMapping.py` & `domain/lom/track/simple_track/AudioToMidiClipMapping.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/track/simple_track/SimpleMatchingTrack.py` & `domain/lom/track/simple_track/SimpleMatchingTrack.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/track/simple_track/SimpleMatchingTrackCreator.py` & `domain/lom/track/simple_track/SimpleMatchingTrackCreator.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/track/simple_track/SimpleTrack.py` & `domain/lom/track/simple_track/SimpleTrack.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/track/simple_track/SimpleTrackArmState.py` & `domain/lom/track/simple_track/SimpleTrackArmState.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/track/simple_track/SimpleTrackClipColorManager.py` & `domain/lom/track/simple_track/SimpleTrackClipColorManager.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/track/simple_track/SimpleTrackClips.py` & `domain/lom/track/simple_track/SimpleTrackClips.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/track/simple_track/SimpleTrackClipSlots.py` & `domain/lom/track/simple_track/SimpleTrackClipSlots.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/track/simple_track/SimpleTrackMonitoringState.py` & `domain/lom/track/simple_track/SimpleTrackMonitoringState.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/track/simple_track/SimpleTrackService.py` & `domain/lom/track/simple_track/SimpleTrackService.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/track/simple_track/audio/SimpleAudioTrack.py` & `domain/lom/track/simple_track/audio/SimpleAudioTrack.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/track/simple_track/audio/SimpleReturnTrack.py` & `domain/lom/track/simple_track/audio/SimpleReturnTrack.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/track/simple_track/audio/master/MasterTrack.py` & `domain/lom/track/simple_track/audio/master/MasterTrack.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/track/simple_track/audio/special/ReferenceTrack.py` & `domain/lom/track/simple_track/audio/special/ReferenceTrack.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/track/simple_track/midi/SimpleMidiTrack.py` & `domain/lom/track/simple_track/midi/SimpleMidiTrack.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/track/simple_track/midi/special/UsamoTrack.py` & `domain/lom/track/simple_track/midi/special/UsamoTrack.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/validation/ValidatorFactory.py` & `domain/lom/validation/ValidatorFactory.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/validation/ValidatorInterface.py` & `domain/lom/validation/ValidatorInterface.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/validation/ValidatorService.py` & `domain/lom/validation/ValidatorService.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/validation/object_validators/SceneValidator.py` & `domain/lom/validation/object_validators/SceneValidator.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/validation/object_validators/SimpleAudioTrackValidator.py` & `domain/lom/validation/object_validators/SimpleAudioTrackValidator.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/validation/object_validators/external_synth_track/ExternalSynthTrackValidator.py` & `domain/lom/validation/object_validators/external_synth_track/ExternalSynthTrackValidator.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/validation/object_validators/external_synth_track/SimpleAudioExtTrackValidator.py` & `domain/lom/validation/object_validators/external_synth_track/SimpleAudioExtTrackValidator.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/validation/object_validators/external_synth_track/SimpleMidiExtTrackValidator.py` & `domain/lom/validation/object_validators/external_synth_track/SimpleMidiExtTrackValidator.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/validation/sub_validators/AggregateValidator.py` & `domain/lom/validation/sub_validators/AggregateValidator.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/validation/sub_validators/CallbackValidator.py` & `domain/lom/validation/sub_validators/CallbackValidator.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/validation/sub_validators/DeviceParameterValidator.py` & `domain/lom/validation/sub_validators/DeviceParameterValidator.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/validation/sub_validators/PropertyValueValidator.py` & `domain/lom/validation/sub_validators/PropertyValueValidator.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/lom/validation/sub_validators/SimpleTrackHasDeviceValidator.py` & `domain/lom/validation/sub_validators/SimpleTrackHasDeviceValidator.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/shared/ApplicationView.py` & `domain/shared/ApplicationView.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/shared/BrowserServiceInterface.py` & `domain/shared/BrowserServiceInterface.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/shared/LiveObject.py` & `domain/shared/LiveObject.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/shared/LiveObjectMapping.py` & `domain/shared/LiveObjectMapping.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/shared/ValueScroller.py` & `domain/shared/ValueScroller.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/shared/ValueToggler.py` & `domain/shared/ValueToggler.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/shared/backend/Backend.py` & `domain/shared/backend/Backend.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/shared/errors/error_handler.py` & `domain/shared/errors/error_handler.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/shared/event/DomainEventBus.py` & `domain/shared/event/DomainEventBus.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/shared/scheduler/Scheduler.py` & `domain/shared/scheduler/Scheduler.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/shared/scheduler/TickSchedulerInterface.py` & `domain/shared/scheduler/TickSchedulerInterface.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/shared/utils/concurrency.py` & `domain/shared/utils/concurrency.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/shared/utils/debug.py` & `domain/shared/utils/debug.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/shared/utils/forward_to.py` & `domain/shared/utils/forward_to.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/shared/utils/func.py` & `domain/shared/utils/func.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/shared/utils/string.py` & `domain/shared/utils/string.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/shared/utils/timing.py` & `domain/shared/utils/timing.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/shared/utils/utils.py` & `domain/shared/utils/utils.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/track_recorder/AbstractRecorderFactory.py` & `domain/track_recorder/AbstractRecorderFactory.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/track_recorder/BaseRecorder.py` & `domain/track_recorder/BaseRecorder.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/track_recorder/RecordProcessorInterface.py` & `domain/track_recorder/RecordProcessorInterface.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/track_recorder/RecordService.py` & `domain/track_recorder/RecordService.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/track_recorder/RecordTypeEnum.py` & `domain/track_recorder/RecordTypeEnum.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/track_recorder/config/RecordConfig.py` & `domain/track_recorder/config/RecordConfig.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/track_recorder/config/RecordProcessors.py` & `domain/track_recorder/config/RecordProcessors.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/track_recorder/count_in/CountInOneBar.py` & `domain/track_recorder/count_in/CountInOneBar.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/track_recorder/count_in/CountInShort.py` & `domain/track_recorder/count_in/CountInShort.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/track_recorder/external_synth/OnRecordEndClipTail.py` & `domain/track_recorder/external_synth/OnRecordEndClipTail.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/track_recorder/external_synth/TrackRecorderExternalSynthFactory.py` & `domain/track_recorder/external_synth/TrackRecorderExternalSynthFactory.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/track_recorder/external_synth/record_audio/PostRecordAudio.py` & `domain/track_recorder/external_synth/record_audio/PostRecordAudio.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/track_recorder/external_synth/record_audio/PostRecordAudioFull.py` & `domain/track_recorder/external_synth/record_audio/PostRecordAudioFull.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/track_recorder/external_synth/record_audio/PreRecordAudio.py` & `domain/track_recorder/external_synth/record_audio/PreRecordAudio.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/track_recorder/external_synth/record_audio/record_multi/PreRecordAudioMulti.py` & `domain/track_recorder/external_synth/record_audio/record_multi/PreRecordAudioMulti.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/track_recorder/external_synth/record_audio/record_multi/RecordAudioMulti.py` & `domain/track_recorder/external_synth/record_audio/record_multi/RecordAudioMulti.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/track_recorder/external_synth/record_midi/PostRecordMidi.py` & `domain/track_recorder/external_synth/record_midi/PostRecordMidi.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/track_recorder/recording_bar_length/RecordingBarLengthEnum.py` & `domain/track_recorder/recording_bar_length/RecordingBarLengthEnum.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/track_recorder/recording_bar_length/RecordingBarLengthScroller.py` & `domain/track_recorder/recording_bar_length/RecordingBarLengthScroller.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/track_recorder/simple/PostRecordSimple.py` & `domain/track_recorder/simple/PostRecordSimple.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/domain/track_recorder/simple/RecorderSimpleFactory.py` & `domain/track_recorder/simple/RecorderSimpleFactory.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/infra/interface/BrowserLoaderService.py` & `infra/interface/BrowserLoaderService.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/infra/interface/BrowserService.py` & `infra/interface/BrowserService.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/infra/interface/session/SessionService.py` & `infra/interface/session/SessionService.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/infra/logging/LoggerService.py` & `infra/logging/LoggerService.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/infra/midi/MidiService.py` & `infra/midi/MidiService.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/infra/persistence/SongDataService.py` & `infra/persistence/SongDataService.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/infra/persistence/TrackData.py` & `infra/persistence/TrackData.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/infra/scheduler/BeatScheduler.py` & `infra/scheduler/BeatScheduler.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/infra/scheduler/BeatSchedulerEvent.py` & `infra/scheduler/BeatSchedulerEvent.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/infra/scheduler/BeatTime.py` & `infra/scheduler/BeatTime.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/infra/scheduler/TickScheduler.py` & `infra/scheduler/TickScheduler.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/infra/scheduler/TickSchedulerEvent.py` & `infra/scheduler/TickSchedulerEvent.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/shared/AbstractEnum.py` & `shared/AbstractEnum.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/shared/Config.py` & `shared/Config.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/shared/Song.py` & `shared/Song.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/shared/UndoFacade.py` & `shared/UndoFacade.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/shared/logging/Logger.py` & `shared/logging/Logger.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/shared/logging/StatusBar.py` & `shared/logging/StatusBar.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/shared/observer/Observable.py` & `shared/observer/Observable.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/shared/sequence/HasSequenceState.py` & `shared/sequence/HasSequenceState.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/shared/sequence/ParallelSequence.py` & `shared/sequence/ParallelSequence.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/shared/sequence/Sequence.py` & `shared/sequence/Sequence.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/shared/sequence/SequenceState.py` & `shared/sequence/SequenceState.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/shared/sequence/SequenceStep.py` & `shared/sequence/SequenceStep.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/shared/sequence/SequenceTransition.py` & `shared/sequence/SequenceTransition.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/shared/sequence/TimeoutLimit.py` & `shared/sequence/TimeoutLimit.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/tests/application/test_multi_encoder.py` & `tests/application/test_multi_encoder.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/tests/domain/clip/test_clip_playing_position.py` & `tests/domain/clip/test_clip_playing_position.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/tests/domain/fixtures/clip.py` & `tests/domain/fixtures/clip.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/tests/domain/fixtures/device.py` & `tests/domain/fixtures/device.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/tests/domain/fixtures/group_track.py` & `tests/domain/fixtures/group_track.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/tests/domain/fixtures/p0.py` & `tests/domain/fixtures/p0.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/tests/domain/fixtures/simple_track.py` & `tests/domain/fixtures/simple_track.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/tests/domain/fixtures/song.py` & `tests/domain/fixtures/song.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/tests/domain/scene/test_scene_clips.py` & `tests/domain/scene/test_scene_clips.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/tests/domain/scene/test_scene_length.py` & `tests/domain/scene/test_scene_length.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/tests/domain/scene/test_scene_playing_position.py` & `tests/domain/scene/test_scene_playing_position.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/tests/domain/shared/test_live_object_mapping.py` & `tests/domain/shared/test_live_object_mapping.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/tests/domain/shared/event/test_domain_event_bus.py` & `tests/domain/shared/event/test_domain_event_bus.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/tests/domain/shared/utils/test_func.py` & `tests/domain/shared/utils/test_func.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/tests/domain/shared/utils/test_utils.py` & `tests/domain/shared/utils/test_utils.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/tests/domain/track/test_audio_to_midi_clip_mapping.py` & `tests/domain/track/test_audio_to_midi_clip_mapping.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/tests/domain/track/test_instantiation.py` & `tests/domain/track/test_instantiation.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/tests/domain/validation/test_aggregate_validator.py` & `tests/domain/validation/test_aggregate_validator.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/tests/domain/validation/test_callback_validator.py` & `tests/domain/validation/test_callback_validator.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/tests/domain/validation/test_property_validator.py` & `tests/domain/validation/test_property_validator.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/tests/infra/test_scheduler.py` & `tests/infra/test_scheduler.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/tests/infra/listeners/test_subject_slot.py` & `tests/infra/listeners/test_subject_slot.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/tests/infra/scheduler/TickSchedulerTest.py` & `tests/infra/scheduler/TickSchedulerTest.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/tests/shared/test_container.py` & `tests/shared/test_container.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/tests/shared/sequence/test_sanity_sequence.py` & `tests/shared/sequence/test_sanity_sequence.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/tests/shared/sequence/test_sequence.py` & `tests/shared/sequence/test_sequence.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/tests/shared/sequence/test_sequence_parallel.py` & `tests/shared/sequence/test_sequence_parallel.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/__main__.py` & `venv/Lib/site-packages/pip/__main__.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/basecommand.py` & `venv/Lib/site-packages/pip/_internal/basecommand.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/baseparser.py` & `venv/Lib/site-packages/pip/_internal/baseparser.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/build_env.py` & `venv/Lib/site-packages/pip/_internal/build_env.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/cache.py` & `venv/Lib/site-packages/pip/_internal/cache.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/cmdoptions.py` & `venv/Lib/site-packages/pip/_internal/cmdoptions.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/compat.py` & `venv/Lib/site-packages/pip/_internal/compat.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/configuration.py` & `venv/Lib/site-packages/pip/_internal/configuration.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/download.py` & `venv/Lib/site-packages/pip/_internal/download.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/exceptions.py` & `venv/Lib/site-packages/pip/_internal/exceptions.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/index.py` & `venv/Lib/site-packages/pip/_internal/index.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/locations.py` & `venv/Lib/site-packages/pip/_internal/locations.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/pep425tags.py` & `venv/Lib/site-packages/pip/_internal/pep425tags.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/resolve.py` & `venv/Lib/site-packages/pip/_internal/resolve.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/wheel.py` & `venv/Lib/site-packages/pip/_internal/wheel.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/__init__.py` & `venv/Lib/site-packages/pip/_internal/__init__.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/commands/check.py` & `venv/Lib/site-packages/pip/_internal/commands/check.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/commands/completion.py` & `venv/Lib/site-packages/pip/_internal/commands/completion.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/commands/configuration.py` & `venv/Lib/site-packages/pip/_internal/commands/configuration.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/commands/download.py` & `venv/Lib/site-packages/pip/_internal/commands/download.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/commands/freeze.py` & `venv/Lib/site-packages/pip/_internal/commands/freeze.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/commands/hash.py` & `venv/Lib/site-packages/pip/_internal/commands/hash.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/commands/help.py` & `venv/Lib/site-packages/pip/_internal/commands/help.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/commands/install.py` & `venv/Lib/site-packages/pip/_internal/commands/install.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/commands/list.py` & `venv/Lib/site-packages/pip/_internal/commands/list.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/commands/search.py` & `venv/Lib/site-packages/pip/_internal/commands/search.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/commands/show.py` & `venv/Lib/site-packages/pip/_internal/commands/show.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/commands/uninstall.py` & `venv/Lib/site-packages/pip/_internal/commands/uninstall.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/commands/wheel.py` & `venv/Lib/site-packages/pip/_internal/commands/wheel.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/commands/__init__.py` & `venv/Lib/site-packages/pip/_internal/commands/__init__.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/operations/check.py` & `venv/Lib/site-packages/pip/_internal/operations/check.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/operations/freeze.py` & `venv/Lib/site-packages/pip/_internal/operations/freeze.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/operations/prepare.py` & `venv/Lib/site-packages/pip/_internal/operations/prepare.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/req/req_file.py` & `venv/Lib/site-packages/pip/_internal/req/req_file.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/req/req_install.py` & `venv/Lib/site-packages/pip/_internal/req/req_install.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/req/req_set.py` & `venv/Lib/site-packages/pip/_internal/req/req_set.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/req/req_uninstall.py` & `venv/Lib/site-packages/pip/_internal/req/req_uninstall.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/req/__init__.py` & `venv/Lib/site-packages/pip/_internal/req/__init__.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/utils/appdirs.py` & `venv/Lib/site-packages/pip/_internal/utils/appdirs.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/utils/deprecation.py` & `venv/Lib/site-packages/pip/_internal/utils/deprecation.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/utils/encoding.py` & `venv/Lib/site-packages/pip/_internal/utils/encoding.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/utils/filesystem.py` & `venv/Lib/site-packages/pip/_internal/utils/filesystem.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/utils/glibc.py` & `venv/Lib/site-packages/pip/_internal/utils/glibc.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/utils/hashes.py` & `venv/Lib/site-packages/pip/_internal/utils/hashes.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/utils/logging.py` & `venv/Lib/site-packages/pip/_internal/utils/logging.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/utils/misc.py` & `venv/Lib/site-packages/pip/_internal/utils/misc.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/utils/outdated.py` & `venv/Lib/site-packages/pip/_internal/utils/outdated.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/utils/packaging.py` & `venv/Lib/site-packages/pip/_internal/utils/packaging.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/utils/temp_dir.py` & `venv/Lib/site-packages/pip/_internal/utils/temp_dir.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/utils/typing.py` & `venv/Lib/site-packages/pip/_internal/utils/typing.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/utils/ui.py` & `venv/Lib/site-packages/pip/_internal/utils/ui.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/vcs/bazaar.py` & `venv/Lib/site-packages/pip/_internal/vcs/bazaar.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/vcs/git.py` & `venv/Lib/site-packages/pip/_internal/vcs/git.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/vcs/mercurial.py` & `venv/Lib/site-packages/pip/_internal/vcs/mercurial.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/vcs/subversion.py` & `venv/Lib/site-packages/pip/_internal/vcs/subversion.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_internal/vcs/__init__.py` & `venv/Lib/site-packages/pip/_internal/vcs/__init__.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/appdirs.py` & `venv/Lib/site-packages/pip/_vendor/appdirs.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/distro.py` & `venv/Lib/site-packages/pip/_vendor/distro.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/ipaddress.py` & `venv/Lib/site-packages/pip/_vendor/ipaddress.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/pyparsing.py` & `venv/Lib/site-packages/pip/_vendor/pyparsing.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/retrying.py` & `venv/Lib/site-packages/pip/_vendor/retrying.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/six.py` & `venv/Lib/site-packages/pip/_vendor/six.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/__init__.py` & `venv/Lib/site-packages/pip/_vendor/__init__.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/adapter.py` & `venv/Lib/site-packages/pip/_vendor/cachecontrol/adapter.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/cache.py` & `venv/Lib/site-packages/pip/_vendor/cachecontrol/cache.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/compat.py` & `venv/Lib/site-packages/pip/_vendor/cachecontrol/compat.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/controller.py` & `venv/Lib/site-packages/pip/_vendor/cachecontrol/controller.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/filewrapper.py` & `venv/Lib/site-packages/pip/_vendor/cachecontrol/filewrapper.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/heuristics.py` & `venv/Lib/site-packages/pip/_vendor/cachecontrol/heuristics.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/serialize.py` & `venv/Lib/site-packages/pip/_vendor/cachecontrol/serialize.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/wrapper.py` & `venv/Lib/site-packages/pip/_vendor/cachecontrol/wrapper.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/_cmd.py` & `venv/Lib/site-packages/pip/_vendor/cachecontrol/_cmd.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py` & `venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py` & `venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/certifi/core.py` & `venv/Lib/site-packages/pip/_vendor/certifi/core.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/big5freq.py` & `venv/Lib/site-packages/pip/_vendor/chardet/big5freq.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/big5prober.py` & `venv/Lib/site-packages/pip/_vendor/chardet/big5prober.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/chardistribution.py` & `venv/Lib/site-packages/pip/_vendor/chardet/chardistribution.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/charsetgroupprober.py` & `venv/Lib/site-packages/pip/_vendor/chardet/charsetgroupprober.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/charsetprober.py` & `venv/Lib/site-packages/pip/_vendor/chardet/charsetprober.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/codingstatemachine.py` & `venv/Lib/site-packages/pip/_vendor/chardet/codingstatemachine.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/compat.py` & `venv/Lib/site-packages/pip/_vendor/chardet/compat.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/cp949prober.py` & `venv/Lib/site-packages/pip/_vendor/chardet/cp949prober.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/enums.py` & `venv/Lib/site-packages/pip/_vendor/chardet/enums.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/escprober.py` & `venv/Lib/site-packages/pip/_vendor/chardet/escprober.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/escsm.py` & `venv/Lib/site-packages/pip/_vendor/chardet/escsm.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/eucjpprober.py` & `venv/Lib/site-packages/pip/_vendor/chardet/eucjpprober.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/euckrfreq.py` & `venv/Lib/site-packages/pip/_vendor/chardet/euckrfreq.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/euckrprober.py` & `venv/Lib/site-packages/pip/_vendor/chardet/euckrprober.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/euctwfreq.py` & `venv/Lib/site-packages/pip/_vendor/chardet/euctwfreq.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/euctwprober.py` & `venv/Lib/site-packages/pip/_vendor/chardet/euctwprober.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/gb2312freq.py` & `venv/Lib/site-packages/pip/_vendor/chardet/gb2312freq.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/gb2312prober.py` & `venv/Lib/site-packages/pip/_vendor/chardet/gb2312prober.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/hebrewprober.py` & `venv/Lib/site-packages/pip/_vendor/chardet/hebrewprober.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/jisfreq.py` & `venv/Lib/site-packages/pip/_vendor/chardet/jisfreq.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/jpcntx.py` & `venv/Lib/site-packages/pip/_vendor/chardet/jpcntx.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/langbulgarianmodel.py` & `venv/Lib/site-packages/pip/_vendor/chardet/langbulgarianmodel.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/langcyrillicmodel.py` & `venv/Lib/site-packages/pip/_vendor/chardet/langcyrillicmodel.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/langgreekmodel.py` & `venv/Lib/site-packages/pip/_vendor/chardet/langgreekmodel.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/langhebrewmodel.py` & `venv/Lib/site-packages/pip/_vendor/chardet/langhebrewmodel.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/langhungarianmodel.py` & `venv/Lib/site-packages/pip/_vendor/chardet/langhungarianmodel.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/langthaimodel.py` & `venv/Lib/site-packages/pip/_vendor/chardet/langthaimodel.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/langturkishmodel.py` & `venv/Lib/site-packages/pip/_vendor/chardet/langturkishmodel.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/latin1prober.py` & `venv/Lib/site-packages/pip/_vendor/chardet/latin1prober.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/mbcharsetprober.py` & `venv/Lib/site-packages/pip/_vendor/chardet/mbcharsetprober.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/mbcsgroupprober.py` & `venv/Lib/site-packages/pip/_vendor/chardet/mbcsgroupprober.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/mbcssm.py` & `venv/Lib/site-packages/pip/_vendor/chardet/mbcssm.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/sbcharsetprober.py` & `venv/Lib/site-packages/pip/_vendor/chardet/sbcharsetprober.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/sbcsgroupprober.py` & `venv/Lib/site-packages/pip/_vendor/chardet/sbcsgroupprober.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/sjisprober.py` & `venv/Lib/site-packages/pip/_vendor/chardet/sjisprober.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/universaldetector.py` & `venv/Lib/site-packages/pip/_vendor/chardet/universaldetector.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/utf8prober.py` & `venv/Lib/site-packages/pip/_vendor/chardet/utf8prober.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/__init__.py` & `venv/Lib/site-packages/pip/_vendor/chardet/__init__.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/chardet/cli/chardetect.py` & `venv/Lib/site-packages/pip/_vendor/chardet/cli/chardetect.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/colorama/ansi.py` & `venv/Lib/site-packages/pip/_vendor/colorama/ansi.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/colorama/ansitowin32.py` & `venv/Lib/site-packages/pip/_vendor/colorama/ansitowin32.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/colorama/initialise.py` & `venv/Lib/site-packages/pip/_vendor/colorama/initialise.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/colorama/win32.py` & `venv/Lib/site-packages/pip/_vendor/colorama/win32.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/colorama/winterm.py` & `venv/Lib/site-packages/pip/_vendor/colorama/winterm.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/distlib/compat.py` & `venv/Lib/site-packages/pip/_vendor/distlib/compat.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/distlib/database.py` & `venv/Lib/site-packages/pip/_vendor/distlib/database.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/distlib/index.py` & `venv/Lib/site-packages/pip/_vendor/distlib/index.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/distlib/locators.py` & `venv/Lib/site-packages/pip/_vendor/distlib/locators.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/distlib/manifest.py` & `venv/Lib/site-packages/pip/_vendor/distlib/manifest.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/distlib/markers.py` & `venv/Lib/site-packages/pip/_vendor/distlib/markers.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/distlib/metadata.py` & `venv/Lib/site-packages/pip/_vendor/distlib/metadata.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/distlib/resources.py` & `venv/Lib/site-packages/pip/_vendor/distlib/resources.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/distlib/scripts.py` & `venv/Lib/site-packages/pip/_vendor/distlib/scripts.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/distlib/util.py` & `venv/Lib/site-packages/pip/_vendor/distlib/util.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/distlib/version.py` & `venv/Lib/site-packages/pip/_vendor/distlib/version.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/distlib/wheel.py` & `venv/Lib/site-packages/pip/_vendor/distlib/wheel.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/distlib/__init__.py` & `venv/Lib/site-packages/pip/_vendor/distlib/__init__.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/distlib/_backport/misc.py` & `venv/Lib/site-packages/pip/_vendor/distlib/_backport/misc.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/distlib/_backport/shutil.py` & `venv/Lib/site-packages/pip/_vendor/distlib/_backport/shutil.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/distlib/_backport/sysconfig.py` & `venv/Lib/site-packages/pip/_vendor/distlib/_backport/sysconfig.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/distlib/_backport/tarfile.py` & `venv/Lib/site-packages/pip/_vendor/distlib/_backport/tarfile.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/constants.py` & `venv/Lib/site-packages/pip/_vendor/html5lib/constants.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/html5parser.py` & `venv/Lib/site-packages/pip/_vendor/html5lib/html5parser.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/serializer.py` & `venv/Lib/site-packages/pip/_vendor/html5lib/serializer.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/_ihatexml.py` & `venv/Lib/site-packages/pip/_vendor/html5lib/_ihatexml.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/_inputstream.py` & `venv/Lib/site-packages/pip/_vendor/html5lib/_inputstream.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/_tokenizer.py` & `venv/Lib/site-packages/pip/_vendor/html5lib/_tokenizer.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/_utils.py` & `venv/Lib/site-packages/pip/_vendor/html5lib/_utils.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/__init__.py` & `venv/Lib/site-packages/pip/_vendor/html5lib/__init__.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/filters/alphabeticalattributes.py` & `venv/Lib/site-packages/pip/_vendor/html5lib/filters/alphabeticalattributes.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/filters/inject_meta_charset.py` & `venv/Lib/site-packages/pip/_vendor/html5lib/filters/inject_meta_charset.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/filters/lint.py` & `venv/Lib/site-packages/pip/_vendor/html5lib/filters/lint.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/filters/optionaltags.py` & `venv/Lib/site-packages/pip/_vendor/html5lib/filters/optionaltags.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/filters/sanitizer.py` & `venv/Lib/site-packages/pip/_vendor/html5lib/filters/sanitizer.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/filters/whitespace.py` & `venv/Lib/site-packages/pip/_vendor/html5lib/filters/whitespace.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/treeadapters/genshi.py` & `venv/Lib/site-packages/pip/_vendor/html5lib/treeadapters/genshi.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/treeadapters/sax.py` & `venv/Lib/site-packages/pip/_vendor/html5lib/treeadapters/sax.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/treeadapters/__init__.py` & `venv/Lib/site-packages/pip/_vendor/html5lib/treeadapters/__init__.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/treebuilders/base.py` & `venv/Lib/site-packages/pip/_vendor/html5lib/treebuilders/base.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/treebuilders/dom.py` & `venv/Lib/site-packages/pip/_vendor/html5lib/treebuilders/dom.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/treebuilders/etree.py` & `venv/Lib/site-packages/pip/_vendor/html5lib/treebuilders/etree.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/treebuilders/etree_lxml.py` & `venv/Lib/site-packages/pip/_vendor/html5lib/treebuilders/etree_lxml.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/treebuilders/__init__.py` & `venv/Lib/site-packages/pip/_vendor/html5lib/treebuilders/__init__.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/treewalkers/base.py` & `venv/Lib/site-packages/pip/_vendor/html5lib/treewalkers/base.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/treewalkers/dom.py` & `venv/Lib/site-packages/pip/_vendor/html5lib/treewalkers/dom.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/treewalkers/etree.py` & `venv/Lib/site-packages/pip/_vendor/html5lib/treewalkers/etree.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/treewalkers/etree_lxml.py` & `venv/Lib/site-packages/pip/_vendor/html5lib/treewalkers/etree_lxml.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/treewalkers/genshi.py` & `venv/Lib/site-packages/pip/_vendor/html5lib/treewalkers/genshi.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/treewalkers/__init__.py` & `venv/Lib/site-packages/pip/_vendor/html5lib/treewalkers/__init__.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/_trie/datrie.py` & `venv/Lib/site-packages/pip/_vendor/html5lib/_trie/datrie.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/_trie/py.py` & `venv/Lib/site-packages/pip/_vendor/html5lib/_trie/py.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/html5lib/_trie/_base.py` & `venv/Lib/site-packages/pip/_vendor/html5lib/_trie/_base.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/idna/codec.py` & `venv/Lib/site-packages/pip/_vendor/idna/codec.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/idna/core.py` & `venv/Lib/site-packages/pip/_vendor/idna/core.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/idna/idnadata.py` & `venv/Lib/site-packages/pip/_vendor/idna/idnadata.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/idna/intranges.py` & `venv/Lib/site-packages/pip/_vendor/idna/intranges.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/idna/uts46data.py` & `venv/Lib/site-packages/pip/_vendor/idna/uts46data.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/lockfile/linklockfile.py` & `venv/Lib/site-packages/pip/_vendor/lockfile/linklockfile.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/lockfile/mkdirlockfile.py` & `venv/Lib/site-packages/pip/_vendor/lockfile/mkdirlockfile.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/lockfile/pidlockfile.py` & `venv/Lib/site-packages/pip/_vendor/lockfile/pidlockfile.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/lockfile/sqlitelockfile.py` & `venv/Lib/site-packages/pip/_vendor/lockfile/sqlitelockfile.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/lockfile/symlinklockfile.py` & `venv/Lib/site-packages/pip/_vendor/lockfile/symlinklockfile.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/lockfile/__init__.py` & `venv/Lib/site-packages/pip/_vendor/lockfile/__init__.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/msgpack/exceptions.py` & `venv/Lib/site-packages/pip/_vendor/msgpack/exceptions.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/msgpack/fallback.py` & `venv/Lib/site-packages/pip/_vendor/msgpack/fallback.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/msgpack/__init__.py` & `venv/Lib/site-packages/pip/_vendor/msgpack/__init__.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/packaging/markers.py` & `venv/Lib/site-packages/pip/_vendor/packaging/markers.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/packaging/requirements.py` & `venv/Lib/site-packages/pip/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/packaging/specifiers.py` & `venv/Lib/site-packages/pip/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/packaging/utils.py` & `venv/Lib/site-packages/pip/_vendor/packaging/utils.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/packaging/version.py` & `venv/Lib/site-packages/pip/_vendor/packaging/version.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/packaging/_compat.py` & `venv/Lib/site-packages/pip/_vendor/packaging/_compat.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/packaging/_structures.py` & `venv/Lib/site-packages/pip/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/packaging/__about__.py` & `venv/Lib/site-packages/pip/_vendor/packaging/__about__.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/packaging/__init__.py` & `venv/Lib/site-packages/pip/_vendor/packaging/__init__.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/pkg_resources/py31compat.py` & `venv/Lib/site-packages/pip/_vendor/pkg_resources/py31compat.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/pkg_resources/__init__.py` & `venv/Lib/site-packages/pip/_vendor/pkg_resources/__init__.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/progress/bar.py` & `venv/Lib/site-packages/pip/_vendor/progress/bar.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/progress/counter.py` & `venv/Lib/site-packages/pip/_vendor/progress/counter.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/progress/helpers.py` & `venv/Lib/site-packages/pip/_vendor/progress/helpers.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/progress/spinner.py` & `venv/Lib/site-packages/pip/_vendor/progress/spinner.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/progress/__init__.py` & `venv/Lib/site-packages/pip/_vendor/progress/__init__.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/pytoml/core.py` & `venv/Lib/site-packages/pip/_vendor/pytoml/core.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/pytoml/parser.py` & `venv/Lib/site-packages/pip/_vendor/pytoml/parser.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/pytoml/writer.py` & `venv/Lib/site-packages/pip/_vendor/pytoml/writer.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/requests/adapters.py` & `venv/Lib/site-packages/pip/_vendor/requests/adapters.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/requests/api.py` & `venv/Lib/site-packages/pip/_vendor/requests/api.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/requests/auth.py` & `venv/Lib/site-packages/pip/_vendor/requests/auth.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/requests/compat.py` & `venv/Lib/site-packages/pip/_vendor/requests/compat.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/requests/cookies.py` & `venv/Lib/site-packages/pip/_vendor/requests/cookies.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/requests/exceptions.py` & `venv/Lib/site-packages/pip/_vendor/requests/exceptions.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/requests/help.py` & `venv/Lib/site-packages/pip/_vendor/requests/help.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/requests/hooks.py` & `venv/Lib/site-packages/pip/_vendor/requests/hooks.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/requests/models.py` & `venv/Lib/site-packages/pip/_vendor/requests/models.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/requests/packages.py` & `venv/Lib/site-packages/pip/_vendor/requests/packages.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/requests/sessions.py` & `venv/Lib/site-packages/pip/_vendor/requests/sessions.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/requests/status_codes.py` & `venv/Lib/site-packages/pip/_vendor/requests/status_codes.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/requests/structures.py` & `venv/Lib/site-packages/pip/_vendor/requests/structures.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/requests/utils.py` & `venv/Lib/site-packages/pip/_vendor/requests/utils.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/requests/_internal_utils.py` & `venv/Lib/site-packages/pip/_vendor/requests/_internal_utils.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/requests/__init__.py` & `venv/Lib/site-packages/pip/_vendor/requests/__init__.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/connection.py` & `venv/Lib/site-packages/pip/_vendor/urllib3/connection.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/connectionpool.py` & `venv/Lib/site-packages/pip/_vendor/urllib3/connectionpool.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/exceptions.py` & `venv/Lib/site-packages/pip/_vendor/urllib3/exceptions.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/fields.py` & `venv/Lib/site-packages/pip/_vendor/urllib3/fields.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/filepost.py` & `venv/Lib/site-packages/pip/_vendor/urllib3/filepost.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/poolmanager.py` & `venv/Lib/site-packages/pip/_vendor/urllib3/poolmanager.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/request.py` & `venv/Lib/site-packages/pip/_vendor/urllib3/request.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/response.py` & `venv/Lib/site-packages/pip/_vendor/urllib3/response.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/_collections.py` & `venv/Lib/site-packages/pip/_vendor/urllib3/_collections.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/__init__.py` & `venv/Lib/site-packages/pip/_vendor/urllib3/__init__.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/appengine.py` & `venv/Lib/site-packages/pip/_vendor/urllib3/contrib/appengine.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py` & `venv/Lib/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py` & `venv/Lib/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/securetransport.py` & `venv/Lib/site-packages/pip/_vendor/urllib3/contrib/securetransport.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/socks.py` & `venv/Lib/site-packages/pip/_vendor/urllib3/contrib/socks.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py` & `venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py` & `venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/packages/ordered_dict.py` & `venv/Lib/site-packages/pip/_vendor/urllib3/packages/ordered_dict.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/packages/six.py` & `venv/Lib/site-packages/pip/_vendor/urllib3/packages/six.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py` & `venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/packages/ssl_match_hostname/_implementation.py` & `venv/Lib/site-packages/pip/_vendor/urllib3/packages/ssl_match_hostname/_implementation.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/packages/ssl_match_hostname/__init__.py` & `venv/Lib/site-packages/pip/_vendor/urllib3/packages/ssl_match_hostname/__init__.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/connection.py` & `venv/Lib/site-packages/pip/_vendor/urllib3/util/connection.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/request.py` & `venv/Lib/site-packages/pip/_vendor/urllib3/util/request.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/response.py` & `venv/Lib/site-packages/pip/_vendor/urllib3/util/response.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/retry.py` & `venv/Lib/site-packages/pip/_vendor/urllib3/util/retry.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/selectors.py` & `venv/Lib/site-packages/pip/_vendor/urllib3/util/selectors.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/ssl_.py` & `venv/Lib/site-packages/pip/_vendor/urllib3/util/ssl_.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/timeout.py` & `venv/Lib/site-packages/pip/_vendor/urllib3/util/timeout.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/url.py` & `venv/Lib/site-packages/pip/_vendor/urllib3/util/url.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/wait.py` & `venv/Lib/site-packages/pip/_vendor/urllib3/util/wait.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/__init__.py` & `venv/Lib/site-packages/pip/_vendor/urllib3/util/__init__.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/webencodings/labels.py` & `venv/Lib/site-packages/pip/_vendor/webencodings/labels.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/webencodings/mklabels.py` & `venv/Lib/site-packages/pip/_vendor/webencodings/mklabels.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/webencodings/tests.py` & `venv/Lib/site-packages/pip/_vendor/webencodings/tests.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/webencodings/x_user_defined.py` & `venv/Lib/site-packages/pip/_vendor/webencodings/x_user_defined.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pip/_vendor/webencodings/__init__.py` & `venv/Lib/site-packages/pip/_vendor/webencodings/__init__.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pkg_resources/py31compat.py` & `venv/Lib/site-packages/pkg_resources/py31compat.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pkg_resources/__init__.py` & `venv/Lib/site-packages/pkg_resources/__init__.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pkg_resources/extern/__init__.py` & `venv/Lib/site-packages/pkg_resources/extern/__init__.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pkg_resources/_vendor/appdirs.py` & `venv/Lib/site-packages/pkg_resources/_vendor/appdirs.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing.py` & `venv/Lib/site-packages/pkg_resources/_vendor/pyparsing.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pkg_resources/_vendor/six.py` & `venv/Lib/site-packages/pkg_resources/_vendor/six.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pkg_resources/_vendor/packaging/markers.py` & `venv/Lib/site-packages/pkg_resources/_vendor/packaging/markers.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pkg_resources/_vendor/packaging/requirements.py` & `venv/Lib/site-packages/pkg_resources/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pkg_resources/_vendor/packaging/specifiers.py` & `venv/Lib/site-packages/pkg_resources/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pkg_resources/_vendor/packaging/version.py` & `venv/Lib/site-packages/pkg_resources/_vendor/packaging/version.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_compat.py` & `venv/Lib/site-packages/pkg_resources/_vendor/packaging/_compat.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_structures.py` & `venv/Lib/site-packages/pkg_resources/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pkg_resources/_vendor/packaging/__about__.py` & `venv/Lib/site-packages/pkg_resources/_vendor/packaging/__about__.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/pkg_resources/_vendor/packaging/__init__.py` & `venv/Lib/site-packages/pkg_resources/_vendor/packaging/__init__.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/setuptools/archive_util.py` & `venv/Lib/site-packages/setuptools/archive_util.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/setuptools/build_meta.py` & `venv/Lib/site-packages/setuptools/build_meta.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/setuptools/config.py` & `venv/Lib/site-packages/setuptools/config.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/setuptools/depends.py` & `venv/Lib/site-packages/setuptools/depends.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/setuptools/dep_util.py` & `venv/Lib/site-packages/setuptools/dep_util.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/setuptools/dist.py` & `venv/Lib/site-packages/setuptools/dist.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/setuptools/extension.py` & `venv/Lib/site-packages/setuptools/extension.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/setuptools/glibc.py` & `venv/Lib/site-packages/setuptools/glibc.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/setuptools/glob.py` & `venv/Lib/site-packages/setuptools/glob.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/setuptools/launch.py` & `venv/Lib/site-packages/setuptools/launch.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/setuptools/lib2to3_ex.py` & `venv/Lib/site-packages/setuptools/lib2to3_ex.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/setuptools/monkey.py` & `venv/Lib/site-packages/setuptools/monkey.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/setuptools/msvc.py` & `venv/Lib/site-packages/setuptools/msvc.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/setuptools/namespaces.py` & `venv/Lib/site-packages/setuptools/namespaces.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/setuptools/package_index.py` & `venv/Lib/site-packages/setuptools/package_index.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/setuptools/pep425tags.py` & `venv/Lib/site-packages/setuptools/pep425tags.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/setuptools/py27compat.py` & `venv/Lib/site-packages/setuptools/py27compat.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/setuptools/py31compat.py` & `venv/Lib/site-packages/setuptools/py31compat.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/setuptools/py33compat.py` & `venv/Lib/site-packages/setuptools/py33compat.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/setuptools/py36compat.py` & `venv/Lib/site-packages/setuptools/py36compat.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/setuptools/sandbox.py` & `venv/Lib/site-packages/setuptools/sandbox.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/setuptools/site-patch.py` & `venv/Lib/site-packages/setuptools/site-patch.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/setuptools/ssl_support.py` & `venv/Lib/site-packages/setuptools/ssl_support.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/setuptools/unicode_utils.py` & `venv/Lib/site-packages/setuptools/unicode_utils.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/setuptools/wheel.py` & `venv/Lib/site-packages/setuptools/wheel.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/setuptools/windows_support.py` & `venv/Lib/site-packages/setuptools/windows_support.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/setuptools/__init__.py` & `venv/Lib/site-packages/setuptools/__init__.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/setuptools/command/alias.py` & `venv/Lib/site-packages/setuptools/command/alias.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/setuptools/command/bdist_egg.py` & `venv/Lib/site-packages/setuptools/command/bdist_egg.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/setuptools/command/bdist_rpm.py` & `venv/Lib/site-packages/setuptools/command/bdist_rpm.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/setuptools/command/bdist_wininst.py` & `venv/Lib/site-packages/setuptools/command/bdist_wininst.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/setuptools/command/build_clib.py` & `venv/Lib/site-packages/setuptools/command/build_clib.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/setuptools/command/build_ext.py` & `venv/Lib/site-packages/setuptools/command/build_ext.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/setuptools/command/build_py.py` & `venv/Lib/site-packages/setuptools/command/build_py.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/setuptools/command/develop.py` & `venv/Lib/site-packages/setuptools/command/develop.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/setuptools/command/dist_info.py` & `venv/Lib/site-packages/setuptools/command/dist_info.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/setuptools/command/easy_install.py` & `venv/Lib/site-packages/setuptools/command/easy_install.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/setuptools/command/egg_info.py` & `venv/Lib/site-packages/setuptools/command/egg_info.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/setuptools/command/install.py` & `venv/Lib/site-packages/setuptools/command/install.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/setuptools/command/install_egg_info.py` & `venv/Lib/site-packages/setuptools/command/install_egg_info.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/setuptools/command/install_lib.py` & `venv/Lib/site-packages/setuptools/command/install_lib.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/setuptools/command/install_scripts.py` & `venv/Lib/site-packages/setuptools/command/install_scripts.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/setuptools/command/py36compat.py` & `venv/Lib/site-packages/setuptools/command/py36compat.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/setuptools/command/rotate.py` & `venv/Lib/site-packages/setuptools/command/rotate.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/setuptools/command/saveopts.py` & `venv/Lib/site-packages/setuptools/command/saveopts.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/setuptools/command/sdist.py` & `venv/Lib/site-packages/setuptools/command/sdist.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/setuptools/command/setopt.py` & `venv/Lib/site-packages/setuptools/command/setopt.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/setuptools/command/test.py` & `venv/Lib/site-packages/setuptools/command/test.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/setuptools/command/upload.py` & `venv/Lib/site-packages/setuptools/command/upload.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/setuptools/command/upload_docs.py` & `venv/Lib/site-packages/setuptools/command/upload_docs.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/setuptools/command/__init__.py` & `venv/Lib/site-packages/setuptools/command/__init__.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/setuptools/extern/__init__.py` & `venv/Lib/site-packages/setuptools/extern/__init__.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/setuptools/_vendor/pyparsing.py` & `venv/Lib/site-packages/setuptools/_vendor/pyparsing.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/setuptools/_vendor/six.py` & `venv/Lib/site-packages/setuptools/_vendor/six.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/setuptools/_vendor/packaging/markers.py` & `venv/Lib/site-packages/setuptools/_vendor/packaging/markers.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/setuptools/_vendor/packaging/requirements.py` & `venv/Lib/site-packages/setuptools/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/setuptools/_vendor/packaging/specifiers.py` & `venv/Lib/site-packages/setuptools/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/setuptools/_vendor/packaging/version.py` & `venv/Lib/site-packages/setuptools/_vendor/packaging/version.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/setuptools/_vendor/packaging/_compat.py` & `venv/Lib/site-packages/setuptools/_vendor/packaging/_compat.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/setuptools/_vendor/packaging/_structures.py` & `venv/Lib/site-packages/setuptools/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/setuptools/_vendor/packaging/__about__.py` & `venv/Lib/site-packages/setuptools/_vendor/packaging/__about__.py`

 * *Files identical despite different names*

## Comparing `p0-script-1.0.2/venv/Lib/site-packages/setuptools/_vendor/packaging/__init__.py` & `venv/Lib/site-packages/setuptools/_vendor/packaging/__init__.py`

 * *Files identical despite different names*

