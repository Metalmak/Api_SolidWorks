<!-- source: swconst/SO_HoleWizardToolbox.htm -->

# SOLIDWORKS API Help

# System Options > Hole Wizard/Toolbox

![](SO_HoleWizardToolbox.gif)

| Setting | Get/Set Methods | Return Value  or  <Value> | Comment |
| Hole Wizard and Toolbox folder | ISldWorks::GetUserPreferenceStringValue(swUserPreferenceStringValue\_e.swHoleWizardToolBoxFolder) ISldWorks::SetUserPreferenceStringValue(swUserPreferenceStringValue\_e.swHoleWizardToolBoxFolder, <Value>) | String value | Specifies the location of the Hole Wizard/Toolbox folder |
| Make this folder the default search location for Toolbox components | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swUseFolderAsDefaultSearchLocation)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swUseFolderAsDefaultSearchLocation, <Value>) | Boolean value | Specifies whether to make the specified Hole Wizard and Toolbox folder the default search location for Toolbox components |
| Toolbox Task Pane - Display Toolbox Favorites folder | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swShowToolboxFavoritesFolder)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swShowToolboxFavoritesFolder, <Value>) | Boolean value | Specifies whether to display the Toolbox Favorites folder |
| Toolbox Mates - Lock rotation of new concentric mates to Toolbox components | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swLockRotationConcentricMates)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swLockRotationConcentricMates, <Value>) | Boolean value |  |
| Hole Wizard settings | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swTransferHoleWizardSizeComboBoxSettings)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swTransferHoleWizardSizeComboBoxSettings, <Value>) | Boolean value | True to preserve settings for each Hole Wizard hole type, false to transfer settings when changing Hole Wizard hole type |
| Include data for DELMIA applications | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swIncludeDataForDelmia)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swIncludeDataForDelmia, <Value>) | Boolean value |  |