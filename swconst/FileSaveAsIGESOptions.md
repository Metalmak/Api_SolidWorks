<!-- source: swconst/FileSaveAsIGESOptions.htm -->

# SOLIDWORKS API Help

# System Options > Export > IGES 5.3

This topic contains two tables. The information in the table:

* appearing immediately after the screen capture corresponds to the
  settings on that dialog.
* titled [Obsolete
  Enumerators](#Obsolete) contains enumerators that previously appeared on the dialog but are now obsolete.

To display the dialog:

Click **Tools > Options > System Options > Export
> IGES 5.3** in **File Format**.

- or -

1. Click **File > Save As**.
2. In **Save as type**, select **IGES**.
3. Click **Options**.

![](FileSaveAsIGESOptions.gif)

| Setting | Get/Set Methods | Return Value  or  <Value>  or  <OnFlag> | Comment |
| Solid/Surface features - Output as - IGES solid/surface entities | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swIGESExportSolidAndSurface)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swIGESExportSolidAndSurface, <OnFlag>) | Boolean value | Specifies whether to export data as solid or surface entities |
| Solid/Surface features - Output as - IGES solid/surface entities <value> | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swIGESRepresentation)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swIGESRepresentation, swIGESRepresentation\_e.<Value>) | See swIGESRepresentation\_e for valid options | Specifies IGES representation type |
| Solid/Surface features - Output as - IGES wireframe (3D curves) | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swIGESExportAsWireframe)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swIGESExportAsWireframe, <OnFlag>) | Boolean value | Specifies whether to convert solid body to a 3D wireframe representation in the IGES file |
| Solid/Surface features - Output as - IGES wireframe (3D curves) <value> | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swIGESCurveRepresentation)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swIGESCurveRepresentation, swIGESCurveRepresentation\_e.<Value>) | See swIGESCurveRepresentation\_e for valid options | Specifies the IGES curve representation |
| Solid/Surface features - Surface representation/System preference | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swIGESSystem)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swIGESSystem, swIGESPreferredSystem\_e.<Value>) | See swIGESPreferredSystem\_e for valid options | Specifies the IGES system setting |
| Export 3D Curve features | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swIGESExportFreeCurves)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swIGESExportFreeCurves, <OnFlag>) | Boolean value | Specifies whether to include 3D curve features in the exported file |
| Export sketch entities | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swIGESExportSketchEntities)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swIGESExportSketchEntities, <OnFlag>) | Boolean value | Specifies whether to export sketch entities |
| Use high trim curve accuracy | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swIGESHighTrimCurveAccuracy)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swIGESHighTrimCurveAccuracy, <OnFlag>) | Boolean value | Specifies whether to use high-trim curve accuracy |
| IGES assembly structure - Save all components of an assembly in one file | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swIGESComponentsIntoOneFile)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swIGESComponentsIntoOneFile, <OnFlag>) | Boolean value | Specifies whether to save all assembly components, sub-assemblies, and sub-assembly components in one file; for assemblies only |
| IGES assembly structure - Flatten assembly hierarchy | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swIGESFlattenAssemHierarchy)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swIGESFlattenAssemHierarchy, <OnFlag>) | Boolean value | Specifies whether to save assembly in flattened hierarchy (one level); for assemblies only |
| Split periodic faces | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swIGESExportSplitPeriodic)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swIGESExportSplitPeriodic, <OnFlag>) | Boolean value | Specifies whether to split periodic faces; for parts only |
| Output coordinate system: | ISldWorks::GetUserPreferenceStringValue(swUserPreferenceStringValue\_e.swExportOutputCoordinateSystem)  ISldWorks::SetUserPreferenceStringValue(swUserPreferenceStringValue\_e.swExportOutputCoordinateSystem, <Value>) | String value | Specifies a coordinate system name in the active document |

Obsolete Enumerators

| Enumerator | Comment |
| swIGESDuplicateEntities | Obsolete |
| swIGESNurbsSetting | Obsolete; see swUserPreferenceIntegerValue\_e.swIGESSystem |
| swIGESStandardSetting | Obsolete; see swUserPreferenceIntegerValue\_e.swIGESSystem |
| swFileSaveAsCoordinateSystem | Obsolete |