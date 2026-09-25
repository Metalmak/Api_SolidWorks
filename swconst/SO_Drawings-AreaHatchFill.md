<!-- source: swconst/SO_Drawings-AreaHatchFill.htm -->

# SOLIDWORKS API Help

# System Options > Drawings > Area Hatch/Fill

![](SO_Drawings-AreaHatchFill.gif)

| Setting | Get/Set Methods | Return Value  or  <Value> | Comment |
| None | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swDrawingAreaHatchFillStyle)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swDrawingAreaHatchFillStyle, swAreaHatchFillStyle\_e.swAreaHatchFillStyle\_None) | See swAreaHatchFillStyle\_e for valid options |  |
| Solid | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swDrawingAreaHatchFillStyle)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swDrawingAreaHatchFillStyle, swAreaHatchFillStyle\_e.swAreaHatchFillStyle\_Solid) | See swAreaHatchFillStyle\_e for valid options |  |
| Hatch | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swDrawingAreaHatchFillStyle)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swDrawingAreaHatchFillStyle, swAreaHatchFillStyle\_e.swAreaHatchFillStyle\_Pattern) | See swAreaHatchFillStyle\_e for valid options |  |
| Pattern | ISldWorks::GetUserPreferenceStringValue(swUserPreferenceStringValue\_e.swDrawingAreaHatchPattern)  ISldWorks::SetUserPreferenceStringValue(swUserPreferenceStringValue\_e.swDrawingAreaHatchPattern, <Value>) | String value | ![](SO_Drawings-areaHatchFillPattern.gif) |
| Scale | ISldWorks::GetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swDrawingAreaHatchScale)  ISldWorks::SetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swDrawingAreaHatchScale, <Value>) | Double value | Specifies value to scale crosshatch |
| Angle | ISldWorks::GetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swDrawingAreaHatchAngle)  ISldWorks::SetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swDrawingAreaHatchAngle, <Value>) | Double value | Specifies angle for crosshatch |