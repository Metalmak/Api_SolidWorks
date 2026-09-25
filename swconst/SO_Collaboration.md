<!-- source: swconst/SO_Collaboration.htm -->

# SOLIDWORKS API Help

# System Options > Collaboration

This topic contains two tables. The information in the table:

* appearing immediately after the dialog corresponds to the settings on that dialog.
* titled [Obsolete
  Enumerators](#Obsolete) contains enumerators that previously appeared on
  the dialog but are now obsolete or have been moved to another location.

THe Collaboration settings are not supported in SOLIDWORKS Connected.

![](SO_Collaboration.gif)

| Setting | Get/Set Methods | Return Value  or  <Value>  or  <OnFlag> | Comment |
| Enable multi-user environment (Not supported in SOLIDWORKS Connected) | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swCollabEnableMultiuser) ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swCollabEnableMultiuser, <OnFlag>) | Boolean value | Specifies whether to  enable multi-user environment |
| Add shortcut menu items for multi-user environment (Not supported in SOLIDWORKS Connected) | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swCollabAddShortcutMenuItems) ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swCollabAddShortcutMenuItems, <OnFlag>) | Boolean value | Specifies whether to add shortcut menu items for multi-user environment |
| Check if files opened read-only have been modified by other users (Not supported in SOLIDWORKS Connected) | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swCollabCheckReadOnlyModifiedByOthers) ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swCollabCheckReadOnlyModifiedByOthers, <OnFlag>) | Boolean value | Specifies whether to check if files opened read-only have been modified by others; works with swUserPreferenceIntegerValue\_e.swCollabCheckReadOnlyModifiedInterval |
| Check files every <n> minutes (Not supported in SOLIDWORKS Connected) | ISldWorks::GetUserPreferenceIntegerValue(wUserPreferenceIntegerValue\_e.swCollabCheckReadOnlyModifiedInterval)  ISldWorks::SetUserPreferenceIntegerValue(wUserPreferenceIntegerValue\_e.swCollabCheckReadOnlyModifiedInterval, swCollabCheckReadOnlyModifiedInterval\_e .<Value>) | See swCollabCheckReadOnlyModifiedInterval\_e for valid options | Works with swUserPreferenceToggle\_e.swCollabCheckReadOnlyModifiedByOthers |

Obsolete Enumerators

| Enumerator | Comment |
| swCollabAddTimeStampToComments | Moved to **Tools > Options > FeatureManager** |
| swCollabShowCommentsInPropertyManager | Moved to **Tools > Options > FeatureManager** |