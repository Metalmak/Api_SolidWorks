<!-- source: swconst/FileSaveAsSTLOptions.htm -->

# SOLIDWORKS API Help

# System Options > Export > STL

This topic contains two tables. The information in the table:

* appearing immediately after the dialog corresponds to the settings on that dialog.
* titled [Obsolete
  Enumerators](#Obsolete) contains enumerators that previously appeared on
  the dialog but are now obsolete.

To display the dialog:

Click **Tools > Options > System Options > Export > STL** in **File
Format**.

- or -

1. Click **File > Save As**.
2. In **Save as type**, select **STL**.
3. Click **Options**.

![](FileSaveAsSTLOptions.gif)

| Setting | Get/Set Methods | Return Value  or  <Value>  or  <OnFlag> | Comment |
| Output as - Binary | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swSTLBinaryFormat)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swSTLBinaryFormat, <OnFlag>) | True |  |
| Output as - ASCII | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swSTLBinaryFormat)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swSTLBinaryFormat, <OnFlag>) | False |  |
| Output as - Unit | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swExportStlUnits)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swExportStlUnits, swLengthUnit\_e.<Value>) | Valid options as defined in swLengthUnit\_e:   * 0 = swMM (millimeters) * 1 = swCM (centimeters) * 2 = swMETER * 3 = swINCHES * 4 = swFEET |  |
| Resolution -  * Coarse * Fine * Custom | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swSTLQuality)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swSTLQuality, swSTLQuality\_e.<*Value*>) | See swSTLQuality\_e for valid options | Specifies the resolution of the output for STL files |
| Resolution - Deviation - Tolerance | ISldWorks::GetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swSTLDeviation)  ISldWorks::SetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swSTLDeviation, <Value>) | Double value | Specifies deviation tolerance, which controls whole-part tessellation; lower numbers generate files with greater whole-part accuracy |
| Resolution - Angle - Tolerance | ISldWorks::GetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swSTLAngleTolerance)  ISldWorks::SetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swSTLAngleTolerance, <Value>) | Double value | Specifies angle tolerance, which controls smaller detail tessellation; lower numbers generate files with greater small-detail accuracy, but those files take longer to generate |
| Resolution - Show STL info before file saving | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swSTLShowInfoOnSave)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swSTLShowInfoOnSave, <OnFlag>) | Boolean value | Specifies whether to show STL information before saving the file |
| Resolution - Preview before saving file | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swSTLPreview)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swSTLPreview, <OnFlag>) | Boolean value | Specifies whether faceted model preview is displayed in the graphics area |
| Do not translate STL output data to positive space | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swSTLDontTranslateToPositive)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swSTLDontTranslateToPositive, <OnFlag>) | Boolean value | Specifies whether exported parts maintain original position in global space, relative to origin |
| Save all components of an assembly in a single file | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swSTLComponentsIntoOneFile)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swSTLComponentsIntoOneFile, <OnFlag>) | Boolean value | Specifies whether to save the assembly and its components to a single file |
| Check for interferences | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swSTLCheckForInterference)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swSTLCheckForInterference, <OnFlag>) | Boolean value | Specifies whether to check for interference prior to saving assembly document; swUserPreferenceToggle\_e.swSTLComponentsIntoOneFile must be set to true |

Obsolete Enumerators

| Enumerator | Comment |
| swFileSaveAsCoordinateSystem | Obsolete |