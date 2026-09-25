<!-- source: swconst/FileOpenOptions3MF.htm -->

# SOLIDWORKS API Help

# System Options > Import > 3MF

To display the dialog:

Select **Tools > Options > System Options > Import > File Format
> 3MF**.

- or -

1. Select **File > Open**.
2. In **Files of type**, select
   **3D Manufacturing Format**.
3. Click **Options**.

![](FileOpenOptions3MF.gif)

| Setting | Get/Set Methods | Return Value  or   <Value>  or  <OnFlag> | Comment |
| Import as - Graphics body | ISldWorks::GetUserPreferenceIntegerValue(swUserPerferenceIntegerValue\_e.swImportStlVrmlModelType) ISldWorks::SetUserPreferenceIntegerValue(swUserPerferenceIntegerValue\_e.swImportStlVrmlModelType, swImportStlVrmlModelType\_e.swImportStlVrmlModelType\_Graphics) | swImportStlVrmlModelType\_e.swImportStlVrmlModelType\_Graphics |  |
| Import as - Solid body | ISldWorks::GetUserPreferenceIntegerValue(swUserPerferenceIntegerValue\_e.swImportStlVrmlModelType) ISldWorks::SetUserPreferenceIntegerValue(swUserPerferenceIntegerValue\_e.swImportStlVrmlModelType, swImportStlVrmlModelType\_e.swImportStlVrmlModelType\_Solid) | swImportStlVrmlModelType\_e.swImportStlVrmlModelType\_Solid |  |
| Import as - Surface body | ISldWorks::GetUserPreferenceIntegerValue(swUserPerferenceIntegerValue\_e.swImportStlVrmlModelType) ISldWorks::SetUserPreferenceIntegerValue(swUserPerferenceIntegerValue\_e.swImportStlVrmlModelType, swImportStlVrmlModelType\_e.swImportStlVrmlModelType\_Surface) | swImportStlVrmlModelType\_e.swImportStlVrmlModelType\_Surface |  |
| Mesh body options - Create mesh bodies bounded by single faces | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swVrmlStlImportAsPSMesh)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swVrmlStlImportAsPSMesh, <OnFlag>) | Boolean value | Valid only when importing as Solid  body or Surface body, specifies whether to create mesh bodies bounded by single faces |
| Mesh body options - Group facets into faces | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swIVrmlStlImportSegmented)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swIVrmlStlImportSegmented, <OnFlag>) | Boolean value | Valid only if **Create mesh bodies bounded by single faces** is selected, specified whether to group facets into faces |
| Unit | ISldWorks::GetUserPreferenceIntegerValue(swUserPerferenceIntegerValue\_e.swImportStlVrmlUnits) ISldWorks::SetUserPreferenceIntegerValue(swUserPerferenceIntegerValue\_e.swImportStlVrmlUnits, swLengthUnit\_e.<Value>) | Valid options from swLengthUnit\_e:   * 0 = swMM (millimeters) * 1 = swCM (centimeters) * 2 = swMETER * 3 = swINCHES * 4 = swFEET |  |