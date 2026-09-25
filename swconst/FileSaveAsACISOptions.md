<!-- source: swconst/FileSaveAsACISOptions.htm -->

# SOLIDWORKS API Help

# System Options > Export > ACIS

To display the dialog:

Click **Tools > Options > System Options > Export > ACIS** in **File
Format**.

- or -

1. Click **File > Save As**.
2. In **Save as type**, select **ACIS**.
3. Click **Options**.

![](FileSaveAsACISOptions.gif)

| Setting | Get/Set Methods | Return Value  or  <Value>  or  <OnFlag> | Comment |
| Output as - Solid/Surface geometry | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swAcisOutputGeometryPreference)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swAcisOutputGeometryPreference, swAcisOutputGeometryPreference\_e.swAcisOutputAsSolidAndSurface) | swAcisOutputGeometryPreference\_e.swAcisOutputAsSolidAndSurface |  |
| Output as - 3D curves | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swAcisOutputGeometryPreference)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swAcisOutputGeometryPreference, swAcisOutputGeometryPreference\_e.swAcisOutputAs3DCurves) | swAcisOutputGeometryPreference\_e.swAcisOutputAs3DCurves |  |
| Output as - Export sketch entities | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swAcisOutputGeometryPreference)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swAcisOutputGeometryPreference, swAcisOutputGeometryPreference\_e.swAcisOutputAs3DCurves\_IncludeSketchEnts) | swAcisOutputGeometryPreference\_e.swAcisOutputAs3DCurves\_IncludeSketchEnts |  |
| Output as - Version | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swAcisOutputVersion)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swAcisOutputVersion, swAcisOutputVersion\_e.<Value>) | See swAcisOutputVersion\_e for valid options |  |
| Output as - Unit | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swAcisOutputUnits)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swAcisOutputUnits, swLengthUnit\_e.<Value>) | See swLengthUnit\_e for valid options |  |
| Export face/edge properties | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swSATExportFaceEdgeProps)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swSATExportFaceEdgeProps, <OnFlag>) | Boolean value | Specifies whether to export face and edge properties |
| Split periodic faces | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swSATExportSplitPeriodic)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swSATExportSplitPeriodic, <OnFlag>) | Boolean value | Specifies whether to split periodic faces on export |
| Write multi body part into a single ACIS body | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swSATExportMultLumpsToSingleBody)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swSATExportMultLumpsToSingleBody, <OnFlag>) | Boolean value |  |