<!-- source: swconst/FileSaveAsPlyOptions.htm -->

# SOLIDWORKS API Help

# System Options > Export > PLY

To display the dialog:

Click **Tools > Options > System Options > Export >
PLY** in **File Format**.

- or -

1. Click **File > Save As**.
2. In **Save as type**, select **Polygon File Format**.
3. Click **Options**.

![](FileSaveAsPLYOptions.gif)

| Setting | Get/Set Methods | Return Value   or   <Value>   or  <OnFlag> | Comment |
| Output as | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swPLYBinaryFormat)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swPLYBinaryFormat, <OnFlag>) | Boolean value |  |
| Output as - Unit | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swExportPlyUnits)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swExportPlyUnits, swLengthUnit\_e.<Value>) | Integer value as defined in swLengthUnit\_e |  |
| Resolution | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swPLYQuality)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swPLYQuality, swPLYQuality\_e.<Value>) | Integer value as defined in swPLYQuality\_e |  |
| Resolution - Deviation Tolerance | ISldWorks::GetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swPLYDeviation)  ISldWorks::SetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swPLYDeviation, <Value>) | Double value in meters | Valid only if swPLYQuality is set to swPLYQuality\_e.swPLYQuality\_CUSTOM; the value range varies by part or assembly. Inspect the dialog for the range of values for the opened model. |
| Resolution - Angle Tolerance | ISldWorks::GetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swPLYAngleTolerance)  ISldWorks::SetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swPLYAngleTolerance, <Value>) | 0.5236 >= Double value in radians >= 0.00873 | Valid only if swPLYQuality is set to swPLYQuality\_e.swPLYQuality\_CUSTOM |
| Resolution - Preview before saving file | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swPLYPreview)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swPLYPreview, <OnFlag>) | Boolean value |  |
| Include colors | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swPLYIncludeColors)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swPLYIncludeColors, <OnFlag>) | Boolean value |  |