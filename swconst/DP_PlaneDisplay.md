<!-- source: swconst/DP_PlaneDisplay.htm -->

# SOLIDWORKS API Help

# Document Properties > Plane Display

![](DP_PlaneDisplay.gif)

| Setting | Get/Set Methods | Return Value or <Value> | Comments |
| Faces - Front Face Color... | IModelDocExtension::GetUserPreferenceInteger(swUserPreferenceIntegerValue\_e.swPlaneDisplayFrontFaceColor, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceInteger(swUserPreferenceIntegerValue\_e.swPlaneDisplayFrontFaceColor, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, <Value>) | Integer RGB color value |  |
| Faces - Back Face Color... | IModelDocExtension::GetUserPreferenceInteger(swUserPreferenceIntegerValue\_e.swPlaneDisplayBackFaceColor, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceInteger(swUserPreferenceIntegerValue\_e.swPlaneDisplayBackFaceColor, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, <Value>) | Integer RGB color value |  |
| Faces - Transparency | IModelDocExtension::GetUserPreferenceInteger(swUserPreferenceIntegerValue\_e.swPlaneDisplayTransparency, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceInteger(swUserPreferenceIntegerValue\_e.swPlaneDisplayTransparency, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, <Value>) | Integer percentage value (0 - 100) |  |
| Intersections - Show intersections | IModelDocExtension::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swPlaneDisplayShowIntersections, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swPlaneDisplayShowIntersections, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, <Value>) | Boolean value | Specifies whether to display the line at which two planes intersect |
| Intersections - Line Color... | IModelDocExtension::GetUserPreferenceInteger(swUserPreferenceIntegerValue\_e.swPlaneDisplayIntersectionLineColor, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceInteger(swUserPreferenceIntegerValue\_e.swPlaneDisplayIntersectionLineColor, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, <Value>) | Integer RGB color value |  |