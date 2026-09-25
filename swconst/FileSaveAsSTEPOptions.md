<!-- source: swconst/FileSaveAsSTEPOptions.htm -->

# SOLIDWORKS API Help

# System Options > Export > STEP

This topic contains two tables. The information in the table:

* appearing immediately after the screen capture corresponds to the settings
  on that dialog.
* titled [Miscellaneous
  Enumerators](#Miscellaneous) contains enumerators related to saving STEP data.
* titled [Obsolete
  Enumerators](#Obsolete) contains enumerators that previously appeared on the dialog but are now obsolete.

To display the dialog:

Click **Tools > Options > System Options > Export
>
STEP** in **File Format**.

- or -

1. Click **File > Save As**.
2. In **Save as type**, select **STEP AP203** or **STEP AP214**.
3. Click **Options**.

![](FileSaveAsSTEPOptions.gif)

| Setting | Get/Set Methods | Return Value  or  <Value> | Comment |
| Output as - Solid/Surface geometry | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swStepExportPreference)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swStepExportPreference, swAcisOutputGeometryPreference\_e.swAcisOutputAsSolidAndSurface) | swAcisOutputGeometryPreference\_e.swAcisOutputAsSolidAndSurface |  |
| Output as - Wireframe | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swStepExportPreference)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swStepExportPreference, swAcisOutputGeometryPreference\_e.swAcisOutputAs3DCurves) | swAcisOutputGeometryPreference\_e.swAcisOutputAs3DCurves |  |
| Output as - Wireframe - Export sketch entities | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swStepExportPreference)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swStepExportPreference, swAcisOutputGeometryPreference\_e.swAcisOutputAs3DCurves\_IncludeSketchEnts) | swAcisOutputGeometryPreference\_e.swAcisOutputAs3DCurves\_IncludeSketchEnts |  |
| Set STEP configuration data | IModelDocExtension::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swStepExportConfigurationData, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swStepExportConfigurationData, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, <Value>) | Boolean value | Specifies whether to export STEP configuration data |
| Export face/edge properties | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swStepExportFaceEdgeProps)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swStepExportFaceEdgeProps, <OnFlag>) | Boolean value | Specifies whether to export face and edge properties |
| Split periodic faces | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swStepExportSplitPeriodic)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swStepExportSplitPeriodic, <OnFlag>) | Boolean value | Specifies whether to split periodic faces on export |
| Export 3D Curve features | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swStepExport3DCurveFeatures)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swStepExport3DCurveFeatures, <OnFlag>) | Boolean value | Specifies whether to include 3D curve features in the exported file |

Miscellaneous Enumerators

| Enumerator | Get/Set Methods | Return Value  or  <Value> | Comment |
| swStepAP | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swStepAP)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swStepAP, <Value>) | Integer value:   * 203 = STEP AP203 format * 214 = STEP AP214 format | Specifies STEP version number for files saved as STEP |

Obsolete Enumerators

| Enumerator | Comment |
| swFileSaveAsCoordinateSystem | Obsolete |