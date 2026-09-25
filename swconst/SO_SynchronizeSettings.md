<!-- source: swconst/SO_SynchronizeSettings.htm -->

# SOLIDWORKS API Help

# System Options > Synchronize Settings

This dialog is only available in SOLIDWORKS Connected.

![](SO_SynchronizeSettings.gif)

| Setting | Get/Set Methods | Return value  or   <Value>  or  <OnFlag> | Comment |
| Last Synchronization (SOLIDWORKS Connected only) | ISldWorks::GetUserPreferenceStringValue(swUserPreferenceStringValue\_e.swLastSynchronizationTimeStamp) | String value |  |
| Automatic Synchronization -  Automatically synchronize settings (SOLIDWORKS Connected only) | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swAutomaticSyncSettings) ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swAutomaticSyncSettings, <OnFlag>) | Boolean value | When set to true, specified settings to include are automatically synchronized when logging in and out of SOLIDWORKS Connected |
| Automatic Synchronization - Settings to include - System Options  (SOLIDWORKS Connected only) | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swAutoSyncSettingsToInclude\_SystemOptions) ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swAutoSyncSettingsToInclude\_SystemOptions, <OnFlag>) | Boolean value | Valid only if swUserPreferenceToggle\_e.swAutomaticSyncSettings is set to true |
| Automatic Synchronization - Settings to include - File Locations (SOLIDWORKS Connected only) | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swAutoSyncSettingsToInclude\_FileLocations) ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swAutoSyncSettingsToInclude\_FileLocations, <OnFlag>) | Boolean value | Valid only if swUserPreferenceToggle\_e.swAutomaticSyncSettings is set to true |
| Automatic Synchronization - Settings to include - Customizations (SOLIDWORKS Connected only) | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swAutoSyncSettingsToInclude\_Customizations) ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swAutoSyncSettingsToInclude\_Customizations, <OnFlag>) | Boolean value | Valid only if swUserPreferenceToggle\_e.swAutomaticSyncSettings is set to true |
| Synchronize Now - Upload Settings... (SOLIDWORKS Connected only) | ISldWorks::UploadToMySolidWorksSettings | Integer value |  |
| Synchronize Now - Download Settings... (SOLIDWORKS Connected only) | ISldWorks::DownloadFromMySolidWorksSettings | Integer value |  |