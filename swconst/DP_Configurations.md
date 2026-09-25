<!-- source: swconst/DP_Configurations.htm -->

# SOLIDWORKS API Help

# Document Properties > Configurations

Configurations settings are not supported in SOLIDWORKS Connected.

![](DP_Configurations.gif)

| Setting | Get/Set Methods | Return Value or <Value> | Comments |
| Add Rebuild/Save mark to new configurations (Not supported in SOLIDWORKS Connected) | IModelDocExtension::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swRebuildSaveNewConfig, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swRebuildSaveNewConfig, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, <Value>) | Boolean value | Specifies whether to apply the Rebuild/Save mark to new configurations. |
| Add Display Data Mark to new configurations (Not supported in SOLIDWORKS Connected) | IModelDocExtension::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swDisplayDataMarkNewConfig, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swDisplayDataMarkNewConfig, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, <Value>) | Boolean value |  |