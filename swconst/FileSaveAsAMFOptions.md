<!-- source: swconst/FileSaveAsAMFOptions.htm -->

# SOLIDWORKS API Help

# System Options > Export > AMF

This topic contains two tables. The information in the table:

* appearing immediately after the dialog corresponds to the settings on that dialog.
* titled [Obsolete
  Enumerators](#Obsolete) contains enumerators that previously appeared on
  the dialog but are now obsolete.

To display the dialog:

Click **Tools > Options > System Options > Export > AMF** in **File
Format**.

- or -

1. Click **File > Save As**.
2. In **Save as type**, select **Additive Manufacturing File**.
3. Click **Options**.

![](FileSaveAsAMFOptions.gif)

| Setting | Get/Set Methods | Return Value  or  <Value>  or  <OnFlag> | Comment |
| Output as - Compress file | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e, swAMFCompression)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e, swAMFCompression, <OnFlag>) | Boolean value | Specifies whether to compress the output file |
| Output as - Unit | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swExportStlUnits)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swExportStlUnits, swLengthUnit\_e.<Value>) | Valid options as defined in swLengthUnit\_e:   * 0 = swMM (millimeters) * 1 = swCM (centimeters) * 2 = swMETER * 3 = swINCHES * 4 = swFEET |  |
| Resolution -  * Coarse * Fine * Custom | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swSTLQuality)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swSTLQuality, swSTLQuality\_e.<*Value*>) | See swSTLQuality\_e for valid options | Specifies the resolution of the output for additive manufacturing files |
| Resolution - Deviation - Tolerance | ISldWorks::GetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swSTLDeviation)  ISldWorks::SetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swSTLDeviation, <Value>) | Double value | Specifies the deviation tolerance, which controls whole-part tessellation; lower numbers generate files with greater whole-part accuracy |
| Resolution - Angle - Tolerance | ISldWorks::GetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swSTLAngleTolerance)  ISldWorks::SetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swSTLAngleTolerance, <Value>) | Double value | Specifies the angle tolerance, which controls smaller detail tessellation; lower numbers generate files with greater small-detail accuracy, but those files take longer to generate |
| Resolution - Preview before saving file | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e, swSTLPreview)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e, swSTLPreview, <OnFlag>) | Boolean value | Specifies whether a faceted model preview is displayed in the graphics area |
| Include materials | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e, swAMFMaterials)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e, swAMFMaterials, <OnFlag>) | Boolean value | Specifies whether to include materials |
| Include colors | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e, swAMFColors)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e, swAMFColors, <OnFlag>) | Boolean value | Specifies whether to include colors |

Obsolete Enumerators

| Enumerator | Comment |
| swFileSaveAsCoordinateSystem | Obsolete |