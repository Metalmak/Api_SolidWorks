<!-- source: swconst/DP_GridSnap.htm -->

# SOLIDWORKS API Help

# Document Properties > Grip/Snap

![](DP_GridSnap.gif)

| Setting | Get/Set Methods | Return Value or <Value> | Comments |
| Display grid | IModelDocExtension::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swGridDisplay, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swGridDisplay, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, <Value>) | Boolean value | Specifies whether to display sketch grid |
| Dash | IModelDocExtension::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swGridDisplayDashed, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swGridDisplayDashed, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, <Value>) | Boolean value | Specifies whether to use solid or dashed grid lines; does not affect current document; only affects future documents |
| Automatic scaling | IModelDocExtension::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swGridAutomaticScaling, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swGridAutomaticScaling, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, <Value>) | Boolean value | Specifies whether to automatically adjust display of grid when zooming in and out |
| Major grid spacing | IModelDocExtension::GetUserPreferenceDouble(swUserPreferenceDoubleValue\_e.swGridMajorSpacing, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceDouble(swUserPreferenceDoubleValue\_e.swGridMajorSpacing, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, <Value>) | Double value in meters | Specifies space between major grid lines |
| Minor-lines per major | IModelDocExtension::GetUserPreferenceInteger(swUserPreferenceIntegerValue\_e.swGridMinorLinesPerMajor, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceInteger(swUserPreferenceIntegerValue\_e.swGridMinorLinesPerMajor, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, <Value>) | Integer value | Specifies the number of minor grid lines between major grid lines |
| Snap points per minor | IModelDocExtension::GetUserPreferenceInteger(swUserPreferenceIntegerValue\_e.swSnapPointsPerMinor, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceInteger(swUserPreferenceIntegerValue\_e.swSnapPointsPerMinor, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, <Value>) | Integer value | Specifies the number of snap points between minor grid lines |