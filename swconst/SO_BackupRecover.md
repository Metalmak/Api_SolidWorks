<!-- source: swconst/SO_BackupRecover.htm -->

# SOLIDWORKS API Help

# System Options > Backup/Recover

This topic contains two tables. The information in the table:

* appearing immediately after the screen capture corresponds to the settings on that dialog.
* titled [Obsolete
  Enumerators](#Obsolete) contains enumerators that previously appeared on the dialog
  but are now obsolete.

![](SO_BackupRecover.gif)

| Setting | Get/Set Methods | Return value  or   <Value>  or  <OnFlag> | Comment |
| Auto-recover - Save auto-recover info every | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swAutoSaveEnable) ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swAutoSaveEnable, <OnFlag>) | Boolean value | Specifies whether auto-recovery is enabled |
| Auto-recover - Save auto-recover info every - <n> | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swAutoSaveInterval) ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swAutoSaveInterval, <Value>) | Integer value:   * 0 = Turn off auto-recovery * non-0 = number of operations between auto-recoveries,   up to 120 |  |
| Auto-recover - Save auto-recover info every - <units> | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swAutoSaveIntervalMode) ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swAutoSaveIntervalMode, swAutoSaveIntervalMode\_e.<Value>) | See swAutoSaveIntervalMode\_e for valid options | Specifies auto-recover mode |
| Auto-recover - Auto-recover folder | ISldWorks::GetUserPreferenceStringValue(swUserPreferenceStringValue\_e.swAutoSaveDirectory)  ISldWorks::SetUserPreferenceStringValue(swUserPreferenceStringValue\_e.swAutoSaveDirectory, <Value>) | String value |  |
| Backup - Number of backup copies per document (Not supported in SOLIDWORKS Connected) | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swBackupEnable) ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swBackupEnable, <OnFlag>) | Boolean value | Specifies whether backup copies of the document are created before any changes to the document are made |
| Backup - Number of backup copies per document - <n> (Not supported in SOLIDWORKS Connected) | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swBackupCopiesPerDocument)  ISldWorks::SetUserPreferIntegerStringValue\_e.swBackupCopiesPerDocument, <Value>) | Integer value: 1 - 10 | Specifies number of backup copies per document |
| Backup - Backup folder  Backup - Save backup files in the same location as the original (Not supported in SOLIDWORKS Connected) | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swSaveBackupFilesInSameLocationAsOriginal) ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swSaveBackupFilesInSameLocationAsOriginal, <OnFlag>) | Boolean value:   * True: Specifies to save backup files in same location   as original file * False: Specifies to save backup files in the folder   specified in Backup folder |  |
| Backup - Backup folder - <folder> (Not supported in SOLIDWORKS Connected) | ISldWorks::GetUserPreferenceStringValue(swUserPreferenceStringValue\_e.swBackupDirectory)  ISldWorks::SetUserPreferenceStringValue(swUserPreferenceStringValue\_e.swBackupDirectory, <Value>) | String value | Specifies the  folder where to save backup files |
| Backup - Remove backups older (Not supported in SOLIDWORKS Connected) | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swBackupRemoveEnable) ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swBackupRemoveEnable, <OnFlag>) | Boolean value | Specifies whether  backup documents older than the specified days are removed when you start up SOLIDWORKS |
| Backup - Remove backups older than <n> days (Not supported in SOLIDWORKS Connected) | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swBackupRemoveInterval)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swBackupRemoveInterval, <Value>) | Integer value: 1 - 30 | Specifies the number of days when to remove backup copies of a document |

Obsolete Enumerators

| Enumerator | Comment |
| swBackupAfterMeshOrRunSimulationStudy | Obsolete |