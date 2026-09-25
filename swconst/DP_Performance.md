<!-- source: swconst/DP_Performance.htm -->

# SOLIDWORKS API Help

# Document Properties > Performance

The Performance tab appears only when a drawing is open.

![](DP_Performance.gif)

| Setting | Get/Set Methods | Return Value or <Value> | Comments |
| Detailing mode - Save model data | IModelDocExtension::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swDetailingModeSaveModelData, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swDetailingModeSaveModelData, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, <OnFlag>) | Boolean value | Valid only for drawings |
| Detailing mode - Include standard views in View Palette | IModelDocExtension::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swDetailingModeIncludeStandardViewsInViewPalette, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swDetailingModeIncludeStandardViewsInViewPalette, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, <OnFlag>) | Boolean value | Valid only for drawings and when Save model data is set to true |